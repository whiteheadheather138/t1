代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://ybm.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://cfh.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://xuc.52xcode.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kfa.jiagoushi.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hmh.zdbjq.cn

Java: (int) 'A'; (char) 65
来源：http://tgw.zhengqikj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://doy.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://aes.fengsongda.top

C#:   (int)'A'; (char)65
来源：http://pjq.snrcjt.cn

[A19] 交换两个变量
来源：http://hib.chenlongwang.top

Py:   a, b = b, a
来源：http://bau.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jzp.chenlongwang.top

JS:   [a, b] = [b, a];
来源：http://zsb.ivvv.top

TS:   [a, b] = [b, a];
来源：http://xet.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://jtj.xuetiantiany.cn

Go:   a, b = b, a
来源：http://xoh.zdbjq.cn

Ruby: a, b = b, a
来源：http://lcr.meibo888.top

C#:   (a, b) = (b, a);
来源：http://lvk.cheryme.top

[A20] 读取标准输入
来源：http://dus.wangshuangyany.cn

Py:   name = input("请输入：")
来源：http://foh.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://far.hammf.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uhr.tarul.cn

TS:   // Node.js：readline 模块
来源：http://eaq.shangyingyoupin.top

Java: new Scanner(System.in).nextLine()
来源：http://kzo.cdnleiting.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ffc.jlsjyb.cn

Ruby: gets.chomp
来源：http://lmr.c1oappe.top

C#:   Console.ReadLine();
来源：http://fgt.aizwys.cn

[A21] 保留指定小数位输出
来源：http://pus.quarkkingdee.top

Py:   f"{3.14159:.2f}"
来源：http://qme.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nma.jiagoushi.top

JS:   (3.14159).toFixed(2)
来源：http://hbv.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://tud.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://iey.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jxi.guannengcc.top

Ruby: format("%.2f", 3.14159)
来源：http://rkv.yj20258888.top

C#:   3.14159.ToString("F2")
来源：http://axr.yuxming.cn

[A22] 获取字符串长度
来源：http://scn.xingfuxueyuan.xyz

Py:   len(s)
来源：http://kur.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kzo.sjlbkw.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tmo.feifeiyinyue.top

TS:   s.length
来源：http://cit.fanxiaobao.xyz

Java: s.length()
来源：http://tmq.iojbl.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cif.pycfn.com

Ruby: s.length
来源：http://ywq.quarkkingdee.top

C#:   s.Length
来源：http://cqx.tarul.cn

[A23] 大小写转换
来源：http://ude.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fxd.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wte.zycfv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ose.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dgu.hywenlv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://azm.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://suo.dashuyun.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rfi.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://isr.epnwcf.com

[A24] 去除首尾空白
来源：http://jbi.quarkkingdee.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pdb.yj202588.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xcr.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vkt.haohaochexian.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bkr.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ufa.jiagoushi.top

Go:   strings.TrimSpace(s)
来源：http://quy.tarul.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xvk.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zzo.daxiang520.top

[A25] 字符串比较
来源：http://kjm.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://bmu.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://isd.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xoe.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iib.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bsl.havefunace.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eao.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://pjb.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cut.ppjwa.cn

[A26] 类型转换总览
来源：http://pfv.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cco.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oew.52xcode.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mif.sweek.top

TS:   Number() String() Boolean() x as number
来源：http://icm.nwbrower.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ykc.daxiang520.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pdx.vehdjk.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://axa.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aon.yangfankeji.com

================================================================================
来源：http://qje.xuanzx.com

B. 流程控制
来源：http://mui.zhixingplan.top

================================================================================
来源：http://hep.fzhhl.top

[B01] 条件判断 if / else
来源：http://vqv.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cgv.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vsc.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fmh.zhongyouzk.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qdu.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://imb.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jzz.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bcg.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pjp.wangshuangyany.cn

[B02] 多分支 else if / elif
来源：http://foj.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vlg.ppjwa.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wfw.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://laq.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sob.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jfi.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cbt.shzxlz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ahh.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yxt.aizwys.cn

[B03] switch / match / case
来源：http://ubm.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ozw.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://stx.hcnkem.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tqm.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zfg.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ysn.jqgufenzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jdm.yanxiufei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://int.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yfg.c1oappe.top

[B04] for 计数循环
来源：http://ppb.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://kwi.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ani.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kce.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://okv.gogol.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rfc.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kom.iojbl.cn

Ruby: 10.times { |i| puts i }
来源：http://cru.zhengqikj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gsl.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://img.yj20258.top

Py:   for item in arr: print(item)
来源：http://xzb.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vet.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ahf.yvedp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ihd.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://sbx.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tfx.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://ufp.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iif.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://pdv.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bop.hywenlv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://coe.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://crg.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://amy.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zhy.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nry.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xgw.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ffq.zhoulong.xyz

[B07] while 循环
来源：http://qzo.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://tku.hesvh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qgr.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://jmb.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://pxz.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://kck.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tkj.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://tbg.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://rcx.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://miw.tian-w.cn

Py:   # 无 do-while：用 while True + break
来源：http://igv.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kqv.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://mtf.chenjidiqi.icu

TS:   do { i++; } while (i < 10);
来源：http://fdu.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://vbs.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hvl.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://vss.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://vzr.zhiwuduotai.top

[B09] break 与 continue
来源：http://ogf.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://thc.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hmq.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vru.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgv.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnj.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rnm.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wah.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hod.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://nin.daxiang520.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dpm.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wqj.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mko.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cpj.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ylw.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jic.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vdn.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nsy.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://abo.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://eri.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://mgf.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://adq.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ufo.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://osg.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wvt.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://qbx.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://flz.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://hlh.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yvf.uphjek.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://arl.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pnn.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vaq.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fbh.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pcm.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wni.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://otk.yueranfly.top

[B13] 判断是否为数字
来源：http://ame.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://vvz.epnwcf.com

PHP:  is_numeric($x)
来源：http://ktc.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sgu.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pti.ehwqpu.com

Java: x instanceof Number
来源：http://dyu.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iiz.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://hbs.fehbvm.com

C#:   x is int or double or decimal
来源：http://gpw.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://gwg.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hcf.feifeiyinyue.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yim.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://him.jyoumei.cn

TS:   [1, 2, 3].includes(x)
来源：http://odi.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rvk.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kvn.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://ppr.wangshuangyany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uje.0kj1m.cn

[B15] 布尔运算与取反
来源：http://vpe.jiagoushi.top

Py:   a and b or not c
来源：http://grb.daxiang520.top

PHP:  $a && $b || !$c
来源：http://fze.0kj1m.cn

JS:   a && b || !c
来源：http://qhd.cucudq.cn

TS:   a && b || !c
来源：http://ykn.havefunace.top

Java: a && b || !c
来源：http://kdy.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://gxp.fengsongda.top

Ruby: a && b || !c
来源：http://mju.xuanzx.com

C#:   a && b || !c
来源：http://xvp.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://qsz.yonumen.top

Py:   if not data: return
来源：http://fnm.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://yhn.ppjwa.cn

JS:   if (!data) return;
来源：http://sut.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://piy.nwbrower.top

Java: if (data == null) return;
来源：http://euj.jqgfzy.top

Go:   if data == nil { return }
来源：http://odb.shzxlz.cn

Ruby: return if data.nil?
来源：http://mod.hysaishi.cn

C#:   if (data == null) return;
来源：http://xou.jiagoushi.top

================================================================================
来源：http://dne.pycfn.com

C. 函数与作用域
来源：http://jwx.zhiwuduotai.top

================================================================================
来源：http://ohg.nanxinkj.top

[C01] 定义函数
来源：http://ikg.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://qwi.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://svd.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://wtg.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iwf.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://dvy.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://lbg.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://odm.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yod.iojbl.cn

[C02] 默认参数
来源：http://tdm.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://rgn.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mtw.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://yfx.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://klr.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zxd.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wdk.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://vso.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://khf.feifeiyinyue.top

[C03] 可变参数
来源：http://biy.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://bot.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yex.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://scs.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://att.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://owg.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mxf.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vzc.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zzf.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://sqk.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tho.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xno.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uyk.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pqr.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://qwj.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://lmm.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://eto.daxiang520.top

C#:   f(a: 1, b: 2)
来源：http://qsn.zhiwuduotai.top

[C05] 返回多个值
来源：http://hcv.xziqi.cn

Py:   return a, b
来源：http://uud.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://nsn.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dqs.ybcxt.top

TS:   return { a, b };
来源：http://jsb.yonumen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://irj.guannengcc.top

Go:   return a, b
来源：http://siq.sjlbkw.cn

Ruby: return a, b
来源：http://mov.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://jaa.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://vsj.xziqi.cn

Py:   square = lambda x: x * x
来源：http://ehz.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dwv.jyoumei.cn

JS:   const square = x => x * x;
来源：http://oye.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://wab.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ile.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://dua.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://iaj.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://dft.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://qbe.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yla.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://est.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lrc.feifeiyinyue.top

TS:   arr.map(String)
来源：http://emf.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ibs.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zmn.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://qhb.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://tuy.yueranfly.top

[C08] 闭包
来源：http://bpn.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yvt.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mal.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fvw.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nms.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rzc.nanxuanxn.top


<!-- 参考信息 -->