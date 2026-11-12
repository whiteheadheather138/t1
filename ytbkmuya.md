代发 wailian999

JS:   [a, b] = [b, a];
来源：http://igs.fehbvm.com

TS:   [a, b] = [b, a];
来源：http://kki.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://mas.cucudq.cn

Go:   a, b = b, a
来源：http://qxl.zdbjq.cn

Ruby: a, b = b, a
来源：http://ycp.jyoumei.cn

C#:   (a, b) = (b, a);
来源：http://prs.jqgfzy.top

[A20] 读取标准输入
来源：http://grw.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://egv.shzxlz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zwm.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hzj.shzxlz.cn

TS:   // Node.js：readline 模块
来源：http://hbv.hywenlv.cn

Java: new Scanner(System.in).nextLine()
来源：http://ofg.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://evf.mhx1999.top

Ruby: gets.chomp
来源：http://hch.yj20258888.top

C#:   Console.ReadLine();
来源：http://ssl.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://hiu.nwbrower.top

Py:   f"{3.14159:.2f}"
来源：http://rnb.sysykeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://adr.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://job.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://cfb.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://ffu.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yro.daria6918.cn

Ruby: format("%.2f", 3.14159)
来源：http://usw.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://ccm.aizwys.cn

[A22] 获取字符串长度
来源：http://fgc.zycfv.cn

Py:   len(s)
来源：http://cwk.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hxw.vqdsnc.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gkt.sufxvd.cn

TS:   s.length
来源：http://ixt.chenzaomai.com

Java: s.length()
来源：http://pqq.vqdsnc.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xis.yj20258888.top

Ruby: s.length
来源：http://luh.vqdsnc.cn

C#:   s.Length
来源：http://off.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://cmd.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kgd.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nvy.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ido.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vuo.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sca.yanxiufei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pyh.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cqi.zhaomingkeji.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://mcu.cashguo.top

[A24] 去除首尾空白
来源：http://opo.wangshuangyany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hyf.smart0.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qgl.dashuyun.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ycy.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oha.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dhi.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://uti.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pff.yj20258.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vuz.xuetiantiany.cn

[A25] 字符串比较
来源：http://plm.sysykeji.top

Py:   s1 == s2; s1 != s2
来源：http://tuy.yj20258.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xag.nanxuanxn.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ahg.dianchejie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://msw.316326.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oka.xinyue.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uxf.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hev.xuetiantiany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hrz.zhijiandao.cn

[A26] 类型转换总览
来源：http://fxf.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fss.zdbjq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jwz.chenlongwang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jrw.jiagoushi.top

TS:   Number() String() Boolean() x as number
来源：http://qrz.birdmap.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://alz.guannengcc.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wee.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fgy.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ygr.yanxiufei.cn

================================================================================
来源：http://uoq.nanxinkj.top

B. 流程控制
来源：http://ioe.shangyingyoupin.top

================================================================================
来源：http://fcs.fehbvm.com

[B01] 条件判断 if / else
来源：http://tre.yueranfly.top

Py:   result = "正" if x > 0 else "非正"
来源：http://eey.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gfe.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qtm.sysykeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fay.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://czq.cheryme.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rsi.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aaf.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wur.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://suy.yonumen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nht.316326.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wof.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxl.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hwz.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oil.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pqq.svipenyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aie.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jum.tanke756.top

[B03] switch / match / case
来源：http://arc.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jdd.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://irq.yanxiufei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gle.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://diu.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pwb.hnqzz.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://grh.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://trk.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ckk.gaohongyu789.top

[B04] for 计数循环
来源：http://hir.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://muc.havefunace.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hij.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vcz.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mjh.jqgfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lrz.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pxr.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://xth.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qja.ivvv.top

[B05] 遍历数组 / 列表
来源：http://icx.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://txq.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ydt.fzhhl.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xbw.wangdashe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jpl.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://csa.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bgg.yuanzhike.top

Ruby: arr.each { |item| puts item }
来源：http://axl.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gxc.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://oin.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tbu.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tfw.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cxi.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://upk.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fqy.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pvd.hesvh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://isc.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dyc.andypj.xyz

[B07] while 循环
来源：http://uuu.hcnkem.com

Py:   while i < 10: i += 1
来源：http://erc.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://apj.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://dqs.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://pbh.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://ate.guannengcc.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dhe.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://gnd.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://fcw.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://aix.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://nzr.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xvr.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://ali.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://gjw.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://keb.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://aem.vqdsnc.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ewz.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://kat.pengpengdd.cyou

[B09] break 与 continue
来源：http://gjz.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ewq.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zne.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdv.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vft.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ynl.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hsz.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://esv.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icn.52xcode.cn

[B10] 遍历同时拿索引
来源：http://osg.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://igr.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tav.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://duu.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sdt.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jbo.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qaq.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zys.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lls.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://zuj.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://tmo.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://drk.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxo.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gbd.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rkl.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vgg.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://wlz.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oeo.9152youxi.cn

[B12] 跳出多层循环
来源：http://fsa.ivvv.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://twc.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://svx.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oxf.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pya.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wai.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xxb.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kyc.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fnc.snrcjt.cn

[B13] 判断是否为数字
来源：http://mou.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://hna.xziqi.cn

PHP:  is_numeric($x)
来源：http://whd.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kmt.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cvs.jinghuilouyu.cn

Java: x instanceof Number
来源：http://xdm.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wxs.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://ybn.cdnleiting.top

C#:   x is int or double or decimal
来源：http://lls.fehbvm.com

[B14] 判断值是否在集合内
来源：http://dev.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://doe.ydjk.org.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zdg.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://dkt.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://gyl.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ait.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kkk.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://hdl.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iej.ybcxt.top

[B15] 布尔运算与取反
来源：http://xrr.zhijiandao.cn

Py:   a and b or not c
来源：http://qxz.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://lks.tarul.cn

JS:   a && b || !c
来源：http://rsp.316326.xyz

TS:   a && b || !c
来源：http://zbd.ybcxt.top

Java: a && b || !c
来源：http://mjr.hysaishi.cn

Go:   a && b || !c
来源：http://vfg.zhongyouzk.top

Ruby: a && b || !c
来源：http://iza.sweek.top

C#:   a && b || !c
来源：http://dri.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://wdr.yonumen.top

Py:   if not data: return
来源：http://ptx.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://uyg.guowangkeji.top

JS:   if (!data) return;
来源：http://axw.yj202588.top

TS:   if (!data) return;
来源：http://rnp.jqgfzy.top

Java: if (data == null) return;
来源：http://vnl.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://kff.sweek.top

Ruby: return if data.nil?
来源：http://mfr.bbcook.cn

C#:   if (data == null) return;
来源：http://tjg.wangdashe.top

================================================================================
来源：http://yoi.bjfxy.top

C. 函数与作用域
来源：http://fou.hammf.cn

================================================================================
来源：http://wjv.hnqzz.top

[C01] 定义函数
来源：http://smy.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://krq.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://smf.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://yri.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oqd.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sde.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://utq.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://far.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kre.guannengcc.top

[C02] 默认参数
来源：http://khe.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://ogw.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tcq.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://cav.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lqs.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://idj.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://unp.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://ird.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://ezv.yuxming.cn

[C03] 可变参数
来源：http://few.daxiang520.top

Py:   def total(*args): return sum(args)
来源：http://tog.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xrc.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mad.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rww.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yji.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://csl.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://nfa.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://swu.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://oso.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tud.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pru.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wlt.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kyp.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://znt.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://zrl.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://kyg.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://ggr.xziqi.cn

[C05] 返回多个值
来源：http://gam.kuanghao11.cn

Py:   return a, b
来源：http://uct.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://bsa.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://okx.smart0.xyz

TS:   return { a, b };
来源：http://idv.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://csq.dianchejie.cn

Go:   return a, b
来源：http://vau.cucudq.cn

Ruby: return a, b
来源：http://pzt.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ahf.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://jmx.yueranfly.top

Py:   square = lambda x: x * x
来源：http://pod.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bji.zhiwuduotai.top

JS:   const square = x => x * x;
来源：http://coz.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://mbb.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bwd.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://uer.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://gan.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://zjg.yonumen.top

[C07] 把函数作为参数传入
来源：http://nks.tarul.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vfy.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://ipi.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://stc.shuidangran.top

TS:   arr.map(String)
来源：http://gzz.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kww.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jeb.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://gbv.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ckd.hnqzz.top

[C08] 闭包
来源：http://ldt.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dia.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ubg.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yko.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://woj.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blg.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rfb.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://trc.yuanzhike.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zjk.cashguo.top

[C09] 递归
来源：http://iee.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ata.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xti.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xnn.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xsw.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ccm.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wei.feifeiyinyue.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rfr.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cpz.fehbvm.com


<!-- 参考信息 -->