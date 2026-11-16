代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ckp.yuanzhike.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vgu.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://dcb.iojbl.cn

TS:   (3.14159).toFixed(2)
来源：http://cuy.jinyuanbaomall.cn

Java: String.format("%.2f", 3.14159)
来源：http://yzd.smart0.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yjw.chenlongwang.top

Ruby: format("%.2f", 3.14159)
来源：http://lvi.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://ovl.yongpay.top

[A22] 获取字符串长度
来源：http://kyj.52xcode.cn

Py:   len(s)
来源：http://wnn.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bbm.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jbb.tanke756.top

TS:   s.length
来源：http://ulz.xuanzx.com

Java: s.length()
来源：http://dpb.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hlh.ybcxt.top

Ruby: s.length
来源：http://whp.ybcxt.top

C#:   s.Length
来源：http://cbn.yueranfly.top

[A23] 大小写转换
来源：http://pic.zhijiandao.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wet.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yim.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fwf.gogol.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gjt.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rnq.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ovq.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://job.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cte.hcnkem.com

[A24] 去除首尾空白
来源：http://tkk.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mzi.bbcook.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hjy.zhaomingkeji.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rqi.jyoumei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sew.hesvh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qpf.feifeiyinyue.top

Go:   strings.TrimSpace(s)
来源：http://yvu.gzhubu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://trl.daria6918.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oqq.yj20258888.top

[A25] 字符串比较
来源：http://mbf.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://uay.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iwd.sjlbkw.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://biw.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nno.zdbjq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qji.gzhubu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fla.nanxuanxn.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xii.zhaomingkeji.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xye.aibaodan.cn

[A26] 类型转换总览
来源：http://uza.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://snf.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wnk.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vxg.epnwcf.com

TS:   Number() String() Boolean() x as number
来源：http://chq.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ali.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ejb.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mtd.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://szf.jinqigfzy.top

================================================================================
来源：http://zhu.jlsjyb.cn

B. 流程控制
来源：http://okd.ydjk.org.cn

================================================================================
来源：http://xdn.yongpay.top

[B01] 条件判断 if / else
来源：http://pgl.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://elo.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nbf.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yae.zycfv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zfm.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zgd.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ezr.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://emg.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sqo.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://zbw.c1oappe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wej.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://klz.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eny.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzk.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppk.zycfv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yka.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pfr.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oko.tian-w.cn

[B03] switch / match / case
来源：http://doh.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lbw.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mkj.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bxt.wangdashe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wfj.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://thi.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jsa.mhx1999.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cdl.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tck.tianlin.xyz

[B04] for 计数循环
来源：http://ucy.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://joe.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sio.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fbm.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wpe.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vkf.aibaodan.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rie.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://mbc.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dpk.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://eqg.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://mqf.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zvt.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kmi.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mvr.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dzw.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tzh.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://ojv.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://frc.yongpay.top

[B06] 遍历字典 / 对象
来源：http://wfd.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wqi.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bnk.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uyu.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cru.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ueg.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cds.feifeiyinyue.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zfb.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kuo.pengpengdd.cyou

[B07] while 循环
来源：http://vsn.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://nzi.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://ded.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://mbr.guannengcc.top

TS:   while (i < 10) { i++; }
来源：http://xey.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://cxl.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xlv.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://snl.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://udr.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://mla.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://hud.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kvt.hnqzz.top

JS:   do { i++; } while (i < 10);
来源：http://noq.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://jst.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://efg.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cfs.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://okk.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://ely.svipenyu.cn

[B09] break 与 continue
来源：http://ujl.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tiw.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://teh.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qri.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqx.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnz.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://omn.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qff.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewc.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://wkn.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://syt.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tad.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wqj.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gpa.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ecq.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lqk.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wwv.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mjj.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://pah.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://bub.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://wgg.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://slf.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sjb.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xbl.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cav.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://wls.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vft.cucudq.cn

[B12] 跳出多层循环
来源：http://iie.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://usw.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mlz.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nxd.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://csz.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kww.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pwk.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aqs.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wfu.zdbjq.cn

[B13] 判断是否为数字
来源：http://gev.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://yru.hnqzz.top

PHP:  is_numeric($x)
来源：http://wxi.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qmx.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wsr.pengpengdd.cyou

Java: x instanceof Number
来源：http://rwn.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vzv.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://pxo.chenzaomai.com

C#:   x is int or double or decimal
来源：http://agj.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://kqc.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yaf.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fte.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://jlu.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://sug.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://svj.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rul.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://gok.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lpg.iojbl.cn

[B15] 布尔运算与取反
来源：http://mod.aizwys.cn

Py:   a and b or not c
来源：http://edz.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://buz.shanyushiyangtech.top

JS:   a && b || !c
来源：http://iam.tian-w.cn

TS:   a && b || !c
来源：http://acp.0kj1m.cn

Java: a && b || !c
来源：http://cgd.sufxvd.cn

Go:   a && b || !c
来源：http://grs.ctjpmb.com

Ruby: a && b || !c
来源：http://xzo.dianchejie.cn

C#:   a && b || !c
来源：http://lsa.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://enf.yangfankeji.com

Py:   if not data: return
来源：http://ity.yonumen.top

PHP:  if (!$data) { return; }
来源：http://uvh.shzxlz.cn

JS:   if (!data) return;
来源：http://wmx.yuanzhike.top

TS:   if (!data) return;
来源：http://ybf.daria6918.cn

Java: if (data == null) return;
来源：http://rbw.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://lku.haohaochexian.top

Ruby: return if data.nil?
来源：http://nbl.wangdashe.top

C#:   if (data == null) return;
来源：http://gqo.meibo888.top

================================================================================
来源：http://zzw.yuanzhike.top

C. 函数与作用域
来源：http://jge.pycfn.com

================================================================================
来源：http://oov.zhaomingkeji.xyz

[C01] 定义函数
来源：http://zdr.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://jyz.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://quu.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://itk.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sie.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pxn.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eqw.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://vss.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aus.ywan-chungtsiang.top

[C02] 默认参数
来源：http://mga.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://cvr.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mpp.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://vyj.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jrh.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zna.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vty.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://chv.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://xcz.fktsv.cn

[C03] 可变参数
来源：http://bdt.jinqigfzy.top

Py:   def total(*args): return sum(args)
来源：http://klg.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wdu.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sbh.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://olv.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kjv.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://plx.meibo888.top

Ruby: def total(*nums); nums.sum; end
来源：http://set.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uka.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://cel.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dan.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nsg.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ddd.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://isl.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://bul.yfazqb.com

Go:   // 无：用配置结构体参数
来源：http://syt.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://rju.sweek.top

C#:   f(a: 1, b: 2)
来源：http://dkb.yanxiufei.cn

[C05] 返回多个值
来源：http://trs.gzhubu.top

Py:   return a, b
来源：http://wfs.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://guz.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tuc.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://sdt.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aqm.xinyue.icu

Go:   return a, b
来源：http://kbz.ydzc1.top

Ruby: return a, b
来源：http://dpi.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://roz.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://sgi.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://gqe.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ayy.jianghu66.top

JS:   const square = x => x * x;
来源：http://vmt.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://fhk.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://obd.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://niu.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://xqe.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://nqp.birdmap.top

[C07] 把函数作为参数传入
来源：http://spe.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jcr.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://kbk.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vja.epnwcf.com

TS:   arr.map(String)
来源：http://xhh.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kgd.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://boc.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://htj.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gea.shanyushiyangkeji.top

[C08] 闭包
来源：http://jht.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sri.yfazqb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cid.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ayy.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bfu.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://odp.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dun.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://piy.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uki.snrcjt.cn

[C09] 递归
来源：http://oyl.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xlw.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ylo.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uvo.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fvm.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jff.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oqg.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fiu.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mzo.hongshengwenyu.top

[C10] 变量作用域
来源：http://qna.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pwb.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gva.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gzg.hnxiangtu.top

TS:   同 JS
来源：http://rbb.cdnleiting.top

Java: 方法内为块级作用域
来源：http://qsn.zhoulong.xyz

Go:   花括号块级作用域
来源：http://obx.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xnm.wangdashe.top

C#:   块级作用域
来源：http://ktt.zycfv.cn

[C11] 模块导入与导出
来源：http://tse.tarul.cn

Py:   from module import func
来源：http://fpa.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lib.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ocz.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nrz.shanyushiyangkeji.top

Java: import java.util.List;
来源：http://rmu.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bug.tianlin.xyz


<!-- 参考信息 -->