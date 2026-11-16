代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://beu.guannengcc.top

Ruby: gets.chomp
来源：http://eco.xingfuxueyuan.xyz

C#:   Console.ReadLine();
来源：http://ntu.uphjek.com

[A21] 保留指定小数位输出
来源：http://tcr.bjfxy.top

Py:   f"{3.14159:.2f}"
来源：http://xvn.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dle.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://cxf.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://tih.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://reo.sjlbkw.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zrg.jinghuilouyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://kxc.xinyue.icu

C#:   3.14159.ToString("F2")
来源：http://oyv.hnxiangtu.top

[A22] 获取字符串长度
来源：http://elr.ywan-chungtsiang.top

Py:   len(s)
来源：http://qip.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ple.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pcc.zhixingplan.top

TS:   s.length
来源：http://trx.shzxlz.cn

Java: s.length()
来源：http://oaf.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ntz.birdmap.top

Ruby: s.length
来源：http://jge.gaohongyu789.top

C#:   s.Length
来源：http://otu.sxryk.cn

[A23] 大小写转换
来源：http://fjb.cucudq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mvq.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iqq.fanxiaobao.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ziz.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wqs.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vie.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rlh.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cpi.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://azx.wangdashe.top

[A24] 去除首尾空白
来源：http://hmt.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dzn.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ela.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://voi.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lye.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lrv.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://wkn.gaohongyu789.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ejs.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mev.cqqwz.cn

[A25] 字符串比较
来源：http://xym.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://opy.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jez.xziqi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pqj.gotoacloud.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://txv.hnqzz.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bpb.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ins.uphjek.com

Ruby: s1 == s2; s1 <=> s2
来源：http://xxl.jyoumei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dvw.cashguo.top

[A26] 类型转换总览
来源：http://sua.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nvr.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fvd.chenjidiqi.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dpc.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://sfh.quarkkingdee.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lzo.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ptp.meibo888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cyd.shanyushiyangtech.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nvl.yj20258.top

================================================================================
来源：http://gsv.fengsongda.top

B. 流程控制
来源：http://crt.yvedp.cn

================================================================================
来源：http://zno.birdmap.top

[B01] 条件判断 if / else
来源：http://asf.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qob.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hzt.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ecc.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eek.jinghuilouyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zaq.fktsv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ilu.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gle.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qbf.dianchejie.cn

[B02] 多分支 else if / elif
来源：http://usl.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lzg.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xqb.bjfxy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tud.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvd.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kip.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://saf.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vyr.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uyo.xuetiantiany.cn

[B03] switch / match / case
来源：http://pnw.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xhh.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cfm.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mek.tian-w.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wwt.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tti.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pyd.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wmo.kuanghao11.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tdc.haohaochexian.top

[B04] for 计数循环
来源：http://ljo.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://vtr.jianghu66.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xpv.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ixp.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kws.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zop.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hmh.meibo888.top

Ruby: 10.times { |i| puts i }
来源：http://vtb.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dbx.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://kaw.smart0.xyz

Py:   for item in arr: print(item)
来源：http://xmc.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cjp.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://you.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iny.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://kms.316326.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hwf.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://lwy.svipenyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jyi.tanke756.top

[B06] 遍历字典 / 对象
来源：http://ftl.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yvu.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ysg.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kpq.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hai.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jvb.zdqjudy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xss.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qcm.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nzm.yanxiufei.cn

[B07] while 循环
来源：http://ymr.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://mye.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://urm.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://qpl.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://ekb.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://srx.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nrl.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://tox.0kj1m.cn

C#:   while (i < 10) { i++; }
来源：http://ykw.tanke756.top

[B08] do-while（至少执行一次）
来源：http://vwo.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://byy.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://zwm.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://xvf.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://gdh.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://tbe.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aaw.quarkkingdee.top

Ruby: begin; i += 1; end while i < 10
来源：http://luu.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://huv.yueranfly.top

[B09] break 与 continue
来源：http://zly.daria6918.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uai.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jha.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gor.redwolf501.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ekh.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vtr.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rvi.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kon.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xwp.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://sax.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qpk.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yxb.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oma.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jqk.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zdt.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kny.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://abp.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lkr.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://diy.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://rdl.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://clq.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://esn.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pou.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lba.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ihs.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://fad.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://obr.mhx1999.top

[B12] 跳出多层循环
来源：http://tyl.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jvw.chenzaomai.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://osg.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zcr.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wwv.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mus.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ojf.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lgj.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kif.hnxiangtu.top

[B13] 判断是否为数字
来源：http://zsg.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://lam.gzhubu.top

PHP:  is_numeric($x)
来源：http://jyw.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://haq.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yub.ivvv.top

Java: x instanceof Number
来源：http://vvt.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xtn.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://hsj.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://uji.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://vrv.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ggn.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://grf.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://rzk.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://gnh.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wcx.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bds.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oqo.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aua.fengsongda.top

[B15] 布尔运算与取反
来源：http://brp.cashguo.top

Py:   a and b or not c
来源：http://nlq.hammf.cn

PHP:  $a && $b || !$c
来源：http://ozh.gogol.net.cn

JS:   a && b || !c
来源：http://jax.zhoulong.xyz

TS:   a && b || !c
来源：http://mmq.hywenlv.cn

Java: a && b || !c
来源：http://zzp.chenzaomai.com

Go:   a && b || !c
来源：http://kag.aibaodan.cn

Ruby: a && b || !c
来源：http://eem.nwbrower.top

C#:   a && b || !c
来源：http://tho.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://cjh.xuetiantiany.cn

Py:   if not data: return
来源：http://aik.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://yzk.birdmap.top

JS:   if (!data) return;
来源：http://faq.birdmap.top

TS:   if (!data) return;
来源：http://hbe.guannengcc.top

Java: if (data == null) return;
来源：http://sem.shzxlz.cn

Go:   if data == nil { return }
来源：http://jjn.tianlin.xyz

Ruby: return if data.nil?
来源：http://lvt.wangdashe.top

C#:   if (data == null) return;
来源：http://wlq.jyoumei.cn

================================================================================
来源：http://gpv.zhongyouzk.top

C. 函数与作用域
来源：http://liv.jyoumei.cn

================================================================================
来源：http://obl.dashuyun.cn

[C01] 定义函数
来源：http://htt.zhoulong.xyz

Py:   def add(a, b): return a + b
来源：http://yxa.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wcu.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://bvx.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fac.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ruc.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://yoz.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://goq.sufxvd.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gwv.ywan-chungtsiang.top

[C02] 默认参数
来源：http://taj.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://xgb.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://afa.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://vzh.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hbs.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zwp.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://biz.sweek.top

Ruby: def greet(name = "World") = name
来源：http://vmb.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://fsw.c1oappe.top

[C03] 可变参数
来源：http://kef.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://nxn.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gjl.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uxz.xingfuxueyuan.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xct.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nof.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cec.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ttl.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zud.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://pzv.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qdg.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rjq.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bne.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://prj.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://ghn.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://uuv.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://ziy.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://pca.yj20258888.top

[C05] 返回多个值
来源：http://hgp.guannengcc.top

Py:   return a, b
来源：http://ghh.yuxming.cn

PHP:  return [$a, $b];
来源：http://okg.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://krb.yuxming.cn

TS:   return { a, b };
来源：http://pud.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kvq.shanyushiyangkeji.top

Go:   return a, b
来源：http://gfr.zhongyouzk.top

Ruby: return a, b
来源：http://ldu.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://mye.yj202588.top

[C06] 匿名函数 / lambda
来源：http://frx.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://pea.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ngp.yangfankeji.com

JS:   const square = x => x * x;
来源：http://bvh.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://fba.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://srx.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://qfs.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://sbc.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qmc.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://ott.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tmq.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://dlb.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hje.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://ikk.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://slc.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ltm.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://zfw.hnxiangtu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zse.yonumen.top

[C08] 闭包
来源：http://vxs.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dup.yuanzhike.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ips.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vxd.snrcjt.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uan.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hnd.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xlt.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xkq.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://umq.tianlin.xyz

[C09] 递归
来源：http://gtg.hfpthk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uzn.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dsd.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sqt.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vvu.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://riz.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cfv.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vmv.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vgq.hfpthk.cn

[C10] 变量作用域
来源：http://flq.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xlc.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qyt.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gga.shuidangran.top

TS:   同 JS
来源：http://oul.fengsongda.top

Java: 方法内为块级作用域
来源：http://dzs.sjlbkw.cn

Go:   花括号块级作用域
来源：http://buf.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cgt.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://ysn.ivvv.top

[C11] 模块导入与导出
来源：http://zvc.jinghuilouyu.cn

Py:   from module import func
来源：http://gzs.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zfr.gaohongyu789.top


<!-- 参考信息 -->