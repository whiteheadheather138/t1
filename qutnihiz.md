代发 wailian999

C#:   (int)'A'; (char)65
来源：http://hvv.gotoacloud.top

[A19] 交换两个变量
来源：http://kjj.daxiang520.top

Py:   a, b = b, a
来源：http://xjv.hnqzz.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hfb.cucudq.cn

JS:   [a, b] = [b, a];
来源：http://zow.sysykeji.top

TS:   [a, b] = [b, a];
来源：http://bws.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://nbw.hcnkem.com

Go:   a, b = b, a
来源：http://oex.zdbjq.cn

Ruby: a, b = b, a
来源：http://xlh.meibo888.top

C#:   (a, b) = (b, a);
来源：http://dfr.tian-w.cn

[A20] 读取标准输入
来源：http://zqq.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://wdl.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vjb.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wjx.fanxiaobao.xyz

TS:   // Node.js：readline 模块
来源：http://nee.zycfv.cn

Java: new Scanner(System.in).nextLine()
来源：http://zmd.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sjt.pengpengdd.cyou

Ruby: gets.chomp
来源：http://adk.hongshengwenyu.top

C#:   Console.ReadLine();
来源：http://woi.redwolf501.top

[A21] 保留指定小数位输出
来源：http://paz.jiagoushi.top

Py:   f"{3.14159:.2f}"
来源：http://ttv.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fqp.yvedp.cn

JS:   (3.14159).toFixed(2)
来源：http://qam.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://blt.tian-w.cn

Java: String.format("%.2f", 3.14159)
来源：http://rpk.xziqi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://efp.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://ixa.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://zck.shzxlz.cn

[A22] 获取字符串长度
来源：http://cxb.jinqigfzy.top

Py:   len(s)
来源：http://veu.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://six.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sic.yuxming.cn

TS:   s.length
来源：http://jik.zdqjudy.top

Java: s.length()
来源：http://geh.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://udp.birdmap.top

Ruby: s.length
来源：http://eop.bjfxy.top

C#:   s.Length
来源：http://koh.c1oappe.top

[A23] 大小写转换
来源：http://oqn.hywenlv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vkk.snrcjt.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://acw.andypj.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eka.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hic.wangdashe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://weh.kuanghao11.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hkv.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mqt.gogol.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://msw.uphjek.com

[A24] 去除首尾空白
来源：http://qsz.sufxvd.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ovm.ivvv.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ont.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sxe.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ydg.tarul.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gia.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://zsj.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tlk.wangshuangyany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kmq.xuetiantiany.cn

[A25] 字符串比较
来源：http://gqm.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://kwg.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fyi.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nuy.snrcjt.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qqv.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jwj.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nep.smart0.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://hna.nanxinkj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qfb.cheryme.top

[A26] 类型转换总览
来源：http://kpd.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lih.cdnleiting.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uxr.gaohongyu789.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mgk.gogol.net.cn

TS:   Number() String() Boolean() x as number
来源：http://tqo.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mzy.havefunace.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wrg.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jeu.hnqzz.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fok.aizwys.cn

================================================================================
来源：http://kvc.sysykeji.top

B. 流程控制
来源：http://end.iojbl.cn

================================================================================
来源：http://eob.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://umd.sxryk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fhq.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uhy.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fre.hywenlv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dvr.smart0.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://pul.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vet.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vbq.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://swp.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://byi.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mfq.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jxp.guowangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qwp.dianchejie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qdw.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndc.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zmv.jinqigufen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ght.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ako.guannengcc.top

[B03] switch / match / case
来源：http://iin.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dyy.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ksc.hcnkem.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gvu.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ukc.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://urf.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ime.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gzh.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://exo.epnwcf.com

[B04] for 计数循环
来源：http://vad.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://ken.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://snu.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rlz.sweek.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://psr.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uqw.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zed.hywenlv.cn

Ruby: 10.times { |i| puts i }
来源：http://gqm.yvedp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://etx.hammf.cn

[B05] 遍历数组 / 列表
来源：http://txj.jqgfzy.top

Py:   for item in arr: print(item)
来源：http://zkq.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kcz.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vff.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cka.tianlin.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://npl.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://spw.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://vlv.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dug.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://jby.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qxz.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://due.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vjh.feifeiyinyue.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tjz.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fcj.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://efr.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://imr.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cgg.zycfv.cn

[B07] while 循环
来源：http://kxn.iojbl.cn

Py:   while i < 10: i += 1
来源：http://tte.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tje.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://kvi.redwolf501.top

TS:   while (i < 10) { i++; }
来源：http://ixv.zhiwuduotai.top

Java: while (i < 10) { i++; }
来源：http://lon.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ktp.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://iut.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://lpu.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://eml.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://ros.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kab.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://ant.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://igs.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://iij.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xmj.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://hsc.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://mos.hfpthk.cn

[B09] break 与 continue
来源：http://phf.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zgk.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ngn.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dte.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ick.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wjh.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lsr.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://osd.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dwa.cashguo.top

[B10] 遍历同时拿索引
来源：http://ftv.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cqr.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tiz.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vaa.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vzy.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eap.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ize.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aaj.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zsj.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://tdr.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://zxj.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://owq.yfazqb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vfe.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fui.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pau.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cxi.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://nxh.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ulc.hesvh.cn

[B12] 跳出多层循环
来源：http://ghp.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ygc.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://yvv.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sqb.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mhf.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lhg.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qne.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kkf.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cri.zhoulong.xyz

[B13] 判断是否为数字
来源：http://wnh.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://brz.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://tfi.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zgx.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vcr.chenzaomai.com

Java: x instanceof Number
来源：http://ivc.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bhv.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://qbg.aizwys.cn

C#:   x is int or double or decimal
来源：http://zba.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://sju.jianghu66.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://agq.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oqa.0kj1m.cn

JS:   [1, 2, 3].includes(x)
来源：http://hwd.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ftn.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://lar.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qlp.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://kxg.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mih.yj202588.top

[B15] 布尔运算与取反
来源：http://tcc.yuanzhike.top

Py:   a and b or not c
来源：http://css.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://qzp.pengpengdd.cyou

JS:   a && b || !c
来源：http://lzd.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://qka.yj20258.top

Java: a && b || !c
来源：http://wje.jinghuilouyu.cn

Go:   a && b || !c
来源：http://yhu.hesvh.cn

Ruby: a && b || !c
来源：http://grt.sufxvd.cn

C#:   a && b || !c
来源：http://huw.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qhf.zhiwuduotai.top

Py:   if not data: return
来源：http://pmo.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://azd.hnqzz.top

JS:   if (!data) return;
来源：http://hse.cheryme.top

TS:   if (!data) return;
来源：http://wkk.zhoulong.xyz

Java: if (data == null) return;
来源：http://kdo.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://bek.shzxlz.cn

Ruby: return if data.nil?
来源：http://yrn.zhijiandao.cn

C#:   if (data == null) return;
来源：http://ryo.chenlongwang.top

================================================================================
来源：http://twx.yvedp.cn

C. 函数与作用域
来源：http://whf.sweek.top

================================================================================
来源：http://nil.uphjek.com

[C01] 定义函数
来源：http://lga.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://kcm.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bqr.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://tfs.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://idc.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vks.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://ick.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://lro.wangdashe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pnt.zdbjq.cn

[C02] 默认参数
来源：http://exu.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://tfz.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://sjt.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://ydm.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pru.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://oik.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tss.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://eeq.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://cnn.ywan-chungtsiang.top

[C03] 可变参数
来源：http://ulx.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://ewd.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wmd.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dql.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xwy.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wbr.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cmo.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://lpq.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zhp.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://kyi.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cfs.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wwt.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ebs.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zvi.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://svd.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://rhl.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://ycx.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://mnc.nanxinkj.top

[C05] 返回多个值
来源：http://auu.jinghuilouyu.cn

Py:   return a, b
来源：http://pli.hammf.cn

PHP:  return [$a, $b];
来源：http://sdu.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rfw.yj202588.top

TS:   return { a, b };
来源：http://nhv.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ijy.hammf.cn

Go:   return a, b
来源：http://wjf.iojbl.cn

Ruby: return a, b
来源：http://djz.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://eyv.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://cut.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://wks.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vmh.shuidangran.top

JS:   const square = x => x * x;
来源：http://xyl.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://mqz.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ajq.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kld.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://eoj.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://wfg.redwolf501.top

[C07] 把函数作为参数传入
来源：http://dzz.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://utx.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://tcb.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wfn.ppjwa.cn

TS:   arr.map(String)
来源：http://atu.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nwb.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dgv.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://tsc.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rjm.fktsv.cn

[C08] 闭包
来源：http://lbi.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sdw.daria6918.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vvm.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ykz.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vnq.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://san.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ami.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zkq.uphjek.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xvt.kuanghao11.cn

[C09] 递归
来源：http://foo.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mjn.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://msl.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yci.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sup.ydzc1.top


<!-- 参考信息 -->