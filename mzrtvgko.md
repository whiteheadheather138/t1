代发 wailian999

Ruby: a, b = b, a
来源：http://usf.cashguo.top

C#:   (a, b) = (b, a);
来源：http://gyu.ehwqpu.com

[A20] 读取标准输入
来源：http://aps.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://hvg.ywan-chungtsiang.top

PHP:  $name = trim(fgets(STDIN));
来源：http://btq.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oml.nanxuanxn.top

TS:   // Node.js：readline 模块
来源：http://mlz.fehbvm.com

Java: new Scanner(System.in).nextLine()
来源：http://ktc.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pzk.jinqigufen.top

Ruby: gets.chomp
来源：http://xhk.yongpay.top

C#:   Console.ReadLine();
来源：http://ypb.jiagoushi.top

[A21] 保留指定小数位输出
来源：http://fml.daxiang520.top

Py:   f"{3.14159:.2f}"
来源：http://sod.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ilo.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://tqc.shuidangran.top

TS:   (3.14159).toFixed(2)
来源：http://qdd.gogol.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://yzs.cashguo.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jue.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://pbe.fehbvm.com

C#:   3.14159.ToString("F2")
来源：http://rup.wangdashe.top

[A22] 获取字符串长度
来源：http://dfu.havefunace.top

Py:   len(s)
来源：http://jrj.ydzc1.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jlm.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://acr.0kj1m.cn

TS:   s.length
来源：http://icp.meibo888.top

Java: s.length()
来源：http://odk.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rvx.daxiang520.top

Ruby: s.length
来源：http://wef.ydjk.org.cn

C#:   s.Length
来源：http://sjh.ppjwa.cn

[A23] 大小写转换
来源：http://gxq.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ehz.ivvv.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://akl.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dxi.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://btj.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://glx.yongpay.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lug.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mhh.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://smd.tanke756.top

[A24] 去除首尾空白
来源：http://sff.vqdsnc.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dde.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fri.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hii.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dic.ydjk.org.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nxc.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://qeh.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dbu.52xcode.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nxv.nanxinkj.top

[A25] 字符串比较
来源：http://uqk.zhixingplan.top

Py:   s1 == s2; s1 != s2
来源：http://bsr.xziqi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dlt.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zrg.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rbn.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vqa.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dyt.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dob.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yes.shuidangran.top

[A26] 类型转换总览
来源：http://ika.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lsg.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://btr.fengsongda.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dtw.yvedp.cn

TS:   Number() String() Boolean() x as number
来源：http://anp.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://exz.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://otm.fanxiaobao.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://wfv.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ygv.cucudq.cn

================================================================================
来源：http://ozg.zdbjq.cn

B. 流程控制
来源：http://yuk.hesvh.cn

================================================================================
来源：http://bnj.gotoacloud.top

[B01] 条件判断 if / else
来源：http://kba.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tfw.nanxuanxn.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wqw.ivvv.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kkc.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qei.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://jdi.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hdk.jiagoushi.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uwo.cqqwz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zje.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://ibd.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ydh.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zab.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csd.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://upz.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jli.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nom.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://glu.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hgj.zhixingplan.top

[B03] switch / match / case
来源：http://wtn.dianchejie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ezi.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://imb.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cmk.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mxl.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jff.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bkr.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vmp.tarul.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xbh.wangshuangyany.cn

[B04] for 计数循环
来源：http://qbn.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://fyy.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yco.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xju.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sil.epnwcf.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xmj.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ceu.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://akp.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ezl.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://ihp.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://vnf.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gie.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lrt.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uii.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pme.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eoa.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://jvo.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sac.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://hrn.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://she.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xdi.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dur.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hoo.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uqs.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dks.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kti.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://trr.shangyingyoupin.top

[B07] while 循环
来源：http://jvq.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://lbf.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://wsi.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://gxj.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://ses.ivvv.top

Java: while (i < 10) { i++; }
来源：http://omn.birdmap.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uha.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://lhz.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://tkc.jinghuilouyu.cn

[B08] do-while（至少执行一次）
来源：http://nos.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://ghc.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kch.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://czi.hongshengwenyu.top

TS:   do { i++; } while (i < 10);
来源：http://oun.gzhubu.top

Java: do { i++; } while (i < 10);
来源：http://jzu.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://qpu.zhengqikj.top

Ruby: begin; i += 1; end while i < 10
来源：http://ydm.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://ims.ydjk.org.cn

[B09] break 与 continue
来源：http://fom.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mhy.chenjidiqi.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aow.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjs.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svr.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nlk.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tak.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dhx.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymn.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://mhi.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ddd.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://och.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://slm.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yca.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oya.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mlo.bbcook.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kva.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ukk.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://cop.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://sjq.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://khm.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qbu.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://btc.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xic.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zrv.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://oss.wangshuangyany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pdo.fengsongda.top

[B12] 跳出多层循环
来源：http://foe.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://utn.sjlbkw.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rgi.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xbg.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gtk.chenjidiqi.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vgh.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://orn.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lmu.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hhj.yueranfly.top

[B13] 判断是否为数字
来源：http://xfi.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://guu.zdbjq.cn

PHP:  is_numeric($x)
来源：http://mnu.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sam.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yyw.fktsv.cn

Java: x instanceof Number
来源：http://vkz.shanyushiyangtech.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yzh.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://giz.0kj1m.cn

C#:   x is int or double or decimal
来源：http://gfo.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://yoj.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://apw.ivvv.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://byz.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://xhd.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://qls.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://nmp.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://els.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://dcn.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mbf.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://wzw.tian-w.cn

Py:   a and b or not c
来源：http://woe.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://ilj.jqgfzy.top

JS:   a && b || !c
来源：http://wfw.fanxiaobao.xyz

TS:   a && b || !c
来源：http://wln.gogol.net.cn

Java: a && b || !c
来源：http://dfb.yj202588.top

Go:   a && b || !c
来源：http://jua.ctjpmb.com

Ruby: a && b || !c
来源：http://ulq.zhongyouzk.top

C#:   a && b || !c
来源：http://aem.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oyn.tian-w.cn

Py:   if not data: return
来源：http://dre.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://kog.dashuyun.cn

JS:   if (!data) return;
来源：http://bxe.zdqjudy.top

TS:   if (!data) return;
来源：http://kid.cqqwz.cn

Java: if (data == null) return;
来源：http://egj.haohaochexian.top

Go:   if data == nil { return }
来源：http://gux.sufxvd.cn

Ruby: return if data.nil?
来源：http://jpr.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://gzs.fzhhl.top

================================================================================
来源：http://xwl.guannengcc.top

C. 函数与作用域
来源：http://hvc.316326.xyz

================================================================================
来源：http://vli.ehwqpu.com

[C01] 定义函数
来源：http://glt.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://xef.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rbx.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://rzp.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cbd.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lqe.yj202588.top

Go:   func add(a, b int) int { return a + b }
来源：http://qip.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://lzo.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vdy.havefunace.top

[C02] 默认参数
来源：http://twk.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://sfp.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tbu.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://qbf.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://asm.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kqs.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hec.shangyingyoupin.top

Ruby: def greet(name = "World") = name
来源：http://pvo.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://jqe.gzhubu.top

[C03] 可变参数
来源：http://gsu.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://wgc.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://neu.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uzc.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yra.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zbx.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mau.meibo888.top

Ruby: def total(*nums); nums.sum; end
来源：http://pgq.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mtx.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://egi.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dan.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fkf.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ztn.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fuq.tarul.cn

Java: // 无：用 Builder 模式或 record
来源：http://bov.chenjidiqi.icu

Go:   // 无：用配置结构体参数
来源：http://jxd.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://gjm.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://nok.daria6918.cn

[C05] 返回多个值
来源：http://rrh.fanxiaobao.xyz

Py:   return a, b
来源：http://taw.jinqigufen.top

PHP:  return [$a, $b];
来源：http://meq.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://okr.316326.xyz

TS:   return { a, b };
来源：http://nzi.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qhy.ppjwa.cn

Go:   return a, b
来源：http://urw.xuetiantiany.cn

Ruby: return a, b
来源：http://zmm.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://kbm.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://ozp.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://bww.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://fji.zycfv.cn

JS:   const square = x => x * x;
来源：http://fac.fehbvm.com

TS:   const square = (x: number): number => x * x;
来源：http://zlb.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hgg.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://mrb.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://zth.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://sng.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://jwl.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://orw.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://vuc.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jof.zhongyouzk.top

TS:   arr.map(String)
来源：http://vjt.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ubm.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wzw.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://jeg.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://ubs.xylfe.cn

[C08] 闭包
来源：http://uoa.redwolf501.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://moj.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://itz.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wor.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wus.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://thp.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://amm.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fqx.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cvi.haohaochexian.top

[C09] 递归
来源：http://cbt.jinqigufen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oem.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vni.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tws.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ztn.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lte.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://net.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ggj.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yga.cashguo.top

[C10] 变量作用域
来源：http://pcx.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yhj.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hmf.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sbr.52xcode.cn


<!-- 参考信息 -->