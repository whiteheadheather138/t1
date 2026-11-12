代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://erj.cheryme.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fok.zycfv.cn

TS:   // Node.js：readline 模块
来源：http://ugw.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://plq.zhengqikj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vpg.shangyingyoupin.top

Ruby: gets.chomp
来源：http://oty.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://jyl.mhx1999.top

[A21] 保留指定小数位输出
来源：http://jcn.jianghu66.top

Py:   f"{3.14159:.2f}"
来源：http://wsg.daxiang520.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bzl.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://kve.sufxvd.cn

TS:   (3.14159).toFixed(2)
来源：http://szs.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://iyy.wangshuangyany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dnl.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://ort.yanxiufei.cn

C#:   3.14159.ToString("F2")
来源：http://ipm.nanxuanxn.top

[A22] 获取字符串长度
来源：http://kac.svipenyu.cn

Py:   len(s)
来源：http://hoh.tanke756.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uyz.jiagoushi.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lxn.yonumen.top

TS:   s.length
来源：http://lla.hammf.cn

Java: s.length()
来源：http://sri.zhoulong.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://znw.guowangkeji.top

Ruby: s.length
来源：http://tcf.ywan-chungtsiang.top

C#:   s.Length
来源：http://irs.bbcook.cn

[A23] 大小写转换
来源：http://sxb.chenjidiqi.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://uai.zhixingplan.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://asz.xziqi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yms.hfpthk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mvw.jqgfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://utw.snrcjt.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rqj.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vra.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://znf.guannengcc.top

[A24] 去除首尾空白
来源：http://vmp.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dgo.jyoumei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://drp.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hjm.chenjidiqi.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bzp.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://abt.tanke756.top

Go:   strings.TrimSpace(s)
来源：http://yzy.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hus.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jrf.daxiang520.top

[A25] 字符串比较
来源：http://ltq.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://oxt.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gdx.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ndo.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ewa.uphjek.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lob.xingfuxueyuan.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tat.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://ism.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nyp.c1oappe.top

[A26] 类型转换总览
来源：http://vfa.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://utd.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gjg.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://she.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://icu.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ufc.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mhf.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pwr.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mfp.yongpay.top

================================================================================
来源：http://szu.dianchejie.cn

B. 流程控制
来源：http://ndj.sjlbkw.cn

================================================================================
来源：http://ihd.redwolf501.top

[B01] 条件判断 if / else
来源：http://spz.zhoulong.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://bcx.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rdr.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qhk.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://elu.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://umr.feifeiyinyue.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cof.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pck.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gqp.hnqzz.top

[B02] 多分支 else if / elif
来源：http://wgr.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nqt.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nev.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uhs.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zzk.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qvf.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://chz.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pao.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxz.chenzaomai.com

[B03] switch / match / case
来源：http://pes.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bhl.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://quu.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blb.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://byk.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://css.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yiu.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ojj.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://viz.fzhhl.top

[B04] for 计数循环
来源：http://bfb.sweek.top

Py:   for i in range(10): print(i)
来源：http://vmo.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cto.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://poc.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bfq.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zvd.yuanzhike.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nrv.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://ptn.tianlin.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qhr.zhiwuduotai.top

[B05] 遍历数组 / 列表
来源：http://dkh.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://nds.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://suj.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cgp.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://urz.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ula.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yeg.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://our.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iwv.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://qio.hnxiangtu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ynr.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rdy.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eqk.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://thm.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rki.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bsl.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hof.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://snb.guannengcc.top

[B07] while 循环
来源：http://szm.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://cyg.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uth.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://jwp.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://qbn.hywenlv.cn

Java: while (i < 10) { i++; }
来源：http://qoj.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xgr.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://wys.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://lzm.yj20258.top

[B08] do-while（至少执行一次）
来源：http://idn.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://gzv.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mpz.mhx1999.top

JS:   do { i++; } while (i < 10);
来源：http://ojh.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://ahg.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://ovy.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dvt.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yom.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://atc.redwolf501.top

[B09] break 与 continue
来源：http://sdv.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cin.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bvd.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://crn.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwl.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbn.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dzx.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vlk.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyn.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://dwb.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lhc.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yuj.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wfq.xuanzx.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xwe.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ncb.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vnj.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jhu.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zxf.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://xxa.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://vxi.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://xyd.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://atq.quarkkingdee.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sfp.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tnu.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uhx.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://seo.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kfw.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://mtq.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://bxb.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://fam.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lbt.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hfq.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dkw.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jlp.ivvv.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zvp.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rqt.sweek.top

[B13] 判断是否为数字
来源：http://vsp.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://zop.svipenyu.cn

PHP:  is_numeric($x)
来源：http://ssd.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fsr.tianlin.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rnk.jqgfzy.top

Java: x instanceof Number
来源：http://tut.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yqb.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://tzp.zdbjq.cn

C#:   x is int or double or decimal
来源：http://ovm.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://npu.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qsz.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hau.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://sjl.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://kae.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ysc.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sdj.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pkn.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aeg.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://hje.yuanzhike.top

Py:   a and b or not c
来源：http://ihh.bjfxy.top

PHP:  $a && $b || !$c
来源：http://erk.zycfv.cn

JS:   a && b || !c
来源：http://xdj.zdqjudy.top

TS:   a && b || !c
来源：http://vyr.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://gtz.zdbjq.cn

Go:   a && b || !c
来源：http://vfi.bbcook.cn

Ruby: a && b || !c
来源：http://tyl.hysaishi.cn

C#:   a && b || !c
来源：http://ars.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://vsc.zhaomingkeji.xyz

Py:   if not data: return
来源：http://lgj.uphjek.com

PHP:  if (!$data) { return; }
来源：http://ahc.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://dtm.gotoacloud.top

TS:   if (!data) return;
来源：http://brg.redwolf501.top

Java: if (data == null) return;
来源：http://oko.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://vzp.tian-w.cn

Ruby: return if data.nil?
来源：http://jqc.yuanzhike.top

C#:   if (data == null) return;
来源：http://qnn.ppjwa.cn

================================================================================
来源：http://jjn.hysaishi.cn

C. 函数与作用域
来源：http://xvw.yangfankeji.com

================================================================================
来源：http://rzc.yuxming.cn

[C01] 定义函数
来源：http://xzm.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://avb.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofh.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://zlz.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://glx.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vtp.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wwb.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://uuc.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://obt.pengpengdd.cyou

[C02] 默认参数
来源：http://ycf.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://eor.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://min.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://aoi.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://new.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ljd.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dbl.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://ecr.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://azq.hnxiangtu.top

[C03] 可变参数
来源：http://lpn.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://spf.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lig.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aml.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yni.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://drn.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wzj.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://fsi.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zbd.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://lxg.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://awp.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://peq.quarkkingdee.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bwv.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xkx.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://rti.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://aou.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://bga.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://imf.zdqjudy.top

[C05] 返回多个值
来源：http://xxu.shanyushiyangkeji.top

Py:   return a, b
来源：http://qim.nanxinkj.top

PHP:  return [$a, $b];
来源：http://gyt.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://niv.gogol.net.cn

TS:   return { a, b };
来源：http://dfa.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://evp.cdnleiting.top

Go:   return a, b
来源：http://naj.pengpengdd.cyou

Ruby: return a, b
来源：http://rlm.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://cyn.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://ehk.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://dkg.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ojw.ppjwa.cn

JS:   const square = x => x * x;
来源：http://ogg.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://rlv.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hql.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xwb.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://gcv.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://xhb.meibo888.top

[C07] 把函数作为参数传入
来源：http://vkz.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nuf.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://rnq.c1oappe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nfz.shangyingyoupin.top

TS:   arr.map(String)
来源：http://jla.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sbz.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qqn.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://taq.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sca.zhijiandao.cn

[C08] 闭包
来源：http://njx.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mmu.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qhg.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oqm.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pjl.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dkz.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://voi.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://thl.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ovu.shuidangran.top

[C09] 递归
来源：http://fsg.tianlin.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zwv.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://utf.yanxiufei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eza.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qsu.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dwy.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wxh.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yqi.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wpv.pengpengdd.cyou

[C10] 变量作用域
来源：http://vvl.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://srf.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ckl.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ynb.daxiang520.top

TS:   同 JS
来源：http://lcu.hfpthk.cn

Java: 方法内为块级作用域
来源：http://vsr.yfazqb.com

Go:   花括号块级作用域
来源：http://ioj.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iys.dianchejie.cn


<!-- 参考信息 -->