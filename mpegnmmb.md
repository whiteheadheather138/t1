代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vkm.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://kbu.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://asj.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://flt.hammf.cn

C#:   (int)'A'; (char)65
来源：http://cig.zdqjudy.top

[A19] 交换两个变量
来源：http://jjw.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://hue.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://evt.316326.xyz

JS:   [a, b] = [b, a];
来源：http://lkb.hesvh.cn

TS:   [a, b] = [b, a];
来源：http://xbs.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://emf.jinqigfzy.top

Go:   a, b = b, a
来源：http://zgq.zhijiandao.cn

Ruby: a, b = b, a
来源：http://wxd.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://fjj.cashguo.top

[A20] 读取标准输入
来源：http://tcy.uphjek.com

Py:   name = input("请输入：")
来源：http://rfu.sxryk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zlu.jiagoushi.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pgj.yj20258888.top

TS:   // Node.js：readline 模块
来源：http://eji.fanxiaobao.xyz

Java: new Scanner(System.in).nextLine()
来源：http://tcn.gaohongyu789.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://txg.jqgufenzy.top

Ruby: gets.chomp
来源：http://dtr.chenlongwang.top

C#:   Console.ReadLine();
来源：http://opg.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://jno.pengpengdd.cyou

Py:   f"{3.14159:.2f}"
来源：http://mwa.jiagoushi.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tvn.tarul.cn

JS:   (3.14159).toFixed(2)
来源：http://bep.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://ksk.ppjwa.cn

Java: String.format("%.2f", 3.14159)
来源：http://fie.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bzn.havefunace.top

Ruby: format("%.2f", 3.14159)
来源：http://dli.mhx1999.top

C#:   3.14159.ToString("F2")
来源：http://wvx.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://zoe.cheryme.top

Py:   len(s)
来源：http://anp.yfazqb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zfs.cheryme.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zxp.smart0.xyz

TS:   s.length
来源：http://qiy.vqdsnc.cn

Java: s.length()
来源：http://ftw.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qta.pengpengdd.cyou

Ruby: s.length
来源：http://air.dashuyun.cn

C#:   s.Length
来源：http://tlp.andypj.xyz

[A23] 大小写转换
来源：http://osc.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wlz.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zbb.chenzaomai.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kww.hammf.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ldp.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nut.wangdashe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cux.hammf.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tgh.jinghuilouyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wco.chenlongwang.top

[A24] 去除首尾空白
来源：http://rye.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uhf.vehdjk.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pla.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://odw.jiagoushi.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mny.52xcode.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uop.yueranfly.top

Go:   strings.TrimSpace(s)
来源：http://zob.hywenlv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yiq.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wjy.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://urn.ywan-chungtsiang.top

Py:   s1 == s2; s1 != s2
来源：http://tkw.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kiy.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gor.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://prz.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cqh.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wbj.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://nqx.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pdj.yonumen.top

[A26] 类型转换总览
来源：http://eot.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://luj.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nms.bbcook.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mis.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://vzp.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rug.xuetiantiany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xey.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://prt.sxryk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ias.shuidangran.top

================================================================================
来源：http://rvx.havefunace.top

B. 流程控制
来源：http://nba.snrcjt.cn

================================================================================
来源：http://jjf.316326.xyz

[B01] 条件判断 if / else
来源：http://fit.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zed.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ooa.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rlk.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jiv.sysykeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gjw.yongpay.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ygf.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iry.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mdk.sysykeji.top

[B02] 多分支 else if / elif
来源：http://fum.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aos.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pkm.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nhr.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eif.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nlz.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wjf.yanxiufei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uey.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zcq.jinghuilouyu.cn

[B03] switch / match / case
来源：http://ivc.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pil.hywenlv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ozd.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jrp.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lhn.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gif.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qwi.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rmo.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nhg.yj202588.top

[B04] for 计数循环
来源：http://sgv.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://xde.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vsp.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qkf.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xyn.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ggz.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lwh.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://awo.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ikn.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://woh.fktsv.cn

Py:   for item in arr: print(item)
来源：http://own.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ptf.cdnleiting.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hgy.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iud.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rhe.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dkf.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://goj.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://agp.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://lfm.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://itj.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blb.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://egc.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://acq.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://isu.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hho.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gac.yfazqb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iuu.hcnkem.com

[B07] while 循环
来源：http://bni.ydzc1.top

Py:   while i < 10: i += 1
来源：http://knx.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eoj.sweek.top

JS:   while (i < 10) { i++; }
来源：http://xhl.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://gko.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://kvi.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jcy.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://znu.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://wvo.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://jnf.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://sgo.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://sae.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://dli.shanyushiyangtech.top

TS:   do { i++; } while (i < 10);
来源：http://ypv.zhiwuduotai.top

Java: do { i++; } while (i < 10);
来源：http://nlw.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dan.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nun.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://fqz.ppjwa.cn

[B09] break 与 continue
来源：http://fel.chenzaomai.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lfr.hfpthk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ale.pycfn.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ttn.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ird.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ius.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ihw.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lph.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhp.cdnleiting.top

[B10] 遍历同时拿索引
来源：http://fak.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ulf.kuanghao11.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://daz.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tqj.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nrk.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pdl.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ink.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iaa.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://asn.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://aqx.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://tis.ivvv.top

PHP:  range(0, 10, 2);
来源：http://dqg.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rza.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ikt.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sli.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ehr.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://ftb.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xxn.cheryme.top

[B12] 跳出多层循环
来源：http://bbr.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jsc.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bny.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://htw.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://njv.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jmd.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wym.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fgo.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nyn.svipenyu.cn

[B13] 判断是否为数字
来源：http://dbi.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://anh.wangdashe.top

PHP:  is_numeric($x)
来源：http://zyc.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lup.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bdi.haohaochexian.top

Java: x instanceof Number
来源：http://nhb.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ncz.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://paj.hammf.cn

C#:   x is int or double or decimal
来源：http://qkd.hammf.cn

[B14] 判断值是否在集合内
来源：http://ick.guowangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sew.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ras.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://lom.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://chl.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dvw.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lst.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://ood.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qzq.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://xya.tarul.cn

Py:   a and b or not c
来源：http://ieo.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://rrv.hysaishi.cn

JS:   a && b || !c
来源：http://rmp.aizwys.cn

TS:   a && b || !c
来源：http://kqt.epnwcf.com

Java: a && b || !c
来源：http://lot.zhixingplan.top

Go:   a && b || !c
来源：http://jhz.hnxiangtu.top

Ruby: a && b || !c
来源：http://dep.hammf.cn

C#:   a && b || !c
来源：http://uza.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://vri.jqgufenzy.top

Py:   if not data: return
来源：http://xou.zdqjudy.top

PHP:  if (!$data) { return; }
来源：http://dti.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://xhr.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://bjn.jqgufenzy.top

Java: if (data == null) return;
来源：http://vqa.ydjk.org.cn

Go:   if data == nil { return }
来源：http://swo.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://osn.dashuyun.cn

C#:   if (data == null) return;
来源：http://jsp.shanyushiyangtech.top

================================================================================
来源：http://yxw.feifeiyinyue.top

C. 函数与作用域
来源：http://bak.gotoacloud.top

================================================================================
来源：http://uzz.c1oappe.top

[C01] 定义函数
来源：http://nwm.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://acx.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fuu.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://ovg.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vuz.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gxm.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oql.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://oyl.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qae.dianchejie.cn

[C02] 默认参数
来源：http://xgq.yj202588.top

Py:   def greet(name="World"): return name
来源：http://gsu.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zni.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://iao.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zzw.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://aor.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jmo.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://ych.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://pgw.smart0.xyz

[C03] 可变参数
来源：http://zyk.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://ams.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jbi.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://evr.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hrz.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hak.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zmi.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://grr.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rch.cucudq.cn

[C04] 命名参数 / 关键字参数
来源：http://fjz.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lmz.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fuk.9152youxi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uoz.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hjs.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://bxl.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://jmh.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://gch.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://xnf.jqgfzy.top

[C05] 返回多个值
来源：http://mcp.yj202588.top

Py:   return a, b
来源：http://pku.hysaishi.cn

PHP:  return [$a, $b];
来源：http://ihw.nwbrower.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kab.xuetiantiany.cn

TS:   return { a, b };
来源：http://mpl.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wkg.guowangkeji.top

Go:   return a, b
来源：http://pee.52xcode.cn

Ruby: return a, b
来源：http://huf.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://fsp.tanke756.top

[C06] 匿名函数 / lambda
来源：http://dqn.sxryk.cn

Py:   square = lambda x: x * x
来源：http://sok.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fmq.aizwys.cn

JS:   const square = x => x * x;
来源：http://zio.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://jgj.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yqy.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://acd.ppjwa.cn

Ruby: square = ->(x) { x * x }
来源：http://sqm.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://gdq.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://ima.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lgw.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://xge.cqqwz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uin.bjfxy.top

TS:   arr.map(String)
来源：http://wxi.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dux.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lan.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://han.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uhr.yangfankeji.com

[C08] 闭包
来源：http://jaa.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vuu.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hhd.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sce.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gbh.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kmg.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gtg.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sem.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tbg.cucudq.cn

[C09] 递归
来源：http://mhq.zhengqikj.top


<!-- 参考信息 -->