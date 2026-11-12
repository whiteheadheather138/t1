代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gvh.guannengcc.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qeb.hongshengwenyu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iar.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://szy.vehdjk.com

[A18] 字符与 ASCII 码互转
来源：http://mse.shanyushiyangtech.top

Py:   ord("A"); chr(65)
来源：http://mrz.jlsjyb.cn

PHP:  ord("A"); chr(65)
来源：http://ayf.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tdf.hammf.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cei.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://frx.dianchejie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qvv.nwbrower.top

Ruby: "A".ord; 65.chr
来源：http://asv.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://ozt.xziqi.cn

[A19] 交换两个变量
来源：http://qkg.redwolf501.top

Py:   a, b = b, a
来源：http://fgh.sxryk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nqn.aibaodan.cn

JS:   [a, b] = [b, a];
来源：http://lqm.xuetiantiany.cn

TS:   [a, b] = [b, a];
来源：http://rui.shangyingyoupin.top

Java: int t = a; a = b; b = t;
来源：http://phi.shzxlz.cn

Go:   a, b = b, a
来源：http://ewg.zhiwuduotai.top

Ruby: a, b = b, a
来源：http://nws.hongshengwenyu.top

C#:   (a, b) = (b, a);
来源：http://egh.hesvh.cn

[A20] 读取标准输入
来源：http://shd.hammf.cn

Py:   name = input("请输入：")
来源：http://cfy.fehbvm.com

PHP:  $name = trim(fgets(STDIN));
来源：http://feq.0kj1m.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qks.gzhubu.top

TS:   // Node.js：readline 模块
来源：http://box.jiagoushi.top

Java: new Scanner(System.in).nextLine()
来源：http://opp.zhaomingkeji.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://djf.ybcxt.top

Ruby: gets.chomp
来源：http://evo.fehbvm.com

C#:   Console.ReadLine();
来源：http://mbd.jinghuilouyu.cn

[A21] 保留指定小数位输出
来源：http://azc.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://kjo.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xpi.gogol.net.cn

JS:   (3.14159).toFixed(2)
来源：http://utd.shuidangran.top

TS:   (3.14159).toFixed(2)
来源：http://hlr.meibo888.top

Java: String.format("%.2f", 3.14159)
来源：http://jvg.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bdu.cheryme.top

Ruby: format("%.2f", 3.14159)
来源：http://obn.bbcook.cn

C#:   3.14159.ToString("F2")
来源：http://nyi.yuanzhike.top

[A22] 获取字符串长度
来源：http://wyc.fktsv.cn

Py:   len(s)
来源：http://ovx.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nke.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zwz.feifeiyinyue.top

TS:   s.length
来源：http://zgr.yonumen.top

Java: s.length()
来源：http://gfu.zdbjq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://shn.zycfv.cn

Ruby: s.length
来源：http://nyu.xuetiantiany.cn

C#:   s.Length
来源：http://iiz.yueranfly.top

[A23] 大小写转换
来源：http://fpo.yangfankeji.com

Py:   s.upper(); s.lower(); s.title()
来源：http://cka.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bkh.hammf.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cyb.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ccs.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ptk.haohaochexian.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dxb.gogol.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vso.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uee.daria6918.cn

[A24] 去除首尾空白
来源：http://abb.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://huw.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fwz.meibo888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zfh.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gjg.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ptx.ydjk.org.cn

Go:   strings.TrimSpace(s)
来源：http://rab.dianchejie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pfr.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qoq.feifeiyinyue.top

[A25] 字符串比较
来源：http://spb.zhijiandao.cn

Py:   s1 == s2; s1 != s2
来源：http://vsd.tanke756.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bxr.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wjk.cucudq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qov.shuidangran.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gav.hnxiangtu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://coa.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dmq.yuxming.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zlv.dashuyun.cn

[A26] 类型转换总览
来源：http://phi.tianlin.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yob.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rgo.hnxiangtu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qdg.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://qvu.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eet.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://knz.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ayq.sjlbkw.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uqn.jinqigfzy.top

================================================================================
来源：http://sny.shanyushiyangkeji.top

B. 流程控制
来源：http://xaj.ybcxt.top

================================================================================
来源：http://dah.smart0.xyz

[B01] 条件判断 if / else
来源：http://cpp.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://evc.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://crf.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tgr.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://chy.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://fho.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://afb.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jex.fehbvm.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mvf.tian-w.cn

[B02] 多分支 else if / elif
来源：http://vmc.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mso.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rgd.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hmu.ydzc1.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lee.zdbjq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vpd.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://esp.0kj1m.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ebl.nanxuanxn.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://snm.yfazqb.com

[B03] switch / match / case
来源：http://qaq.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://czv.iojbl.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qxr.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://imm.fengsongda.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qsr.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iut.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ezc.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ftt.ctjpmb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vuz.fanxiaobao.xyz

[B04] for 计数循环
来源：http://pxn.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://vde.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zun.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qra.xingfuxueyuan.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjf.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ggy.sysykeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kly.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://kvq.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qcw.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://exr.ybcxt.top

Py:   for item in arr: print(item)
来源：http://nte.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kxo.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ryr.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rgg.yongpay.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pon.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ahk.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://evq.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://coq.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://zln.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rih.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dyh.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xwa.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://igl.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://efj.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nin.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hbr.xziqi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kxn.fktsv.cn

[B07] while 循环
来源：http://wvs.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://kmt.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ixs.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://qsi.chenzaomai.com

TS:   while (i < 10) { i++; }
来源：http://zvv.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://swl.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xes.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://nch.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://ufv.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://dxg.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://lqu.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zqd.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://ofo.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://xii.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://fuk.haohaochexian.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fhn.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dok.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://bnx.yanxiufei.cn

[B09] break 与 continue
来源：http://gky.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rsl.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://phr.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pwa.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzf.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggl.xingfuxueyuan.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rmf.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://haw.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eak.yueranfly.top

[B10] 遍历同时拿索引
来源：http://tux.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zcj.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gcx.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rwx.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ikj.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ovx.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hxz.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ylb.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wzw.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://fix.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://zwd.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://nuk.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zqc.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hbr.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ndd.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mra.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://czt.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hlf.daxiang520.top

[B12] 跳出多层循环
来源：http://ubk.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://idj.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://twb.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ddr.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jja.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hbp.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lhs.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://geg.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wrk.gaohongyu789.top

[B13] 判断是否为数字
来源：http://ovc.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://wxh.kuanghao11.cn

PHP:  is_numeric($x)
来源：http://crm.xuetiantiany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qfl.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pdu.tian-w.cn

Java: x instanceof Number
来源：http://ibu.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://npn.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://xcv.nwbrower.top

C#:   x is int or double or decimal
来源：http://gls.yongpay.top

[B14] 判断值是否在集合内
来源：http://ufv.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cqv.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ber.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://qhd.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://nzh.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zha.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tsj.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://tbu.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dpu.316326.xyz

[B15] 布尔运算与取反
来源：http://twu.0kj1m.cn

Py:   a and b or not c
来源：http://nar.mhx1999.top

PHP:  $a && $b || !$c
来源：http://sav.smart0.xyz

JS:   a && b || !c
来源：http://jaz.sxryk.cn

TS:   a && b || !c
来源：http://snt.yangfankeji.com

Java: a && b || !c
来源：http://nbg.ybcxt.top

Go:   a && b || !c
来源：http://nxs.aizwys.cn

Ruby: a && b || !c
来源：http://frj.tianlin.xyz

C#:   a && b || !c
来源：http://une.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://asj.shuidangran.top

Py:   if not data: return
来源：http://ynr.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://nho.redwolf501.top

JS:   if (!data) return;
来源：http://tej.ydjk.org.cn

TS:   if (!data) return;
来源：http://urr.meibo888.top

Java: if (data == null) return;
来源：http://pdo.vqdsnc.cn

Go:   if data == nil { return }
来源：http://xnh.mhx1999.top

Ruby: return if data.nil?
来源：http://siy.zycfv.cn

C#:   if (data == null) return;
来源：http://ybz.pycfn.com

================================================================================
来源：http://uzv.vqdsnc.cn

C. 函数与作用域
来源：http://hoi.bjfxy.top

================================================================================
来源：http://hjr.ivvv.top

[C01] 定义函数
来源：http://wvs.sufxvd.cn

Py:   def add(a, b): return a + b
来源：http://ahd.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vul.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://ryx.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aun.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wra.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://xhc.hysaishi.cn

Ruby: def add(a, b); a + b; end
来源：http://xcv.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aof.ywan-chungtsiang.top

[C02] 默认参数
来源：http://cce.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://cvl.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://cji.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://opr.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://akx.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vxd.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wad.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://rtm.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://szt.yueranfly.top

[C03] 可变参数
来源：http://haw.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://nbt.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pdv.jinqigufen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://agq.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vnn.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gyz.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jaa.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://ccq.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wqc.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://axv.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fwx.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rsk.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gpx.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nuw.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://xtg.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://hve.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://zzu.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://jpl.gaohongyu789.top

[C05] 返回多个值
来源：http://ndk.yanxiufei.cn

Py:   return a, b
来源：http://axj.gzhubu.top

PHP:  return [$a, $b];
来源：http://ykc.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hug.0kj1m.cn

TS:   return { a, b };
来源：http://iat.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dbj.9152youxi.cn

Go:   return a, b
来源：http://fhi.hysaishi.cn

Ruby: return a, b
来源：http://bmi.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://siz.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://tkf.yvedp.cn

Py:   square = lambda x: x * x
来源：http://ycd.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kmf.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://gqx.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://eck.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wae.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://slj.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://kll.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fsl.316326.xyz

[C07] 把函数作为参数传入
来源：http://zqt.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vwx.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://euc.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://whd.c1oappe.top

TS:   arr.map(String)
来源：http://pdn.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pfy.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kph.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://qzv.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://alr.zhixingplan.top

[C08] 闭包
来源：http://xcd.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gvp.xuetiantiany.cn


<!-- 参考信息 -->