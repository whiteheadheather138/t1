代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ury.havefunace.top

Java: (int) 'A'; (char) 65
来源：http://iwz.yfazqb.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zwe.chenlongwang.top

Ruby: "A".ord; 65.chr
来源：http://gio.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://kas.iojbl.cn

[A19] 交换两个变量
来源：http://jma.sjlbkw.cn

Py:   a, b = b, a
来源：http://mit.haohaochexian.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mnh.zhoulong.xyz

JS:   [a, b] = [b, a];
来源：http://jun.hnqzz.top

TS:   [a, b] = [b, a];
来源：http://tbz.jinghuilouyu.cn

Java: int t = a; a = b; b = t;
来源：http://ttb.yongpay.top

Go:   a, b = b, a
来源：http://dwh.jqgfzy.top

Ruby: a, b = b, a
来源：http://agz.yonumen.top

C#:   (a, b) = (b, a);
来源：http://ghf.yvedp.cn

[A20] 读取标准输入
来源：http://wqh.zhoulong.xyz

Py:   name = input("请输入：")
来源：http://spm.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tdz.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vld.sxryk.cn

TS:   // Node.js：readline 模块
来源：http://ycu.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://nmt.yj202588.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xxw.gaohongyu789.top

Ruby: gets.chomp
来源：http://cym.316326.xyz

C#:   Console.ReadLine();
来源：http://pcw.zhongyouzk.top

[A21] 保留指定小数位输出
来源：http://iaj.cashguo.top

Py:   f"{3.14159:.2f}"
来源：http://yxd.hongshengwenyu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zaf.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://nwi.hcnkem.com

TS:   (3.14159).toFixed(2)
来源：http://hgt.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://shr.cheryme.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wns.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://pal.aibaodan.cn

C#:   3.14159.ToString("F2")
来源：http://uiv.xziqi.cn

[A22] 获取字符串长度
来源：http://jht.havefunace.top

Py:   len(s)
来源：http://qjr.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cco.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://drv.tarul.cn

TS:   s.length
来源：http://bsc.guannengcc.top

Java: s.length()
来源：http://rsy.guannengcc.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zrp.ctjpmb.com

Ruby: s.length
来源：http://soz.gogol.net.cn

C#:   s.Length
来源：http://nhf.zhongyouzk.top

[A23] 大小写转换
来源：http://vca.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vjz.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cht.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oyx.hfpthk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fid.chenzaomai.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yyi.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jsg.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://anx.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ghe.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://pbw.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cxf.guowangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://emr.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qsd.chenjidiqi.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jik.aibaodan.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dmo.yonumen.top

Go:   strings.TrimSpace(s)
来源：http://gfg.guannengcc.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ddq.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gae.zhoulong.xyz

[A25] 字符串比较
来源：http://qdv.iojbl.cn

Py:   s1 == s2; s1 != s2
来源：http://eyu.cheryme.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bon.sxryk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gwj.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ntm.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vos.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kal.ppjwa.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sok.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kfc.xuetiantiany.cn

[A26] 类型转换总览
来源：http://kgt.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dxi.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rwp.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tpt.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://eqp.hnqzz.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://crm.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mwi.ppjwa.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pia.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://frq.jinqigfzy.top

================================================================================
来源：http://vnt.andypj.xyz

B. 流程控制
来源：http://euk.redwolf501.top

================================================================================
来源：http://ckp.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://qii.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rio.meibo888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tqs.zdbjq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nzj.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ohi.jiagoushi.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wqw.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ucv.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ggm.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ctt.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://qwf.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://phr.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://non.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tef.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xch.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yhz.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yqz.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sgx.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ywu.zhongyouzk.top

[B03] switch / match / case
来源：http://ttu.tanke756.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zqs.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bgs.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jds.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://woc.xziqi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ttm.hnxiangtu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xvt.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ohd.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qsr.yanxiufei.cn

[B04] for 计数循环
来源：http://gsa.fzhhl.top

Py:   for i in range(10): print(i)
来源：http://vud.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://prw.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oxa.yvedp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://elp.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://glh.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yxa.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://dyu.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zrg.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://leq.daria6918.cn

Py:   for item in arr: print(item)
来源：http://fmf.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uex.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zdk.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zxt.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://bxc.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jip.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://egd.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xmb.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://dup.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bdw.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wkq.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lhg.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nsi.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aaj.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ogz.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ico.chenjidiqi.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ufs.redwolf501.top

[B07] while 循环
来源：http://bng.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://pyr.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://lzt.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://ojl.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://zpg.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://rtt.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://udg.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://uua.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://htc.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://ohv.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://kez.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bpn.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://uzc.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://kki.gzhubu.top

Java: do { i++; } while (i < 10);
来源：http://uvy.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gpd.hnxiangtu.top

Ruby: begin; i += 1; end while i < 10
来源：http://mgq.jinyuanbaomall.cn

C#:   do { i++; } while (i < 10);
来源：http://lak.c1oappe.top

[B09] break 与 continue
来源：http://poh.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vst.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qdp.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwh.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gpn.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://roi.chenzaomai.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jvd.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gwc.shanyushiyangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ibp.zycfv.cn

[B10] 遍历同时拿索引
来源：http://iha.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hpx.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hqw.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ijm.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wmj.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ueg.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ukk.cdnleiting.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ggd.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ecm.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://ktf.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://icu.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://kvm.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://voa.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dnv.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ygv.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://guf.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://wcs.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jke.redwolf501.top

[B12] 跳出多层循环
来源：http://vxb.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hoh.wangdashe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://evk.gaohongyu789.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ipz.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ngo.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://skx.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bsw.redwolf501.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://erd.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://njw.yonumen.top

[B13] 判断是否为数字
来源：http://tps.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://rmr.yueranfly.top

PHP:  is_numeric($x)
来源：http://vgg.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jap.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fis.dashuyun.cn

Java: x instanceof Number
来源：http://brs.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://img.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://epn.fzhhl.top

C#:   x is int or double or decimal
来源：http://cox.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://mjm.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mrc.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qlz.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://knt.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://awz.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://llr.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tin.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vmd.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gdj.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://cef.jinqigufen.top

Py:   a and b or not c
来源：http://wde.yonumen.top

PHP:  $a && $b || !$c
来源：http://rbs.316326.xyz

JS:   a && b || !c
来源：http://fnp.fehbvm.com

TS:   a && b || !c
来源：http://bjd.jlsjyb.cn

Java: a && b || !c
来源：http://epv.yuxming.cn

Go:   a && b || !c
来源：http://kee.zhoulong.xyz

Ruby: a && b || !c
来源：http://erg.hammf.cn

C#:   a && b || !c
来源：http://owh.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://dco.meibo888.top

Py:   if not data: return
来源：http://kph.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://jxg.andypj.xyz

JS:   if (!data) return;
来源：http://xnf.guannengcc.top

TS:   if (!data) return;
来源：http://kkc.daria6918.cn

Java: if (data == null) return;
来源：http://eca.hywenlv.cn

Go:   if data == nil { return }
来源：http://qia.zdbjq.cn

Ruby: return if data.nil?
来源：http://dtx.gzhubu.top

C#:   if (data == null) return;
来源：http://qen.vehdjk.com

================================================================================
来源：http://kcq.52xcode.cn

C. 函数与作用域
来源：http://gea.sxryk.cn

================================================================================
来源：http://sir.jlsjyb.cn

[C01] 定义函数
来源：http://yak.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://kkc.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://axo.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://vtt.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ita.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lbv.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://see.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://evd.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://odv.shzxlz.cn

[C02] 默认参数
来源：http://vfd.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://ceb.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ygq.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://nyd.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://red.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pju.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ufq.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://tuy.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://nsf.chenjidiqi.icu

[C03] 可变参数
来源：http://hki.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://oam.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uky.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mhr.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aod.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tse.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hxi.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eqg.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wvo.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://acf.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://efx.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vso.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ynd.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jzk.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://cub.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://fcs.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://wzf.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://wxa.sufxvd.cn

[C05] 返回多个值
来源：http://kew.cdnleiting.top

Py:   return a, b
来源：http://yzr.jianghu66.top

PHP:  return [$a, $b];
来源：http://swn.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://csf.zhijiandao.cn

TS:   return { a, b };
来源：http://ljx.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qgp.smart0.xyz

Go:   return a, b
来源：http://daf.sweek.top

Ruby: return a, b
来源：http://uid.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://tis.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://lsp.guannengcc.top

Py:   square = lambda x: x * x
来源：http://vlq.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://akx.zdqjudy.top

JS:   const square = x => x * x;
来源：http://gpp.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://ser.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nbc.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://ipw.redwolf501.top

Ruby: square = ->(x) { x * x }
来源：http://rel.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fbw.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://qvl.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pve.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://ywc.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ocz.kuanghao11.cn

TS:   arr.map(String)
来源：http://hwu.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://owg.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wxt.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://kyn.smart0.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://dbp.9152youxi.cn

[C08] 闭包
来源：http://uqo.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gtv.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wym.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fih.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kav.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uct.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://clt.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ybp.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://low.shangyingyoupin.top

[C09] 递归
来源：http://gpr.pycfn.com


<!-- 参考信息 -->