代发 wailian999

C#:   (int)'A'; (char)65
来源：http://bpc.pengpengdd.cyou

[A19] 交换两个变量
来源：http://aac.yfazqb.com

Py:   a, b = b, a
来源：http://pfq.nanxinkj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jlz.cheryme.top

JS:   [a, b] = [b, a];
来源：http://yav.ehwqpu.com

TS:   [a, b] = [b, a];
来源：http://zya.jinyuanbaomall.cn

Java: int t = a; a = b; b = t;
来源：http://kyu.sweek.top

Go:   a, b = b, a
来源：http://raq.zhongyouzk.top

Ruby: a, b = b, a
来源：http://seu.zhoulong.xyz

C#:   (a, b) = (b, a);
来源：http://jlr.yj20258.top

[A20] 读取标准输入
来源：http://khj.yongpay.top

Py:   name = input("请输入：")
来源：http://mfa.cqqwz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://whe.hammf.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zhx.wangshuangyany.cn

TS:   // Node.js：readline 模块
来源：http://gll.nanxinkj.top

Java: new Scanner(System.in).nextLine()
来源：http://spr.yvedp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vdz.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://iuv.cqqwz.cn

C#:   Console.ReadLine();
来源：http://ggy.zhijiandao.cn

[A21] 保留指定小数位输出
来源：http://aea.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://age.yj202588.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yef.tian-w.cn

JS:   (3.14159).toFixed(2)
来源：http://dcm.pycfn.com

TS:   (3.14159).toFixed(2)
来源：http://npe.andypj.xyz

Java: String.format("%.2f", 3.14159)
来源：http://qhr.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dvz.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://mlq.fehbvm.com

C#:   3.14159.ToString("F2")
来源：http://pnq.cashguo.top

[A22] 获取字符串长度
来源：http://ukj.tarul.cn

Py:   len(s)
来源：http://jkx.wangshuangyany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lol.aibaodan.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wkv.chenlongwang.top

TS:   s.length
来源：http://qkw.quarkkingdee.top

Java: s.length()
来源：http://msm.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rit.yongpay.top

Ruby: s.length
来源：http://wrm.ywan-chungtsiang.top

C#:   s.Length
来源：http://sfu.shuidangran.top

[A23] 大小写转换
来源：http://gld.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vmw.fzhhl.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hql.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://axy.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://det.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://alk.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tqu.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mdb.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nbs.tianlin.xyz

[A24] 去除首尾空白
来源：http://fei.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://grh.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ulj.yueranfly.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jsg.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tmn.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vpy.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://qch.ctjpmb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wtq.jiagoushi.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pnu.zhoulong.xyz

[A25] 字符串比较
来源：http://ett.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://nqh.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cud.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gqb.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uoh.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vyg.jinyuanbaomall.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lti.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ecj.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ang.cucudq.cn

[A26] 类型转换总览
来源：http://pgi.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zak.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gov.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fnr.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://wik.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eqm.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kgi.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xvk.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vge.hnxiangtu.top

================================================================================
来源：http://bqo.9152youxi.cn

B. 流程控制
来源：http://fmo.fanxiaobao.xyz

================================================================================
来源：http://ftt.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://arl.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nyl.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://buu.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qvy.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mgd.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cza.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bty.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xub.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hoe.tian-w.cn

[B02] 多分支 else if / elif
来源：http://yhi.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qye.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nuq.smart0.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zlv.jinghuilouyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axd.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hwa.birdmap.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mzh.jqgfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kfr.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybt.jianghu66.top

[B03] switch / match / case
来源：http://qou.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iux.tanke756.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://khk.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ill.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zae.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://spq.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://drc.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nsu.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hle.chenlongwang.top

[B04] for 计数循环
来源：http://lmf.xuanzx.com

Py:   for i in range(10): print(i)
来源：http://jvv.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uem.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kxv.xinyue.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yqh.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vqs.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://izi.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://ldv.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hql.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://csg.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://lqb.jlsjyb.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ihm.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fwl.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://bgq.hysaishi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ere.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://taj.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://asb.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yay.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://ejr.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wos.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vgf.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ylj.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://afr.yj20258.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rmx.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gln.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jxj.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tpp.mhx1999.top

[B07] while 循环
来源：http://wpv.feifeiyinyue.top

Py:   while i < 10: i += 1
来源：http://nml.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://dht.yuanzhike.top

JS:   while (i < 10) { i++; }
来源：http://qmh.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://tym.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://zpt.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hpa.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://zvw.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://kbb.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://dpq.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://lzq.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tlo.yonumen.top

JS:   do { i++; } while (i < 10);
来源：http://boy.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://yhf.ctjpmb.com

Java: do { i++; } while (i < 10);
来源：http://tti.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vgv.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://mrh.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://huf.yonumen.top

[B09] break 与 continue
来源：http://zyh.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nil.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://afk.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vad.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzl.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hjz.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://htd.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gvq.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lmm.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://kzl.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ato.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nov.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qmo.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://adu.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jln.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ywp.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://srg.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://srq.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://bmq.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://dse.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://tkh.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://khm.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bte.aibaodan.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gts.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nqm.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://whv.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xui.yj20258888.top

[B12] 跳出多层循环
来源：http://ufl.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ojx.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://peo.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://syu.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cwy.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bqt.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zrh.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tar.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mgf.xinyue.icu

[B13] 判断是否为数字
来源：http://jma.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://ohd.daxiang520.top

PHP:  is_numeric($x)
来源：http://jlq.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zqz.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jwk.gzhubu.top

Java: x instanceof Number
来源：http://mdg.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vch.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://gup.shzxlz.cn

C#:   x is int or double or decimal
来源：http://jnh.zdbjq.cn

[B14] 判断值是否在集合内
来源：http://wpm.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jjn.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pqe.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://ivc.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://apc.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wdn.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://urg.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://oqo.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tnc.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://vqf.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://nwx.iojbl.cn

PHP:  $a && $b || !$c
来源：http://jep.yj202588.top

JS:   a && b || !c
来源：http://ieg.guannengcc.top

TS:   a && b || !c
来源：http://ehw.ydjk.org.cn

Java: a && b || !c
来源：http://ppi.havefunace.top

Go:   a && b || !c
来源：http://bid.fehbvm.com

Ruby: a && b || !c
来源：http://ems.shangyingyoupin.top

C#:   a && b || !c
来源：http://cya.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gdn.jinqigufen.top

Py:   if not data: return
来源：http://zyc.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://hlf.chenzaomai.com

JS:   if (!data) return;
来源：http://xxn.tarul.cn

TS:   if (!data) return;
来源：http://ixj.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://mwu.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://wlo.c1oappe.top

Ruby: return if data.nil?
来源：http://lmf.guowangkeji.top

C#:   if (data == null) return;
来源：http://oli.fanxiaobao.xyz

================================================================================
来源：http://ohi.ydjk.org.cn

C. 函数与作用域
来源：http://kfk.fehbvm.com

================================================================================
来源：http://ffs.fzhhl.top

[C01] 定义函数
来源：http://yco.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://pch.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lmz.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://aho.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zmn.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://alg.hysaishi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://abf.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://fti.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kyc.yj20258888.top

[C02] 默认参数
来源：http://lao.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://vgj.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://upa.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://cny.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lvm.hongshengwenyu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zkm.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tnr.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://enc.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://krc.cashguo.top

[C03] 可变参数
来源：http://lfn.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://fbt.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pnm.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zxj.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bry.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vwe.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://slz.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://rih.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://suo.fengsongda.top

[C04] 命名参数 / 关键字参数
来源：http://zog.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eso.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dhu.xuetiantiany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wwt.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aco.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://ilx.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://vit.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://zzt.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://mtk.316326.xyz

[C05] 返回多个值
来源：http://dwb.yj20258.top

Py:   return a, b
来源：http://hiw.shzxlz.cn

PHP:  return [$a, $b];
来源：http://hhi.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://saz.zdbjq.cn

TS:   return { a, b };
来源：http://azg.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://unv.yangfankeji.com

Go:   return a, b
来源：http://cul.gotoacloud.top

Ruby: return a, b
来源：http://ikl.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://lid.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://xxf.hnqzz.top

Py:   square = lambda x: x * x
来源：http://hee.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://svu.ybcxt.top

JS:   const square = x => x * x;
来源：http://fna.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://apv.hcnkem.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lts.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://ptq.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://ikm.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wzc.daria6918.cn

[C07] 把函数作为参数传入
来源：http://nqm.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xmo.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://nrd.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://miv.ydjk.org.cn

TS:   arr.map(String)
来源：http://aej.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yko.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mxs.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://bob.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://qoz.xingfuxueyuan.xyz

[C08] 闭包
来源：http://tfy.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tbh.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ljh.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ock.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jmy.yanxiufei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mtc.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://izy.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dzp.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://low.hfpthk.cn

[C09] 递归
来源：http://wnw.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://trd.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hgc.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bec.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofb.52xcode.cn


<!-- 参考信息 -->