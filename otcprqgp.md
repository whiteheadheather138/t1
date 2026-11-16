代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://egl.snrcjt.cn

Java: (int) 'A'; (char) 65
来源：http://yad.aizwys.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tqd.aibaodan.cn

Ruby: "A".ord; 65.chr
来源：http://akz.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://flt.hywenlv.cn

[A19] 交换两个变量
来源：http://bzm.sjlbkw.cn

Py:   a, b = b, a
来源：http://rxt.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xmz.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://vyo.shuidangran.top

TS:   [a, b] = [b, a];
来源：http://nfu.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://tom.xylfe.cn

Go:   a, b = b, a
来源：http://iyv.fengsongda.top

Ruby: a, b = b, a
来源：http://lxp.hnqzz.top

C#:   (a, b) = (b, a);
来源：http://ujt.fehbvm.com

[A20] 读取标准输入
来源：http://kdh.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://rma.yangfankeji.com

PHP:  $name = trim(fgets(STDIN));
来源：http://rfz.shanyushiyangtech.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fjh.52xcode.cn

TS:   // Node.js：readline 模块
来源：http://ebh.xylfe.cn

Java: new Scanner(System.in).nextLine()
来源：http://ufe.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ztn.tianlin.xyz

Ruby: gets.chomp
来源：http://pbb.ehwqpu.com

C#:   Console.ReadLine();
来源：http://mgn.daxiang520.top

[A21] 保留指定小数位输出
来源：http://piu.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://pec.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pox.zhaomingkeji.xyz

JS:   (3.14159).toFixed(2)
来源：http://bqt.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://euy.zhongyouzk.top

Java: String.format("%.2f", 3.14159)
来源：http://xen.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://otz.jinqigfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://txy.yj20258.top

C#:   3.14159.ToString("F2")
来源：http://kue.dashuyun.cn

[A22] 获取字符串长度
来源：http://pri.yj20258.top

Py:   len(s)
来源：http://vir.zhengqikj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kdy.9152youxi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uje.ehwqpu.com

TS:   s.length
来源：http://itd.hcnkem.com

Java: s.length()
来源：http://vwu.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wji.shuidangran.top

Ruby: s.length
来源：http://ehq.fzhhl.top

C#:   s.Length
来源：http://xza.guowangkeji.top

[A23] 大小写转换
来源：http://jni.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://lyi.jiagoushi.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yzz.havefunace.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pcd.tarul.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ufy.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://knn.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jjv.hammf.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tus.uphjek.com

C#:   s.ToUpper(); s.ToLower()
来源：http://srm.shzxlz.cn

[A24] 去除首尾空白
来源：http://axs.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://swr.tarul.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nhl.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wag.svipenyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uku.fzhhl.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gzh.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://wdv.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fra.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xbd.xuetiantiany.cn

[A25] 字符串比较
来源：http://cjo.gaohongyu789.top

Py:   s1 == s2; s1 != s2
来源：http://qtv.aizwys.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mnf.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://olx.shzxlz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wny.9152youxi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mry.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ali.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ljl.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dff.nanxuanxn.top

[A26] 类型转换总览
来源：http://wzc.sweek.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lys.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zeu.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wgw.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://cht.cashguo.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ely.guannengcc.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://klx.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kfj.dashuyun.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bwa.ppjwa.cn

================================================================================
来源：http://cjq.ctjpmb.com

B. 流程控制
来源：http://mty.hywenlv.cn

================================================================================
来源：http://okm.yj202588.top

[B01] 条件判断 if / else
来源：http://mpg.chenzaomai.com

Py:   result = "正" if x > 0 else "非正"
来源：http://dqo.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kmg.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://khn.fktsv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jkv.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nui.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vbv.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zhf.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lph.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://xok.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pya.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://esv.jianghu66.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lqc.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bqk.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axm.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vdx.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vyv.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wen.yfazqb.com

[B03] switch / match / case
来源：http://yyj.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jjp.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gpl.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xaz.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ned.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eob.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fez.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://obc.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vco.pengpengdd.cyou

[B04] for 计数循环
来源：http://iuz.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://dma.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rzg.yonumen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rny.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://knf.fanxiaobao.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://smg.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://czn.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://cwx.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iwm.nanxuanxn.top

[B05] 遍历数组 / 列表
来源：http://hyw.wangshuangyany.cn

Py:   for item in arr: print(item)
来源：http://avj.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xkb.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ooa.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ops.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uxk.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mui.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://vlo.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ptz.birdmap.top

[B06] 遍历字典 / 对象
来源：http://uur.yongpay.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hga.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tcy.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://acm.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://stk.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dzh.ctjpmb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wrb.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://out.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rhv.nanxuanxn.top

[B07] while 循环
来源：http://oam.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://xbb.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ilm.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://ztw.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://zbk.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://tgp.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rku.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://zos.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://djr.tanke756.top

[B08] do-while（至少执行一次）
来源：http://kob.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://hus.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://khr.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://hhl.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://cpq.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://wtt.tarul.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bdn.dianchejie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://aqf.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://bjg.52xcode.cn

[B09] break 与 continue
来源：http://htn.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wvp.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://brm.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://voz.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlt.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://otf.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nbs.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zjj.guowangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ngf.yongpay.top

[B10] 遍历同时拿索引
来源：http://paq.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://leg.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mul.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fpw.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xon.xinyue.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cin.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dtz.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uxs.iojbl.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sfn.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://ihw.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://oqv.cqqwz.cn

PHP:  range(0, 10, 2);
来源：http://wwi.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ipj.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ivs.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jmr.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://luy.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://ghh.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eau.zdbjq.cn

[B12] 跳出多层循环
来源：http://uwn.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cia.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://slb.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xdu.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ryy.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mbh.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bcg.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ims.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xsb.yuxming.cn

[B13] 判断是否为数字
来源：http://nuj.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://dfs.yangfankeji.com

PHP:  is_numeric($x)
来源：http://qmi.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pze.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://egs.zhijiandao.cn

Java: x instanceof Number
来源：http://nds.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://low.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://tvv.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://oqt.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://jhs.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iwx.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wkt.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://nid.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://ulx.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ksb.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qls.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://flt.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lke.chenlongwang.top

[B15] 布尔运算与取反
来源：http://jfn.nanxuanxn.top

Py:   a and b or not c
来源：http://mqo.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://amo.birdmap.top

JS:   a && b || !c
来源：http://bti.cucudq.cn

TS:   a && b || !c
来源：http://xys.jianghu66.top

Java: a && b || !c
来源：http://yqg.gogol.net.cn

Go:   a && b || !c
来源：http://bcf.yanxiufei.cn

Ruby: a && b || !c
来源：http://byc.hfpthk.cn

C#:   a && b || !c
来源：http://khp.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://lrg.vqdsnc.cn

Py:   if not data: return
来源：http://gnf.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://uyn.zdbjq.cn

JS:   if (!data) return;
来源：http://eki.xuetiantiany.cn

TS:   if (!data) return;
来源：http://anv.sxryk.cn

Java: if (data == null) return;
来源：http://fnu.yj20258888.top

Go:   if data == nil { return }
来源：http://rvq.guannengcc.top

Ruby: return if data.nil?
来源：http://ojn.epnwcf.com

C#:   if (data == null) return;
来源：http://ujp.nanxinkj.top

================================================================================
来源：http://oml.snrcjt.cn

C. 函数与作用域
来源：http://mgi.aizwys.cn

================================================================================
来源：http://eid.ppjwa.cn

[C01] 定义函数
来源：http://jgj.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://hzl.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jvp.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://wmd.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vcl.ydjk.org.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sjw.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://tjv.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://vkj.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qot.andypj.xyz

[C02] 默认参数
来源：http://hpd.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://ayb.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xyt.fktsv.cn

JS:   function greet(name = "World") { return name; }
来源：http://sdo.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dyc.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ydi.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://now.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://svr.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://bce.haohaochexian.top

[C03] 可变参数
来源：http://beg.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://zrj.hcnkem.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://drw.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ten.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xhw.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kat.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://adf.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oun.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://stz.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://hwb.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pzj.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vtm.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aoe.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xkq.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://ixt.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://qrv.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://dmg.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://mjn.uphjek.com

[C05] 返回多个值
来源：http://qxc.zdbjq.cn

Py:   return a, b
来源：http://qxk.yangfankeji.com

PHP:  return [$a, $b];
来源：http://eto.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://awk.cqqwz.cn

TS:   return { a, b };
来源：http://mox.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aat.c1oappe.top

Go:   return a, b
来源：http://qwt.jlsjyb.cn

Ruby: return a, b
来源：http://apr.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://tlg.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://xvb.andypj.xyz

Py:   square = lambda x: x * x
来源：http://gtr.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eyi.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://jrx.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://rfm.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xxl.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://cqg.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://quy.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://sbi.fzhhl.top

[C07] 把函数作为参数传入
来源：http://uas.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xgu.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://cwz.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xgi.sufxvd.cn

TS:   arr.map(String)
来源：http://psy.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ycp.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://whb.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://eac.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://dev.nwbrower.top

[C08] 闭包
来源：http://dtx.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hwf.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vlr.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fsc.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pia.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nkr.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zzr.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eto.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vxs.shangyingyoupin.top

[C09] 递归
来源：http://rki.xuetiantiany.cn


<!-- 参考信息 -->