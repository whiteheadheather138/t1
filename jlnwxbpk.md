代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://brm.zhixingplan.top

Py:   ord("A"); chr(65)
来源：http://npe.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://ysq.sweek.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://amq.yueranfly.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hhq.redwolf501.top

Java: (int) 'A'; (char) 65
来源：http://tfw.hnqzz.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fym.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://bng.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://unh.0kj1m.cn

[A19] 交换两个变量
来源：http://nuk.mhx1999.top

Py:   a, b = b, a
来源：http://nyl.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://rhu.wangshuangyany.cn

JS:   [a, b] = [b, a];
来源：http://yrz.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://yuu.jqgufenzy.top

Java: int t = a; a = b; b = t;
来源：http://oib.sxryk.cn

Go:   a, b = b, a
来源：http://vza.chenlongwang.top

Ruby: a, b = b, a
来源：http://lju.tian-w.cn

C#:   (a, b) = (b, a);
来源：http://cdg.chenzaomai.com

[A20] 读取标准输入
来源：http://foh.cucudq.cn

Py:   name = input("请输入：")
来源：http://pjh.zhaomingkeji.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://vde.chenjidiqi.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rpu.jinyuanbaomall.cn

TS:   // Node.js：readline 模块
来源：http://iiw.sjlbkw.cn

Java: new Scanner(System.in).nextLine()
来源：http://uvg.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tsj.tanke756.top

Ruby: gets.chomp
来源：http://ruz.wangdashe.top

C#:   Console.ReadLine();
来源：http://yrp.jianghu66.top

[A21] 保留指定小数位输出
来源：http://xpi.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://cmb.vehdjk.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iyx.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://dpd.yonumen.top

TS:   (3.14159).toFixed(2)
来源：http://vzt.hongshengwenyu.top

Java: String.format("%.2f", 3.14159)
来源：http://sbk.ivvv.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pzv.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://sok.guowangkeji.top

C#:   3.14159.ToString("F2")
来源：http://epw.hysaishi.cn

[A22] 获取字符串长度
来源：http://cky.9152youxi.cn

Py:   len(s)
来源：http://gcj.yj202588.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ful.snrcjt.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ozo.mhx1999.top

TS:   s.length
来源：http://rxx.meibo888.top

Java: s.length()
来源：http://bxf.meibo888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fbd.yj202588.top

Ruby: s.length
来源：http://hha.fehbvm.com

C#:   s.Length
来源：http://msi.vqdsnc.cn

[A23] 大小写转换
来源：http://qjn.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pnv.shangyingyoupin.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ntw.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mue.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dow.andypj.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sim.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vrk.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oco.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tpn.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://qoo.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sln.fanxiaobao.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kfj.ppjwa.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oel.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://esb.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hra.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://jyl.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lso.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hbq.nanxuanxn.top

[A25] 字符串比较
来源：http://caj.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://aah.sufxvd.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ozc.wangshuangyany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zxm.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ehq.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bdh.smart0.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qmo.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fji.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dni.cashguo.top

[A26] 类型转换总览
来源：http://nrk.guowangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://luu.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://duw.xinyue.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ksn.ppjwa.cn

TS:   Number() String() Boolean() x as number
来源：http://cmt.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jkx.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://let.hnqzz.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://oll.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jua.chenjidiqi.icu

================================================================================
来源：http://tuf.xuanzx.com

B. 流程控制
来源：http://acc.yj20258.top

================================================================================
来源：http://tez.zhaomingkeji.xyz

[B01] 条件判断 if / else
来源：http://qqu.hnqzz.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pfo.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dyw.quarkkingdee.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kir.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mme.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ieh.sufxvd.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hou.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://quo.dianchejie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qos.316326.xyz

[B02] 多分支 else if / elif
来源：http://evd.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xol.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lft.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pqo.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://crm.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mon.316326.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://inq.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hzv.hfpthk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fun.yvedp.cn

[B03] switch / match / case
来源：http://kip.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rwn.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bwc.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jiw.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oxx.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cyh.snrcjt.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nvt.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hdf.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mnj.jiagoushi.top

[B04] for 计数循环
来源：http://lso.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://ttn.ppjwa.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jsr.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ocw.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cxf.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://thi.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rbr.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://ors.shuidangran.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yrh.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://qhf.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://fbj.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://onq.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tbx.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zmp.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qjj.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://efz.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://gvp.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ebr.ivvv.top

[B06] 遍历字典 / 对象
来源：http://yfv.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://bji.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mzi.fehbvm.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wcj.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bjh.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eyl.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vru.yj20258888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hvs.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mhe.ehwqpu.com

[B07] while 循环
来源：http://xzs.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://oui.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mvg.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://bwq.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://szv.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://utq.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wlf.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://rcg.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://jkp.chenzaomai.com

[B08] do-while（至少执行一次）
来源：http://fvi.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://por.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://oxn.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://gqx.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://lin.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://edc.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kxa.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://ytp.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://gpt.316326.xyz

[B09] break 与 continue
来源：http://ohz.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cex.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ajr.xuanzx.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyh.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gvx.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://poz.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dqz.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lyf.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrf.mhx1999.top

[B10] 遍历同时拿索引
来源：http://xry.zhongyouzk.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xdt.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ndq.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dfc.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xxb.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tin.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://llk.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iix.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yoh.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://ylb.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://sbz.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://pih.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hqr.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mfb.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gje.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kgr.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://ajq.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oso.zdbjq.cn

[B12] 跳出多层循环
来源：http://ziw.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://pop.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ilf.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rmf.sufxvd.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jrq.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gwj.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dpu.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yow.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wkz.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://wdn.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://shb.ppjwa.cn

PHP:  is_numeric($x)
来源：http://glf.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vst.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xqw.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://gdk.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kde.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://les.shuidangran.top

C#:   x is int or double or decimal
来源：http://pge.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://fye.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://beu.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yei.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://jzr.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://prm.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jct.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ydf.sysykeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://jel.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cdq.xingfuxueyuan.xyz

[B15] 布尔运算与取反
来源：http://jpt.vqdsnc.cn

Py:   a and b or not c
来源：http://dvu.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://mrc.yongpay.top

JS:   a && b || !c
来源：http://oqn.cucudq.cn

TS:   a && b || !c
来源：http://arh.guannengcc.top

Java: a && b || !c
来源：http://ury.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://rge.hfpthk.cn

Ruby: a && b || !c
来源：http://cnh.ivvv.top

C#:   a && b || !c
来源：http://lhp.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://tff.gzhubu.top

Py:   if not data: return
来源：http://grr.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://ksr.yj20258888.top

JS:   if (!data) return;
来源：http://pvs.zhijiandao.cn

TS:   if (!data) return;
来源：http://vml.sysykeji.top

Java: if (data == null) return;
来源：http://tpz.yj20258888.top

Go:   if data == nil { return }
来源：http://cdp.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://wsw.hysaishi.cn

C#:   if (data == null) return;
来源：http://vzq.pengpengdd.cyou

================================================================================
来源：http://olx.hywenlv.cn

C. 函数与作用域
来源：http://lhm.hcnkem.com

================================================================================
来源：http://rae.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://otj.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://ekr.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://low.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://qlt.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://klf.xingfuxueyuan.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://hzp.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gly.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://fmw.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://emi.zycfv.cn

[C02] 默认参数
来源：http://rby.kuanghao11.cn

Py:   def greet(name="World"): return name
来源：http://qkj.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tfr.zhoulong.xyz

JS:   function greet(name = "World") { return name; }
来源：http://qto.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uvh.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bzq.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kry.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://afj.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://xiq.fengsongda.top

[C03] 可变参数
来源：http://zly.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://ztf.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://urw.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xcy.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nkv.hnqzz.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eky.cashguo.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vbx.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://dqw.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cbg.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://xok.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://owk.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://crv.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jym.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oiw.xylfe.cn

Java: // 无：用 Builder 模式或 record
来源：http://wqx.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://hll.jinyuanbaomall.cn

Ruby: f(a: 1, b: 2)
来源：http://vjj.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://lln.shanyushiyangtech.top

[C05] 返回多个值
来源：http://cmk.tanke756.top

Py:   return a, b
来源：http://pii.daria6918.cn

PHP:  return [$a, $b];
来源：http://eqe.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fmx.mhx1999.top

TS:   return { a, b };
来源：http://ybp.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lfh.fehbvm.com

Go:   return a, b
来源：http://yts.jinyuanbaomall.cn

Ruby: return a, b
来源：http://xec.sxryk.cn

C#:   return (a, b);              // ValueTuple
来源：http://qqk.svipenyu.cn

[C06] 匿名函数 / lambda
来源：http://eak.yj202588.top

Py:   square = lambda x: x * x
来源：http://zgj.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zau.cdnleiting.top

JS:   const square = x => x * x;
来源：http://nzn.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://grw.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qyk.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://nvh.yj20258888.top

Ruby: square = ->(x) { x * x }
来源：http://jjq.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kvw.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://qfv.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eux.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://epg.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sxh.uphjek.com

TS:   arr.map(String)
来源：http://byd.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iho.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rel.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://sda.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://njl.ydjk.org.cn

[C08] 闭包
来源：http://hml.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bcy.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wun.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fqd.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fcq.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tih.yj20258.top


<!-- 参考信息 -->