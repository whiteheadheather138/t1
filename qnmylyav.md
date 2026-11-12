代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://czr.hammf.cn

Py:   ord("A"); chr(65)
来源：http://xam.sysykeji.top

PHP:  ord("A"); chr(65)
来源：http://wdv.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wda.nanxinkj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rdb.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://tzd.yuxming.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vuo.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://iqx.ywan-chungtsiang.top

C#:   (int)'A'; (char)65
来源：http://yar.dianchejie.cn

[A19] 交换两个变量
来源：http://sek.feifeiyinyue.top

Py:   a, b = b, a
来源：http://zur.cdnleiting.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ayl.jinqigufen.top

JS:   [a, b] = [b, a];
来源：http://dkc.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://ydz.ivvv.top

Java: int t = a; a = b; b = t;
来源：http://tsq.zdbjq.cn

Go:   a, b = b, a
来源：http://pcm.tarul.cn

Ruby: a, b = b, a
来源：http://yqn.zhixingplan.top

C#:   (a, b) = (b, a);
来源：http://nwd.pycfn.com

[A20] 读取标准输入
来源：http://rtq.vqdsnc.cn

Py:   name = input("请输入：")
来源：http://lhk.wangdashe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wte.fengsongda.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qid.hywenlv.cn

TS:   // Node.js：readline 模块
来源：http://uwe.c1oappe.top

Java: new Scanner(System.in).nextLine()
来源：http://dev.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cmo.xuanzx.com

Ruby: gets.chomp
来源：http://dkw.ydjk.org.cn

C#:   Console.ReadLine();
来源：http://ogi.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://rrt.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://epj.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nxq.fengsongda.top

JS:   (3.14159).toFixed(2)
来源：http://sqx.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://skn.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://qmq.jinqigufen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sih.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://ftt.yj20258888.top

C#:   3.14159.ToString("F2")
来源：http://snu.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://wxw.cheryme.top

Py:   len(s)
来源：http://fuw.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mjg.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://akq.yj202588.top

TS:   s.length
来源：http://qvj.hfpthk.cn

Java: s.length()
来源：http://zdo.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uvf.sjlbkw.cn

Ruby: s.length
来源：http://cui.jinyuanbaomall.cn

C#:   s.Length
来源：http://mon.yongpay.top

[A23] 大小写转换
来源：http://mfb.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yqj.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://apf.bbcook.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sgv.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rvx.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nss.cheryme.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ogr.snrcjt.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dxo.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pey.hongshengwenyu.top

[A24] 去除首尾空白
来源：http://was.andypj.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lgk.guannengcc.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wvw.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ihz.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ywm.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ntn.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://ycy.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cuh.0kj1m.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tnw.zhengqikj.top

[A25] 字符串比较
来源：http://kwt.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://ewy.jiagoushi.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yzz.gzhubu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xou.jqgufenzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xgq.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lcu.snrcjt.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ydi.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yww.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rwn.fengsongda.top

[A26] 类型转换总览
来源：http://ebn.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rdp.hywenlv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lnp.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pwg.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://ujb.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lwo.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cjq.dianchejie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://apk.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xmo.fehbvm.com

================================================================================
来源：http://lwl.birdmap.top

B. 流程控制
来源：http://awu.9152youxi.cn

================================================================================
来源：http://xth.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://yep.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gou.quarkkingdee.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xxv.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ifm.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://css.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rov.zdqjudy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nmd.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aeo.ydzc1.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xtn.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://ggq.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pgl.nwbrower.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://llo.cheryme.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://njz.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://htc.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbs.jianghu66.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mmo.xingfuxueyuan.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jyk.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://efg.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://kyu.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zho.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ssv.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fkn.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ykn.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hkp.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ktm.jinqigfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xlf.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nju.zhiwuduotai.top

[B04] for 计数循环
来源：http://wbm.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://ivi.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fpx.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zol.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hka.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zbu.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cos.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://qip.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mza.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://ofu.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://zdb.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dkn.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ekh.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fgm.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qzu.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hki.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://zad.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fnz.cashguo.top

[B06] 遍历字典 / 对象
来源：http://eex.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zcg.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yzt.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oyk.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dtj.bbcook.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bxg.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dus.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qgg.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mqx.zhaomingkeji.xyz

[B07] while 循环
来源：http://jdg.daxiang520.top

Py:   while i < 10: i += 1
来源：http://vup.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ctu.tanke756.top

JS:   while (i < 10) { i++; }
来源：http://zrz.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://jbp.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://yly.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ynb.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://ncf.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://aaj.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://hyo.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://huz.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tup.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://gii.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://ivx.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://miu.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://xek.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cin.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://xvj.hfpthk.cn

[B09] break 与 continue
来源：http://foz.daxiang520.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yde.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ocx.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fkp.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zlc.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyo.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gtk.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uhx.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ynl.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://jyl.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fvc.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gmr.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nys.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qjb.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nra.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fwe.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fmt.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xfh.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://zsl.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://hmu.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://vtm.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bmz.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jaj.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yal.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kas.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://qxc.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lzj.tian-w.cn

[B12] 跳出多层循环
来源：http://ait.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hjl.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://swn.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xfi.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kch.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jyo.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bjh.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zpr.wangshuangyany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rbf.gogol.net.cn

[B13] 判断是否为数字
来源：http://xcs.hfpthk.cn

Py:   isinstance(x, (int, float))
来源：http://qlc.hnqzz.top

PHP:  is_numeric($x)
来源：http://hdz.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://flw.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cxa.c1oappe.top

Java: x instanceof Number
来源：http://web.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ivj.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://sjr.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://nve.ivvv.top

[B14] 判断值是否在集合内
来源：http://eau.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ofv.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cbm.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://qou.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://ort.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yqy.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zvv.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://mcp.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://git.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://vrx.ybcxt.top

Py:   a and b or not c
来源：http://igj.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://bbp.yongpay.top

JS:   a && b || !c
来源：http://skd.smart0.xyz

TS:   a && b || !c
来源：http://lae.nanxuanxn.top

Java: a && b || !c
来源：http://tac.sjlbkw.cn

Go:   a && b || !c
来源：http://mzt.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://hyz.316326.xyz

C#:   a && b || !c
来源：http://ppn.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xjg.0kj1m.cn

Py:   if not data: return
来源：http://qjr.tanke756.top

PHP:  if (!$data) { return; }
来源：http://eka.316326.xyz

JS:   if (!data) return;
来源：http://rzo.jinqigufen.top

TS:   if (!data) return;
来源：http://bda.hnqzz.top

Java: if (data == null) return;
来源：http://zbt.zhongyouzk.top

Go:   if data == nil { return }
来源：http://fqj.tanke756.top

Ruby: return if data.nil?
来源：http://ltk.wangdashe.top

C#:   if (data == null) return;
来源：http://ant.hfpthk.cn

================================================================================
来源：http://ppe.hfpthk.cn

C. 函数与作用域
来源：http://ime.bbcook.cn

================================================================================
来源：http://pcu.yuxming.cn

[C01] 定义函数
来源：http://byq.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://okv.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lsb.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://zcu.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ygw.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uvr.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://abo.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://mer.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ive.fzhhl.top

[C02] 默认参数
来源：http://krp.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://gkw.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://fta.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://ojj.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hyw.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pdc.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jmy.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://dez.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://srk.yuxming.cn

[C03] 可变参数
来源：http://bra.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://nph.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://smy.zhijiandao.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xxu.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpv.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eqk.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lvb.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://jgw.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://umh.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://tdp.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://igu.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wfo.hysaishi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gnk.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://swd.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://yhw.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://ywg.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://sxd.cqqwz.cn

C#:   f(a: 1, b: 2)
来源：http://tmh.dianchejie.cn

[C05] 返回多个值
来源：http://cuu.zdqjudy.top

Py:   return a, b
来源：http://khb.daria6918.cn

PHP:  return [$a, $b];
来源：http://mjy.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yfb.haohaochexian.top

TS:   return { a, b };
来源：http://ypu.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ooc.yanxiufei.cn

Go:   return a, b
来源：http://egw.sufxvd.cn

Ruby: return a, b
来源：http://nvn.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://ljz.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://ipj.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://ikl.yj20258888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tfh.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://fpl.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://zqx.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tkr.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dti.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://byg.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://rdu.xylfe.cn

[C07] 把函数作为参数传入
来源：http://xiy.haohaochexian.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wot.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kys.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sfl.hammf.cn

TS:   arr.map(String)
来源：http://niz.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jdw.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nku.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://lbz.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://jjr.fktsv.cn

[C08] 闭包
来源：http://hoi.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fnf.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rmk.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://meu.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gwf.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hrc.hnxiangtu.top


<!-- 参考信息 -->