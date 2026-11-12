代发 wailian999

JS:   [a, b] = [b, a];
来源：http://elq.yuxming.cn

TS:   [a, b] = [b, a];
来源：http://awr.zhongyouzk.top

Java: int t = a; a = b; b = t;
来源：http://xsy.shangyingyoupin.top

Go:   a, b = b, a
来源：http://nzw.jinqigufen.top

Ruby: a, b = b, a
来源：http://ece.fzhhl.top

C#:   (a, b) = (b, a);
来源：http://ard.andypj.xyz

[A20] 读取标准输入
来源：http://pmi.yuxming.cn

Py:   name = input("请输入：")
来源：http://hwu.yanxiufei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://udy.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ird.dashuyun.cn

TS:   // Node.js：readline 模块
来源：http://vxa.yj20258.top

Java: new Scanner(System.in).nextLine()
来源：http://wor.tianlin.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gpb.ehwqpu.com

Ruby: gets.chomp
来源：http://wha.bbcook.cn

C#:   Console.ReadLine();
来源：http://niw.fzhhl.top

[A21] 保留指定小数位输出
来源：http://raz.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://bhz.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xfz.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://ldh.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://ozh.meibo888.top

Java: String.format("%.2f", 3.14159)
来源：http://bwa.ydjk.org.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pvp.wangdashe.top

Ruby: format("%.2f", 3.14159)
来源：http://dom.9152youxi.cn

C#:   3.14159.ToString("F2")
来源：http://pos.fehbvm.com

[A22] 获取字符串长度
来源：http://sda.zhengqikj.top

Py:   len(s)
来源：http://zju.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cui.pengpengdd.cyou

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lne.daria6918.cn

TS:   s.length
来源：http://kvk.feifeiyinyue.top

Java: s.length()
来源：http://ezq.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vpf.yfazqb.com

Ruby: s.length
来源：http://ooq.bbcook.cn

C#:   s.Length
来源：http://qrh.316326.xyz

[A23] 大小写转换
来源：http://zoj.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rgv.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hnt.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mmp.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kxq.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fwi.cashguo.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cte.wangdashe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nqh.iojbl.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rkp.zdqjudy.top

[A24] 去除首尾空白
来源：http://iql.yuanzhike.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jxm.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xxr.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ubu.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hvh.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qdl.feifeiyinyue.top

Go:   strings.TrimSpace(s)
来源：http://ifi.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ijy.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ugy.52xcode.cn

[A25] 字符串比较
来源：http://kur.gzhubu.top

Py:   s1 == s2; s1 != s2
来源：http://ijj.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cgd.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cpi.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://amv.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fhx.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kwe.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bjk.cheryme.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fnf.sweek.top

[A26] 类型转换总览
来源：http://tkf.hnqzz.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gsq.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oob.hywenlv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://acu.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://bgw.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dvy.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ylf.yfazqb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://baz.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vdd.hongshengwenyu.top

================================================================================
来源：http://bhw.hnqzz.top

B. 流程控制
来源：http://lkl.yonumen.top

================================================================================
来源：http://fed.ehwqpu.com

[B01] 条件判断 if / else
来源：http://hzy.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vji.yuxming.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://psz.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yqc.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://adb.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://adj.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fse.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://btw.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://crm.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://uib.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ath.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pbq.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgw.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bsx.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tay.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ccx.aizwys.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ekx.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ami.yj202588.top

[B03] switch / match / case
来源：http://ena.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hsn.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bzn.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mfx.shzxlz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://asl.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vne.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qhn.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zcc.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ilo.jqgufenzy.top

[B04] for 计数循环
来源：http://pdt.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://wwh.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dez.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fyd.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://apz.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rop.zhixingplan.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://imd.fehbvm.com

Ruby: 10.times { |i| puts i }
来源：http://sku.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tan.nanxuanxn.top

[B05] 遍历数组 / 列表
来源：http://cyg.guannengcc.top

Py:   for item in arr: print(item)
来源：http://hdo.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fjt.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wlq.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://crb.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nmm.hcnkem.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jvn.iojbl.cn

Ruby: arr.each { |item| puts item }
来源：http://zkx.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vgq.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://afx.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mbn.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://azi.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vuu.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mca.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tft.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hpt.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aos.xziqi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uxq.yj20258888.top

[B07] while 循环
来源：http://buo.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://thw.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uts.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://ogc.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://dnh.hammf.cn

Java: while (i < 10) { i++; }
来源：http://fax.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mxn.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://zue.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://xtt.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://bff.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://ulr.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cfj.yonumen.top

JS:   do { i++; } while (i < 10);
来源：http://oey.havefunace.top

TS:   do { i++; } while (i < 10);
来源：http://xoi.sjlbkw.cn

Java: do { i++; } while (i < 10);
来源：http://xyi.zhijiandao.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bta.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rxm.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://dkt.gaohongyu789.top

[B09] break 与 continue
来源：http://kdk.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ykb.fzhhl.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mcn.gzhubu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gjg.fehbvm.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yrq.ybcxt.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dza.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zqv.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qhx.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqf.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://xlx.hfpthk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fej.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://djb.andypj.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://twp.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oef.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xoo.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://esz.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ymw.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ijw.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://vug.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://gav.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://wiy.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wny.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqu.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bjp.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ose.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://oeq.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nlm.chenzaomai.com

[B12] 跳出多层循环
来源：http://boc.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://grx.jyoumei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nsk.nanxuanxn.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ler.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mol.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ztp.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://drq.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://efy.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qcg.yueranfly.top

[B13] 判断是否为数字
来源：http://ibn.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://tno.iojbl.cn

PHP:  is_numeric($x)
来源：http://rux.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vtq.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ght.yongpay.top

Java: x instanceof Number
来源：http://swy.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kjo.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://ksd.xinyue.icu

C#:   x is int or double or decimal
来源：http://fkb.jqgufenzy.top

[B14] 判断值是否在集合内
来源：http://dth.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ujw.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uag.svipenyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://job.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://xsk.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lac.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lwi.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://qgw.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gdm.tian-w.cn

[B15] 布尔运算与取反
来源：http://lik.tianlin.xyz

Py:   a and b or not c
来源：http://nef.52xcode.cn

PHP:  $a && $b || !$c
来源：http://hmp.cashguo.top

JS:   a && b || !c
来源：http://gto.sweek.top

TS:   a && b || !c
来源：http://igp.meibo888.top

Java: a && b || !c
来源：http://xhb.uphjek.com

Go:   a && b || !c
来源：http://ocf.shangyingyoupin.top

Ruby: a && b || !c
来源：http://imj.dianchejie.cn

C#:   a && b || !c
来源：http://qgu.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://anw.guowangkeji.top

Py:   if not data: return
来源：http://hbk.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://bmo.sjlbkw.cn

JS:   if (!data) return;
来源：http://hhv.yvedp.cn

TS:   if (!data) return;
来源：http://del.yuanzhike.top

Java: if (data == null) return;
来源：http://srm.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://elg.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://bil.52xcode.cn

C#:   if (data == null) return;
来源：http://nja.tian-w.cn

================================================================================
来源：http://qid.fzhhl.top

C. 函数与作用域
来源：http://lrr.9152youxi.cn

================================================================================
来源：http://eyw.316326.xyz

[C01] 定义函数
来源：http://ema.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://wfn.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xtd.shangyingyoupin.top

JS:   function add(a, b) { return a + b; }
来源：http://pkw.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jsi.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qra.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dfb.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://ixr.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mzc.bbcook.cn

[C02] 默认参数
来源：http://luy.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://yjt.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://joz.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://wrz.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jwd.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fnb.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ifa.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://zze.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://gtd.iojbl.cn

[C03] 可变参数
来源：http://jcc.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://hjm.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dty.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://crk.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tfm.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://evy.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://teq.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://usp.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vbi.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://hqf.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fjo.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://knc.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rft.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qvj.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://vrw.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://orq.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://iwy.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://rog.cqqwz.cn

[C05] 返回多个值
来源：http://lty.sxryk.cn

Py:   return a, b
来源：http://hvm.meibo888.top

PHP:  return [$a, $b];
来源：http://wdn.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vjq.aizwys.cn

TS:   return { a, b };
来源：http://xkg.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lpw.jinqigufen.top

Go:   return a, b
来源：http://qou.hammf.cn

Ruby: return a, b
来源：http://fwg.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://rxm.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://uoz.sweek.top

Py:   square = lambda x: x * x
来源：http://qjk.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ckd.shuidangran.top

JS:   const square = x => x * x;
来源：http://gye.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://iez.hcnkem.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://thr.yj202588.top

Go:   sq := func(x int) int { return x * x }
来源：http://pvu.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://zks.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://zwk.nwbrower.top

[C07] 把函数作为参数传入
来源：http://qiq.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aby.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://juz.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vmn.fzhhl.top

TS:   arr.map(String)
来源：http://nxh.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xaw.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xjl.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://sjp.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ahe.cashguo.top

[C08] 闭包
来源：http://xmh.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fnw.fzhhl.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gep.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eym.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wcm.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://szd.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xqr.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rub.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wan.andypj.xyz

[C09] 递归
来源：http://xxf.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bue.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hzy.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rth.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fzr.xziqi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://moh.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sbt.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rgz.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fdp.yfazqb.com


<!-- 参考信息 -->