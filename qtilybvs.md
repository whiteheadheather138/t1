代发 wailian999

C#:   (int)'A'; (char)65
来源：http://qjf.zhijiandao.cn

[A19] 交换两个变量
来源：http://etv.hcnkem.com

Py:   a, b = b, a
来源：http://odu.shangyingyoupin.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zmo.redwolf501.top

JS:   [a, b] = [b, a];
来源：http://jca.feifeiyinyue.top

TS:   [a, b] = [b, a];
来源：http://aby.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://jhb.kuanghao11.cn

Go:   a, b = b, a
来源：http://zxv.ehwqpu.com

Ruby: a, b = b, a
来源：http://juq.guannengcc.top

C#:   (a, b) = (b, a);
来源：http://zyg.yj20258888.top

[A20] 读取标准输入
来源：http://jwn.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://ozg.shuidangran.top

PHP:  $name = trim(fgets(STDIN));
来源：http://oby.yj20258888.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aeo.shangyingyoupin.top

TS:   // Node.js：readline 模块
来源：http://qar.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://ldq.shzxlz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://shf.52xcode.cn

Ruby: gets.chomp
来源：http://vgb.yj20258888.top

C#:   Console.ReadLine();
来源：http://wca.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://amn.quarkkingdee.top

Py:   f"{3.14159:.2f}"
来源：http://byb.fzhhl.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dcs.aizwys.cn

JS:   (3.14159).toFixed(2)
来源：http://mrc.hcnkem.com

TS:   (3.14159).toFixed(2)
来源：http://xez.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://utu.zhongyouzk.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ila.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://htd.yj202588.top

C#:   3.14159.ToString("F2")
来源：http://jmq.shanyushiyangkeji.top

[A22] 获取字符串长度
来源：http://ukh.jqgfzy.top

Py:   len(s)
来源：http://yjv.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://flv.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qez.ppjwa.cn

TS:   s.length
来源：http://jep.hcnkem.com

Java: s.length()
来源：http://qsn.mhx1999.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nca.yongpay.top

Ruby: s.length
来源：http://wht.yj20258.top

C#:   s.Length
来源：http://ffw.pengpengdd.cyou

[A23] 大小写转换
来源：http://xnn.zhiwuduotai.top

Py:   s.upper(); s.lower(); s.title()
来源：http://yuj.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://req.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mjw.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://szd.c1oappe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gpm.shanyushiyangtech.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wzj.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nda.yuxming.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eae.birdmap.top

[A24] 去除首尾空白
来源：http://gor.chenlongwang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jyo.shanyushiyangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gbm.redwolf501.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tfg.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://buq.hammf.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tzn.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://ysg.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aiz.zhiwuduotai.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dje.ydjk.org.cn

[A25] 字符串比较
来源：http://iow.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://qyf.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tdl.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lvq.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://idf.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qvf.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kmp.hongshengwenyu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kli.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jjg.xuanzx.com

[A26] 类型转换总览
来源：http://pms.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xja.fengsongda.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cyq.hywenlv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xrl.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://gbh.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://var.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dzp.jianghu66.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mdx.shangyingyoupin.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lcx.shanyushiyangkeji.top

================================================================================
来源：http://qip.jyoumei.cn

B. 流程控制
来源：http://kry.quarkkingdee.top

================================================================================
来源：http://kco.sufxvd.cn

[B01] 条件判断 if / else
来源：http://bqg.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ucj.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tkp.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gyv.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ick.ivvv.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zkd.sysykeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xxy.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qup.guowangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tuk.yuxming.cn

[B02] 多分支 else if / elif
来源：http://qxn.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ioy.cheryme.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zzw.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kiv.yj20258888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fmu.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgl.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cdn.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rel.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ohm.fanxiaobao.xyz

[B03] switch / match / case
来源：http://fjd.ivvv.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gzg.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ugz.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jgi.ydzc1.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://azv.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gjx.dianchejie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ivi.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yve.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sid.feifeiyinyue.top

[B04] for 计数循环
来源：http://vnl.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://tyv.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rry.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dyy.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jms.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fzn.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ras.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://khi.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mgv.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://olf.bjfxy.top

Py:   for item in arr: print(item)
来源：http://yau.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bep.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dan.9152youxi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://chp.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yyj.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uyk.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://kiw.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://voo.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://vfh.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wdc.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://csc.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hca.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uht.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zvs.ivvv.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xiy.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pxw.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wab.meibo888.top

[B07] while 循环
来源：http://won.vehdjk.com

Py:   while i < 10: i += 1
来源：http://ncr.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://oal.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://wsv.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://mxx.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://seo.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rpx.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://tmh.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://btq.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://fms.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://ppm.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zzh.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://hgo.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://fwt.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://kjc.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://qtt.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://bzl.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://vgh.bbcook.cn

[B09] break 与 continue
来源：http://ejf.yj20258.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://owr.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tac.zhijiandao.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cmh.yangfankeji.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://guy.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rru.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bdt.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ofn.cqqwz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bcp.yfazqb.com

[B10] 遍历同时拿索引
来源：http://qwg.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hqc.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://azh.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://umy.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mhy.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://brf.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xhk.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uiu.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://umy.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://dga.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://vth.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://idi.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://stz.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nhw.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lfp.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wme.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://bng.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hyz.kuanghao11.cn

[B12] 跳出多层循环
来源：http://oxt.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wlz.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qbq.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yvj.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ihv.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://thr.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://svj.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qky.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://byh.cucudq.cn

[B13] 判断是否为数字
来源：http://bhk.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://dcn.zdbjq.cn

PHP:  is_numeric($x)
来源：http://xbe.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tlt.yuxming.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eof.ydjk.org.cn

Java: x instanceof Number
来源：http://pvv.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tye.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://ult.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://crr.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://hci.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ibb.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yka.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://lac.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://jkt.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dxk.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zpb.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://rzq.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xwu.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://wbn.jqgufenzy.top

Py:   a and b or not c
来源：http://gnx.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://oks.iojbl.cn

JS:   a && b || !c
来源：http://wrq.gotoacloud.top

TS:   a && b || !c
来源：http://tny.daxiang520.top

Java: a && b || !c
来源：http://zen.jyoumei.cn

Go:   a && b || !c
来源：http://rss.ehwqpu.com

Ruby: a && b || !c
来源：http://fxd.hysaishi.cn

C#:   a && b || !c
来源：http://mze.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gen.zhengqikj.top

Py:   if not data: return
来源：http://vph.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://zhk.zhoulong.xyz

JS:   if (!data) return;
来源：http://wnn.shuidangran.top

TS:   if (!data) return;
来源：http://mop.aibaodan.cn

Java: if (data == null) return;
来源：http://ezu.quarkkingdee.top

Go:   if data == nil { return }
来源：http://ito.sysykeji.top

Ruby: return if data.nil?
来源：http://hwv.chenlongwang.top

C#:   if (data == null) return;
来源：http://skj.pycfn.com

================================================================================
来源：http://opc.shanyushiyangtech.top

C. 函数与作用域
来源：http://yth.iojbl.cn

================================================================================
来源：http://xqc.shangyingyoupin.top

[C01] 定义函数
来源：http://feg.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://xkv.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://veg.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://rhv.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bhc.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ozc.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://bxj.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://yei.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uvw.tianlin.xyz

[C02] 默认参数
来源：http://deg.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://qwd.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tqi.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://fxp.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ltd.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://soi.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kfk.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://djo.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://ryf.vehdjk.com

[C03] 可变参数
来源：http://kdp.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://uqt.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hlc.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://puq.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mwj.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xqq.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mlp.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lxc.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zkr.hongshengwenyu.top

[C04] 命名参数 / 关键字参数
来源：http://zzq.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ioy.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hah.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aiq.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rvc.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://sim.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://bwg.jiagoushi.top

Ruby: f(a: 1, b: 2)
来源：http://ejl.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://afz.jiagoushi.top

[C05] 返回多个值
来源：http://cyx.smart0.xyz

Py:   return a, b
来源：http://jef.yonumen.top

PHP:  return [$a, $b];
来源：http://ovx.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jfb.kuanghao11.cn

TS:   return { a, b };
来源：http://huc.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qcd.tanke756.top

Go:   return a, b
来源：http://nab.jqgufenzy.top

Ruby: return a, b
来源：http://guh.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://lsv.jianghu66.top

[C06] 匿名函数 / lambda
来源：http://geg.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://rll.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://srq.sysykeji.top

JS:   const square = x => x * x;
来源：http://cfd.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://ccy.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dlq.jlsjyb.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vjv.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://ddy.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://vny.havefunace.top

[C07] 把函数作为参数传入
来源：http://oaq.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ltq.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://txx.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bvu.cheryme.top

TS:   arr.map(String)
来源：http://yze.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vyp.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://seo.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://yms.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wuw.jqgfzy.top

[C08] 闭包
来源：http://fvi.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ztd.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wad.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://czl.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vcm.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kel.cdnleiting.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lmw.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://toy.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mne.shanyushiyangkeji.top

[C09] 递归
来源：http://ptm.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jkp.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nac.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gcn.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ues.jyoumei.cn


<!-- 参考信息 -->