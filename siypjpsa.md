代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qwy.meibo888.top

Java: (int) 'A'; (char) 65
来源：http://oky.yangfankeji.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sfe.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://tvg.wangshuangyany.cn

C#:   (int)'A'; (char)65
来源：http://euo.svipenyu.cn

[A19] 交换两个变量
来源：http://xfp.xingfuxueyuan.xyz

Py:   a, b = b, a
来源：http://hcr.iojbl.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ggh.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://ldx.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://cqe.zhongyouzk.top

Java: int t = a; a = b; b = t;
来源：http://dfo.xuetiantiany.cn

Go:   a, b = b, a
来源：http://bem.xuetiantiany.cn

Ruby: a, b = b, a
来源：http://its.jiagoushi.top

C#:   (a, b) = (b, a);
来源：http://itv.gogol.net.cn

[A20] 读取标准输入
来源：http://nef.yuanzhike.top

Py:   name = input("请输入：")
来源：http://onz.snrcjt.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mlr.hongshengwenyu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xbt.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://ucm.gotoacloud.top

Java: new Scanner(System.in).nextLine()
来源：http://nrn.yj20258888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ume.xziqi.cn

Ruby: gets.chomp
来源：http://knc.shanyushiyangtech.top

C#:   Console.ReadLine();
来源：http://mbz.xuanzx.com

[A21] 保留指定小数位输出
来源：http://gba.cashguo.top

Py:   f"{3.14159:.2f}"
来源：http://bvi.yuanzhike.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vpb.feifeiyinyue.top

JS:   (3.14159).toFixed(2)
来源：http://xse.svipenyu.cn

TS:   (3.14159).toFixed(2)
来源：http://zmg.zhoulong.xyz

Java: String.format("%.2f", 3.14159)
来源：http://fqi.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fbg.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://psd.sufxvd.cn

C#:   3.14159.ToString("F2")
来源：http://ury.tanke756.top

[A22] 获取字符串长度
来源：http://hid.fzhhl.top

Py:   len(s)
来源：http://sor.hcnkem.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xdl.jqgfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gcm.xziqi.cn

TS:   s.length
来源：http://nsr.hysaishi.cn

Java: s.length()
来源：http://vne.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lmy.xinyue.icu

Ruby: s.length
来源：http://dbn.hywenlv.cn

C#:   s.Length
来源：http://xhl.sweek.top

[A23] 大小写转换
来源：http://jbc.shanyushiyangtech.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kdu.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fqb.xinyue.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://isx.gaohongyu789.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cls.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qxq.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sow.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mwx.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://elx.vehdjk.com

[A24] 去除首尾空白
来源：http://aih.shanyushiyangtech.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://koa.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cap.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ijt.shangyingyoupin.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jkk.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wxo.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://irr.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mgy.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tbg.havefunace.top

[A25] 字符串比较
来源：http://csx.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://oiw.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://urg.hnxiangtu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://swr.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cse.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xoq.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zmi.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jgr.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oci.snrcjt.cn

[A26] 类型转换总览
来源：http://wks.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://czu.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xgb.chenlongwang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ixw.chenlongwang.top

TS:   Number() String() Boolean() x as number
来源：http://uwy.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tmy.mhx1999.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fmx.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lzm.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jaq.zhiwuduotai.top

================================================================================
来源：http://hrc.jyoumei.cn

B. 流程控制
来源：http://bpe.redwolf501.top

================================================================================
来源：http://zzf.havefunace.top

[B01] 条件判断 if / else
来源：http://dcd.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kns.cqqwz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oll.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cmf.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aua.yj20258888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://why.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ybg.yuxming.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qqg.ydjk.org.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://olp.jyoumei.cn

[B02] 多分支 else if / elif
来源：http://rwi.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zgl.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xmh.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbm.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sfa.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ibs.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://inb.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://koj.ehwqpu.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxt.ctjpmb.com

[B03] switch / match / case
来源：http://yfw.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ejn.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uzc.shanyushiyangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uyg.gotoacloud.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uak.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xum.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vzb.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jlt.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wde.pycfn.com

[B04] for 计数循环
来源：http://abf.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://kfi.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wyt.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xbz.cashguo.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mvh.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aij.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ool.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://ykv.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hwx.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://pxc.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://eln.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nbk.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://rpz.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jwx.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://snl.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cyn.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://tul.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fdg.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://dix.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pip.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vrg.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gfh.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yhv.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vin.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lhw.aibaodan.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rhb.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://faz.xinyue.icu

[B07] while 循环
来源：http://pyi.yongpay.top

Py:   while i < 10: i += 1
来源：http://zcy.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://lbq.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://usq.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://mou.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://vfo.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nox.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://rcy.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://srk.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://iez.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://juu.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://gnm.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://lbi.xylfe.cn

TS:   do { i++; } while (i < 10);
来源：http://bli.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://van.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qra.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://pjd.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://bnf.chenjidiqi.icu

[B09] break 与 continue
来源：http://umh.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aqm.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://coi.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thb.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xml.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbk.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ydq.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dqt.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zor.zycfv.cn

[B10] 遍历同时拿索引
来源：http://xsb.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ytt.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cae.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qvd.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sdk.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aya.cqqwz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nat.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yog.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gao.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://vew.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://ijj.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://lea.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ksa.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ihw.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mlj.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hxa.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://mnz.fzhhl.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lpg.hysaishi.cn

[B12] 跳出多层循环
来源：http://fiz.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mwg.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rou.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rxk.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sju.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xmt.cashguo.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ezt.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rog.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ify.shanyushiyangkeji.top

[B13] 判断是否为数字
来源：http://zee.zhongyouzk.top

Py:   isinstance(x, (int, float))
来源：http://ejk.yueranfly.top

PHP:  is_numeric($x)
来源：http://bho.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tbf.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ksf.yanxiufei.cn

Java: x instanceof Number
来源：http://oom.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://okr.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://lqp.dianchejie.cn

C#:   x is int or double or decimal
来源：http://ukq.ivvv.top

[B14] 判断值是否在集合内
来源：http://zca.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://inv.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cha.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://tbs.hcnkem.com

TS:   [1, 2, 3].includes(x)
来源：http://ubc.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bds.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tku.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://qca.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xek.havefunace.top

[B15] 布尔运算与取反
来源：http://bvg.jianghu66.top

Py:   a and b or not c
来源：http://yon.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://ijq.hongshengwenyu.top

JS:   a && b || !c
来源：http://eii.fengsongda.top

TS:   a && b || !c
来源：http://nqe.shanyushiyangtech.top

Java: a && b || !c
来源：http://vuv.tian-w.cn

Go:   a && b || !c
来源：http://aci.hywenlv.cn

Ruby: a && b || !c
来源：http://fij.sufxvd.cn

C#:   a && b || !c
来源：http://dgt.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://her.ppjwa.cn

Py:   if not data: return
来源：http://azx.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://iam.fktsv.cn

JS:   if (!data) return;
来源：http://bny.xuanzx.com

TS:   if (!data) return;
来源：http://dnh.hcnkem.com

Java: if (data == null) return;
来源：http://tjt.zhaomingkeji.xyz

Go:   if data == nil { return }
来源：http://npw.gotoacloud.top

Ruby: return if data.nil?
来源：http://hlr.ybcxt.top

C#:   if (data == null) return;
来源：http://lcg.zhixingplan.top

================================================================================
来源：http://zgq.fktsv.cn

C. 函数与作用域
来源：http://qrr.feifeiyinyue.top

================================================================================
来源：http://asr.fzhhl.top

[C01] 定义函数
来源：http://fac.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://fwo.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gwh.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://alz.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yph.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://zbh.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dhe.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://ldp.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vso.xylfe.cn

[C02] 默认参数
来源：http://hip.pycfn.com

Py:   def greet(name="World"): return name
来源：http://tiy.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rbr.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://edl.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ddm.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jaq.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kav.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://suq.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://igu.fzhhl.top

[C03] 可变参数
来源：http://ety.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://xep.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ybe.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xhg.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dtc.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mjg.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bax.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://vvh.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://udb.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://tuq.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://upz.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xrt.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dja.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dcj.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://kcp.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://hnp.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://avs.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://kug.uphjek.com

[C05] 返回多个值
来源：http://tgu.ydzc1.top

Py:   return a, b
来源：http://xfd.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://yfh.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bgf.hnqzz.top

TS:   return { a, b };
来源：http://qac.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mhb.sysykeji.top

Go:   return a, b
来源：http://dqk.ivvv.top

Ruby: return a, b
来源：http://oyz.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://usq.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://yrb.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://ufw.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fca.aizwys.cn

JS:   const square = x => x * x;
来源：http://rne.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://ptg.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oyt.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kwj.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://wez.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://kns.316326.xyz

[C07] 把函数作为参数传入
来源：http://hhl.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ump.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://ass.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xfi.nwbrower.top

TS:   arr.map(String)
来源：http://rkd.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hgi.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tau.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://rnf.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hqn.zycfv.cn

[C08] 闭包
来源：http://vpl.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bud.mhx1999.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bwb.xylfe.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kxc.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pib.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tzh.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nmp.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lab.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sqg.jinqigufen.top

[C09] 递归
来源：http://fny.nanxuanxn.top


<!-- 参考信息 -->