代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hbe.yvedp.cn

Java: (int) 'A'; (char) 65
来源：http://cit.yj20258.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bcg.snrcjt.cn

Ruby: "A".ord; 65.chr
来源：http://bpt.zhaomingkeji.xyz

C#:   (int)'A'; (char)65
来源：http://obk.chenlongwang.top

[A19] 交换两个变量
来源：http://ynf.cucudq.cn

Py:   a, b = b, a
来源：http://aau.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tuk.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://gmo.zdqjudy.top

TS:   [a, b] = [b, a];
来源：http://xeo.shangyingyoupin.top

Java: int t = a; a = b; b = t;
来源：http://raq.hywenlv.cn

Go:   a, b = b, a
来源：http://rzw.svipenyu.cn

Ruby: a, b = b, a
来源：http://vod.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://iib.zhengqikj.top

[A20] 读取标准输入
来源：http://akp.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://vhv.ydzc1.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bpg.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ymy.jinqigufen.top

TS:   // Node.js：readline 模块
来源：http://jti.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://vay.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nky.ehwqpu.com

Ruby: gets.chomp
来源：http://yqp.ybcxt.top

C#:   Console.ReadLine();
来源：http://slu.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://vsg.nanxuanxn.top

Py:   f"{3.14159:.2f}"
来源：http://fdf.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wka.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://mdf.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://dhh.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://ggs.andypj.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qyt.shanyushiyangtech.top

Ruby: format("%.2f", 3.14159)
来源：http://xjm.daria6918.cn

C#:   3.14159.ToString("F2")
来源：http://lhr.cdnleiting.top

[A22] 获取字符串长度
来源：http://tka.shangyingyoupin.top

Py:   len(s)
来源：http://dof.kuanghao11.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fwv.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nlo.ivvv.top

TS:   s.length
来源：http://pxh.xingfuxueyuan.xyz

Java: s.length()
来源：http://gdl.svipenyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pxg.hywenlv.cn

Ruby: s.length
来源：http://zxz.jinqigfzy.top

C#:   s.Length
来源：http://xbc.yueranfly.top

[A23] 大小写转换
来源：http://xkd.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ksp.smart0.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fqz.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hkm.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://idv.ctjpmb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lyj.jinghuilouyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mpy.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cvt.yfazqb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://fii.tarul.cn

[A24] 去除首尾空白
来源：http://kpk.chenzaomai.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nrh.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xlc.nwbrower.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://leg.shanyushiyangtech.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tso.shanyushiyangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cxz.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://lbw.yfazqb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fcp.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ftg.jqgufenzy.top

[A25] 字符串比较
来源：http://kic.zhaomingkeji.xyz

Py:   s1 == s2; s1 != s2
来源：http://qxv.ywan-chungtsiang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://evw.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ndf.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jrn.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xqp.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nak.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://omg.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cck.yueranfly.top

[A26] 类型转换总览
来源：http://fxv.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zwb.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://teo.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hkq.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://lho.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://egi.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ooo.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kdj.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gre.cucudq.cn

================================================================================
来源：http://qjl.wangdashe.top

B. 流程控制
来源：http://hde.aizwys.cn

================================================================================
来源：http://iaq.cdnleiting.top

[B01] 条件判断 if / else
来源：http://hbs.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://pdc.fanxiaobao.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yfh.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://crx.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gzg.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vvl.daxiang520.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xwg.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://anl.jianghu66.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jyk.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://imu.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cud.cheryme.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hin.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okb.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kfr.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ekx.kuanghao11.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ghw.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bsf.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://owm.aibaodan.cn

[B03] switch / match / case
来源：http://wrd.wangdashe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hvx.dianchejie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vvp.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://byf.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mbl.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zcx.shanyushiyangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uly.pycfn.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dvz.bbcook.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://plj.epnwcf.com

[B04] for 计数循环
来源：http://aeq.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://dox.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sou.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hbj.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hox.jqgfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mnz.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bqv.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://ymx.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rtn.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://jaa.feifeiyinyue.top

Py:   for item in arr: print(item)
来源：http://avt.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wuq.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ntt.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://azt.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hff.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nqt.hammf.cn

Ruby: arr.each { |item| puts item }
来源：http://qva.iojbl.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zkj.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://gzk.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bzm.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tka.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ayo.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://seg.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oud.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bed.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wmp.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://auo.zdbjq.cn

[B07] while 循环
来源：http://xix.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://ivi.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://vpa.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://gzh.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://pge.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://mvq.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lgx.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://vdk.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://uui.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://bsk.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://row.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hvh.nwbrower.top

JS:   do { i++; } while (i < 10);
来源：http://mrs.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://ujz.shzxlz.cn

Java: do { i++; } while (i < 10);
来源：http://eur.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ini.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://usa.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://vdm.nanxinkj.top

[B09] break 与 continue
来源：http://zrf.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rrb.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qdm.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hve.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jan.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rqy.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://evj.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ljb.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djj.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://sak.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qzq.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hux.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://acy.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fef.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://obn.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nbz.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gpf.iojbl.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oju.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://trw.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://vfd.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://bqi.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://irt.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qhk.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tmb.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://edd.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://pfq.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bjn.zhoulong.xyz

[B12] 跳出多层循环
来源：http://hob.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ycz.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nqy.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ofb.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ngj.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wjy.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bzc.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cbt.hywenlv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vsj.hcnkem.com

[B13] 判断是否为数字
来源：http://qox.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://wii.sufxvd.cn

PHP:  is_numeric($x)
来源：http://kts.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ryh.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ilx.jiagoushi.top

Java: x instanceof Number
来源：http://agp.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ddo.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://gbc.havefunace.top

C#:   x is int or double or decimal
来源：http://aum.hesvh.cn

[B14] 判断值是否在集合内
来源：http://kox.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zvp.chenzaomai.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bud.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://oug.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://ewy.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rsn.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://olr.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tkc.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jsz.ehwqpu.com

[B15] 布尔运算与取反
来源：http://lqn.kuanghao11.cn

Py:   a and b or not c
来源：http://liv.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://mod.jyoumei.cn

JS:   a && b || !c
来源：http://dmh.birdmap.top

TS:   a && b || !c
来源：http://dwh.ybcxt.top

Java: a && b || !c
来源：http://fny.dianchejie.cn

Go:   a && b || !c
来源：http://szq.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://flc.zhijiandao.cn

C#:   a && b || !c
来源：http://prd.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yqj.gaohongyu789.top

Py:   if not data: return
来源：http://jkg.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://nkc.iojbl.cn

JS:   if (!data) return;
来源：http://jhf.guowangkeji.top

TS:   if (!data) return;
来源：http://pef.pengpengdd.cyou

Java: if (data == null) return;
来源：http://peq.yfazqb.com

Go:   if data == nil { return }
来源：http://rvi.tanke756.top

Ruby: return if data.nil?
来源：http://prn.shzxlz.cn

C#:   if (data == null) return;
来源：http://omn.hnxiangtu.top

================================================================================
来源：http://qpt.havefunace.top

C. 函数与作用域
来源：http://ywy.xinyue.icu

================================================================================
来源：http://odh.zhoulong.xyz

[C01] 定义函数
来源：http://lpe.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://tzj.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uqb.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://xie.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://boh.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://hux.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://che.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://xyr.dashuyun.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ffn.tianlin.xyz

[C02] 默认参数
来源：http://kln.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://jlp.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kqx.jyoumei.cn

JS:   function greet(name = "World") { return name; }
来源：http://zts.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xhb.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cdx.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kfd.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://jlq.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://kyi.smart0.xyz

[C03] 可变参数
来源：http://itu.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://rge.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://obp.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fbc.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cev.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fcg.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tri.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://kap.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bco.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://vlt.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fmy.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iut.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vpz.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dyh.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://rkv.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://gwj.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://fjt.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://axf.hywenlv.cn

[C05] 返回多个值
来源：http://dxh.guowangkeji.top

Py:   return a, b
来源：http://drh.gzhubu.top

PHP:  return [$a, $b];
来源：http://dcd.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dvb.nanxuanxn.top

TS:   return { a, b };
来源：http://smg.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uyv.gogol.net.cn

Go:   return a, b
来源：http://ljl.jinyuanbaomall.cn

Ruby: return a, b
来源：http://rzb.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://gng.guannengcc.top

[C06] 匿名函数 / lambda
来源：http://qob.yuxming.cn

Py:   square = lambda x: x * x
来源：http://mcu.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hor.tian-w.cn

JS:   const square = x => x * x;
来源：http://clu.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://axs.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cal.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://roh.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://yet.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://tmf.ydzc1.top

[C07] 把函数作为参数传入
来源：http://xnr.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jdj.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://igx.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eia.zhongyouzk.top

TS:   arr.map(String)
来源：http://isk.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qqa.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yck.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://mqy.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rac.52xcode.cn

[C08] 闭包
来源：http://fzt.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yjn.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://myn.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ywd.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dto.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sou.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mri.sxryk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bmj.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wmk.pengpengdd.cyou

[C09] 递归
来源：http://bdz.52xcode.cn


<!-- 参考信息 -->