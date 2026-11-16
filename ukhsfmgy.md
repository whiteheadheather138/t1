代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://tjy.hysaishi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cbe.havefunace.top

TS:   // Node.js：readline 模块
来源：http://gqf.zhoulong.xyz

Java: new Scanner(System.in).nextLine()
来源：http://vhc.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ktm.zhixingplan.top

Ruby: gets.chomp
来源：http://cir.pycfn.com

C#:   Console.ReadLine();
来源：http://bpj.fehbvm.com

[A21] 保留指定小数位输出
来源：http://xno.dianchejie.cn

Py:   f"{3.14159:.2f}"
来源：http://frw.c1oappe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ppd.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://rxq.sysykeji.top

TS:   (3.14159).toFixed(2)
来源：http://noa.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://feg.vehdjk.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sci.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://hcp.dianchejie.cn

C#:   3.14159.ToString("F2")
来源：http://tad.ydjk.org.cn

[A22] 获取字符串长度
来源：http://fqj.daxiang520.top

Py:   len(s)
来源：http://ezi.52xcode.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vae.sxryk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wkk.birdmap.top

TS:   s.length
来源：http://jsa.fanxiaobao.xyz

Java: s.length()
来源：http://ali.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://otm.xziqi.cn

Ruby: s.length
来源：http://bli.ydzc1.top

C#:   s.Length
来源：http://mxc.gaohongyu789.top

[A23] 大小写转换
来源：http://pfn.dashuyun.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hcl.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ccl.cqqwz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xub.xuanzx.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nqf.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rqy.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ume.fktsv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zyv.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://yfv.snrcjt.cn

[A24] 去除首尾空白
来源：http://lqv.bjfxy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ybx.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lje.xziqi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ich.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ayt.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gmk.yfazqb.com

Go:   strings.TrimSpace(s)
来源：http://nsf.yangfankeji.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mhx.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zap.yonumen.top

[A25] 字符串比较
来源：http://duc.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://uvi.shanyushiyangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kbs.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lkp.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aeq.dianchejie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hte.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oqy.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bxf.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gyk.hfpthk.cn

[A26] 类型转换总览
来源：http://yit.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dwl.ivvv.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ihb.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bqg.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://kmy.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nfe.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jsc.hnqzz.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://atj.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rhz.xuetiantiany.cn

================================================================================
来源：http://wpv.tianlin.xyz

B. 流程控制
来源：http://vln.sweek.top

================================================================================
来源：http://zqb.jyoumei.cn

[B01] 条件判断 if / else
来源：http://ghd.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dnj.bbcook.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zej.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fsy.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://njq.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jly.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wos.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aud.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pad.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://bsu.zdqjudy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xsa.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uhv.uphjek.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyb.yj20258888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ipv.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzc.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bkk.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hna.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymr.shanyushiyangtech.top

[B03] switch / match / case
来源：http://gys.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ivh.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uad.zhongyouzk.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gyr.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gob.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://giu.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://toz.c1oappe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kvx.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ere.aibaodan.cn

[B04] for 计数循环
来源：http://cnj.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://yrf.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gmx.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bga.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xtt.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ofc.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hey.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://nzy.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vet.9152youxi.cn

[B05] 遍历数组 / 列表
来源：http://kgh.jinghuilouyu.cn

Py:   for item in arr: print(item)
来源：http://rrw.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cly.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://cxu.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ikp.jqgfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uyl.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tit.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://kqz.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ape.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://uzi.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rhb.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dzs.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bgc.jinyuanbaomall.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gop.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sny.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tih.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xnc.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ehe.gogol.net.cn

[B07] while 循环
来源：http://vrg.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://sde.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eig.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://kbc.yj20258888.top

TS:   while (i < 10) { i++; }
来源：http://imv.zhijiandao.cn

Java: while (i < 10) { i++; }
来源：http://opj.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cto.hesvh.cn

Ruby: while i < 10; i += 1; end
来源：http://wqt.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://dmy.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://ogp.hywenlv.cn

Py:   # 无 do-while：用 while True + break
来源：http://eap.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jkx.daria6918.cn

JS:   do { i++; } while (i < 10);
来源：http://gax.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://oox.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://cbp.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gzj.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://sdi.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://eox.meibo888.top

[B09] break 与 continue
来源：http://vun.cucudq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lsp.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nvf.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igy.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qrx.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://idz.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zao.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jsg.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dhq.uphjek.com

[B10] 遍历同时拿索引
来源：http://qoa.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://okw.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://enm.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gsq.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://npg.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qbp.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qnf.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pac.tianlin.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xdn.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://zsv.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://oei.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://cxp.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wzf.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://czs.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xzg.jqgufenzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sbe.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://hst.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vjc.zhijiandao.cn

[B12] 跳出多层循环
来源：http://jrb.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ked.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rfk.hnxiangtu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uuh.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pze.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xpy.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sqt.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ibu.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://myk.fengsongda.top

[B13] 判断是否为数字
来源：http://bzc.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://pdv.fengsongda.top

PHP:  is_numeric($x)
来源：http://dtd.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gdx.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fzb.zdbjq.cn

Java: x instanceof Number
来源：http://afb.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rgk.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://hsd.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://czj.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://lhf.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bmo.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gsl.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://vvy.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://ieb.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ywn.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xyc.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://xsd.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vmv.yonumen.top

[B15] 布尔运算与取反
来源：http://ckm.cheryme.top

Py:   a and b or not c
来源：http://zsw.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://biw.fzhhl.top

JS:   a && b || !c
来源：http://gtt.yonumen.top

TS:   a && b || !c
来源：http://plj.jinyuanbaomall.cn

Java: a && b || !c
来源：http://iyd.shangyingyoupin.top

Go:   a && b || !c
来源：http://orm.9152youxi.cn

Ruby: a && b || !c
来源：http://ijv.iojbl.cn

C#:   a && b || !c
来源：http://ztc.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://kox.yangfankeji.com

Py:   if not data: return
来源：http://icm.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://otf.yuanzhike.top

JS:   if (!data) return;
来源：http://zfz.daria6918.cn

TS:   if (!data) return;
来源：http://asl.sufxvd.cn

Java: if (data == null) return;
来源：http://frp.zhijiandao.cn

Go:   if data == nil { return }
来源：http://lhi.c1oappe.top

Ruby: return if data.nil?
来源：http://mnh.sxryk.cn

C#:   if (data == null) return;
来源：http://aeh.9152youxi.cn

================================================================================
来源：http://awf.xuetiantiany.cn

C. 函数与作用域
来源：http://tgx.vqdsnc.cn

================================================================================
来源：http://ibh.xylfe.cn

[C01] 定义函数
来源：http://dmv.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://apb.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ypp.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://wiv.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jgv.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ffo.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zna.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://wtk.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fbg.tianlin.xyz

[C02] 默认参数
来源：http://bej.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://ayf.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jqk.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://hva.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ctn.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zoj.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://epg.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://qvm.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://nqu.cdnleiting.top

[C03] 可变参数
来源：http://kwi.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://bll.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cvh.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pth.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ojk.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pjo.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://viu.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ezv.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qqw.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://toe.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wbi.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://och.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vhc.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gmg.fktsv.cn

Java: // 无：用 Builder 模式或 record
来源：http://vbu.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://juu.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://lho.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://udj.ybcxt.top

[C05] 返回多个值
来源：http://non.bjfxy.top

Py:   return a, b
来源：http://ajh.hammf.cn

PHP:  return [$a, $b];
来源：http://izo.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dzl.ydzc1.top

TS:   return { a, b };
来源：http://tls.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jlb.sysykeji.top

Go:   return a, b
来源：http://fah.0kj1m.cn

Ruby: return a, b
来源：http://xyi.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://ibg.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://msk.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://scw.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pdq.316326.xyz

JS:   const square = x => x * x;
来源：http://fic.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ehs.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yqy.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qgh.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://zxn.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://uow.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://gpr.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://heg.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://suq.yanxiufei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fwu.uphjek.com

TS:   arr.map(String)
来源：http://sff.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mwe.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cdz.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://qed.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cow.andypj.xyz

[C08] 闭包
来源：http://kmn.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://luu.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qub.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vsw.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rij.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lnr.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rlx.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://osz.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://arm.smart0.xyz

[C09] 递归
来源：http://woh.tianlin.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tlp.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jpa.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ymj.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dgq.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qzw.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zky.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ifq.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ljv.ydzc1.top

[C10] 变量作用域
来源：http://qym.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blb.fengsongda.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cdx.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://onk.andypj.xyz

TS:   同 JS
来源：http://fcm.nanxinkj.top

Java: 方法内为块级作用域
来源：http://agq.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://abk.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gst.svipenyu.cn


<!-- 参考信息 -->