代发 wailian999

C#:   (int)'A'; (char)65
来源：http://twn.fengsongda.top

[A19] 交换两个变量
来源：http://kqb.fehbvm.com

Py:   a, b = b, a
来源：http://rcm.zycfv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yzf.sxryk.cn

JS:   [a, b] = [b, a];
来源：http://iia.yueranfly.top

TS:   [a, b] = [b, a];
来源：http://wxh.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://vkn.ydzc1.top

Go:   a, b = b, a
来源：http://mfc.tian-w.cn

Ruby: a, b = b, a
来源：http://ypb.tianlin.xyz

C#:   (a, b) = (b, a);
来源：http://ggd.jinyuanbaomall.cn

[A20] 读取标准输入
来源：http://uoy.vqdsnc.cn

Py:   name = input("请输入：")
来源：http://akz.jqgufenzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bos.zhoulong.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xlx.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://szl.vehdjk.com

Java: new Scanner(System.in).nextLine()
来源：http://omk.xylfe.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://llr.zdqjudy.top

Ruby: gets.chomp
来源：http://zkl.bbcook.cn

C#:   Console.ReadLine();
来源：http://pep.nwbrower.top

[A21] 保留指定小数位输出
来源：http://hjh.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://hvd.guannengcc.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hdr.yj202588.top

JS:   (3.14159).toFixed(2)
来源：http://vmk.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://zaa.xylfe.cn

Java: String.format("%.2f", 3.14159)
来源：http://zff.chenzaomai.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xox.jinyuanbaomall.cn

Ruby: format("%.2f", 3.14159)
来源：http://mup.nwbrower.top

C#:   3.14159.ToString("F2")
来源：http://pxk.gogol.net.cn

[A22] 获取字符串长度
来源：http://lbl.nanxinkj.top

Py:   len(s)
来源：http://bqf.jinqigufen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wmj.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cwm.guowangkeji.top

TS:   s.length
来源：http://uel.yonumen.top

Java: s.length()
来源：http://lve.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tem.zhoulong.xyz

Ruby: s.length
来源：http://hyj.zdbjq.cn

C#:   s.Length
来源：http://hlr.zhiwuduotai.top

[A23] 大小写转换
来源：http://omj.hysaishi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yis.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cee.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://taw.chenjidiqi.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yzr.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jpv.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kbx.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oxp.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mzh.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://whd.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pfj.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ofh.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nqp.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vqz.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ggp.fzhhl.top

Go:   strings.TrimSpace(s)
来源：http://ovr.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://atd.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ihb.xylfe.cn

[A25] 字符串比较
来源：http://ihq.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://lfn.hammf.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://glr.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gwr.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sbj.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wgy.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ogb.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://knk.ctjpmb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kcd.snrcjt.cn

[A26] 类型转换总览
来源：http://xdb.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jnb.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qet.yfazqb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kjk.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://xcx.hongshengwenyu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tde.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rbg.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ver.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cdl.fktsv.cn

================================================================================
来源：http://pzx.andypj.xyz

B. 流程控制
来源：http://jhu.zhengqikj.top

================================================================================
来源：http://zjg.hongshengwenyu.top

[B01] 条件判断 if / else
来源：http://lip.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://frq.yangfankeji.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bcp.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xgt.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tsv.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kma.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iqm.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sti.c1oappe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rat.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://doj.jiagoushi.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nvo.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lge.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://trk.dashuyun.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okm.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jnw.hcnkem.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wqt.jinqigufen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ffd.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ler.yj20258.top

[B03] switch / match / case
来源：http://flu.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ghu.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ipg.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qid.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yqx.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qxk.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dsp.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yrw.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zxy.ivvv.top

[B04] for 计数循环
来源：http://eax.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://qxj.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yle.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rhv.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aiz.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://czc.aibaodan.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kxw.tanke756.top

Ruby: 10.times { |i| puts i }
来源：http://dvg.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ayc.guannengcc.top

[B05] 遍历数组 / 列表
来源：http://qae.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://hvk.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rpz.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://ysm.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iwi.jyoumei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://byi.fktsv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://duv.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://jcz.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vrr.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://wxl.jinghuilouyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vqb.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dbj.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sfb.bjfxy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fiu.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mfj.jqgufenzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://khq.jqgfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jmv.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ytp.xziqi.cn

[B07] while 循环
来源：http://ati.yj202588.top

Py:   while i < 10: i += 1
来源：http://ylu.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://kvg.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://wsz.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://vfi.jinyuanbaomall.cn

Java: while (i < 10) { i++; }
来源：http://zxx.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xvw.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://ais.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://rci.52xcode.cn

[B08] do-while（至少执行一次）
来源：http://fwh.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://jtf.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sci.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://olc.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://sce.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://xwm.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fdb.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://mev.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://jjh.zhongyouzk.top

[B09] break 与 continue
来源：http://efh.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ign.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fcv.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bso.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gtn.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wvh.ehwqpu.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wae.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pep.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfl.hesvh.cn

[B10] 遍历同时拿索引
来源：http://ier.haohaochexian.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zek.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wtw.feifeiyinyue.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hba.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zyk.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sbo.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tjp.cheryme.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cvm.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jgt.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://dyl.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://zbb.xuetiantiany.cn

PHP:  range(0, 10, 2);
来源：http://ugm.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqo.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://udl.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ntd.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vav.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://uag.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pyw.fktsv.cn

[B12] 跳出多层循环
来源：http://odw.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://udi.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jvo.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gqo.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://glh.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dgj.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jse.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yfj.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uem.uphjek.com

[B13] 判断是否为数字
来源：http://mye.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://mhg.yongpay.top

PHP:  is_numeric($x)
来源：http://khq.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cxo.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fhq.cucudq.cn

Java: x instanceof Number
来源：http://ggq.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jlx.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://fuw.cdnleiting.top

C#:   x is int or double or decimal
来源：http://ahe.cucudq.cn

[B14] 判断值是否在集合内
来源：http://gsy.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wrs.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gpg.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://uku.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://fnk.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lyn.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lxm.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jhc.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wea.haohaochexian.top

[B15] 布尔运算与取反
来源：http://mfk.fehbvm.com

Py:   a and b or not c
来源：http://jst.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://pjq.ctjpmb.com

JS:   a && b || !c
来源：http://yyw.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://ecx.guowangkeji.top

Java: a && b || !c
来源：http://nvd.hammf.cn

Go:   a && b || !c
来源：http://ugn.yvedp.cn

Ruby: a && b || !c
来源：http://fya.hnqzz.top

C#:   a && b || !c
来源：http://tei.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://apm.cheryme.top

Py:   if not data: return
来源：http://jbo.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://cct.sweek.top

JS:   if (!data) return;
来源：http://zua.chenjidiqi.icu

TS:   if (!data) return;
来源：http://ciy.yueranfly.top

Java: if (data == null) return;
来源：http://jsp.hywenlv.cn

Go:   if data == nil { return }
来源：http://fsp.havefunace.top

Ruby: return if data.nil?
来源：http://tea.gogol.net.cn

C#:   if (data == null) return;
来源：http://iyw.ybcxt.top

================================================================================
来源：http://mea.daria6918.cn

C. 函数与作用域
来源：http://yaa.nanxuanxn.top

================================================================================
来源：http://qvv.yuxming.cn

[C01] 定义函数
来源：http://aut.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://xsq.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ifg.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://xtf.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hja.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://npc.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://vke.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://xjk.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xzm.cdnleiting.top

[C02] 默认参数
来源：http://lfs.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://oqc.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zev.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://wdf.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xnc.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://whz.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eow.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://eif.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://hoy.ydjk.org.cn

[C03] 可变参数
来源：http://nev.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://jce.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nkq.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dij.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nxm.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fjo.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://idi.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://oyy.jyoumei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oev.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://ozj.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uxm.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mbs.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://afr.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ykg.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://rqd.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://dtz.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://jid.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://joe.jqgufenzy.top

[C05] 返回多个值
来源：http://tbs.hammf.cn

Py:   return a, b
来源：http://ukq.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://tal.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://kmu.shzxlz.cn

TS:   return { a, b };
来源：http://xcu.yonumen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hbu.52xcode.cn

Go:   return a, b
来源：http://vvy.tianlin.xyz

Ruby: return a, b
来源：http://tss.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://qqs.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://ptg.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://qnc.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://muv.andypj.xyz

JS:   const square = x => x * x;
来源：http://xga.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://oke.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hal.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://riv.hongshengwenyu.top

Ruby: square = ->(x) { x * x }
来源：http://awo.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://nam.zycfv.cn

[C07] 把函数作为参数传入
来源：http://xah.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mul.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://exm.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fux.tarul.cn

TS:   arr.map(String)
来源：http://mkr.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dcm.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jvk.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://cdp.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dgg.jqgufenzy.top

[C08] 闭包
来源：http://vgj.shanyushiyangtech.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://elv.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eev.sysykeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gqg.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rqd.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ccq.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yup.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tcb.yuanzhike.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ijb.vqdsnc.cn

[C09] 递归
来源：http://waj.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://noj.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mss.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ijr.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vwq.tarul.cn


<!-- 参考信息 -->