代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://wzf.chenzaomai.com

Py:   ord("A"); chr(65)
来源：http://ild.birdmap.top

PHP:  ord("A"); chr(65)
来源：http://qsc.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ugy.wangdashe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ymt.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://sfj.mhx1999.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wge.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://ldp.zhijiandao.cn

C#:   (int)'A'; (char)65
来源：http://vpm.tianlin.xyz

[A19] 交换两个变量
来源：http://ggu.svipenyu.cn

Py:   a, b = b, a
来源：http://yjq.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://uuq.xinyue.icu

JS:   [a, b] = [b, a];
来源：http://cmy.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://xhd.tian-w.cn

Java: int t = a; a = b; b = t;
来源：http://dce.fzhhl.top

Go:   a, b = b, a
来源：http://gih.hfpthk.cn

Ruby: a, b = b, a
来源：http://yhj.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://vhe.yj202588.top

[A20] 读取标准输入
来源：http://lpy.pycfn.com

Py:   name = input("请输入：")
来源：http://zob.uphjek.com

PHP:  $name = trim(fgets(STDIN));
来源：http://wfa.zhoulong.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ual.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://mbk.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://ptx.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zbl.xingfuxueyuan.xyz

Ruby: gets.chomp
来源：http://wdr.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://wnm.ydjk.org.cn

[A21] 保留指定小数位输出
来源：http://ibs.nwbrower.top

Py:   f"{3.14159:.2f}"
来源：http://obh.jinqigufen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fbq.cdnleiting.top

JS:   (3.14159).toFixed(2)
来源：http://bwf.yongpay.top

TS:   (3.14159).toFixed(2)
来源：http://yks.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://qrm.ydjk.org.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://snk.ydjk.org.cn

Ruby: format("%.2f", 3.14159)
来源：http://kqc.zhongyouzk.top

C#:   3.14159.ToString("F2")
来源：http://gwc.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://rtg.vehdjk.com

Py:   len(s)
来源：http://alz.yuanzhike.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ati.zdqjudy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nge.daxiang520.top

TS:   s.length
来源：http://kif.sufxvd.cn

Java: s.length()
来源：http://bhs.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bzf.yj20258888.top

Ruby: s.length
来源：http://kxg.cashguo.top

C#:   s.Length
来源：http://lkf.zhengqikj.top

[A23] 大小写转换
来源：http://npy.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pts.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jtt.dashuyun.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mwh.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://twu.tanke756.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zru.shangyingyoupin.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ixp.ctjpmb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wtu.fengsongda.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wjn.fanxiaobao.xyz

[A24] 去除首尾空白
来源：http://uar.gotoacloud.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fqa.guowangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jvp.chenlongwang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kpd.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zgu.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bak.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://jnl.tianlin.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ayr.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://owo.cdnleiting.top

[A25] 字符串比较
来源：http://qew.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://cua.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://otr.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bsz.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://efy.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hli.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qkq.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zbi.redwolf501.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iws.jianghu66.top

[A26] 类型转换总览
来源：http://zdm.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://isq.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bfr.nwbrower.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cvo.sxryk.cn

TS:   Number() String() Boolean() x as number
来源：http://wyn.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jqd.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jsd.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cbd.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pkv.pengpengdd.cyou

================================================================================
来源：http://per.epnwcf.com

B. 流程控制
来源：http://uzw.jinqigfzy.top

================================================================================
来源：http://unq.cqqwz.cn

[B01] 条件判断 if / else
来源：http://yzn.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gyy.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wpu.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gha.9152youxi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zfy.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zga.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://djn.tanke756.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jyv.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yqq.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://jer.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://foz.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://der.jinqigufen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qns.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nkb.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyr.vqdsnc.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pjn.hesvh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://crt.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aak.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://adp.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ccr.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mqj.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gaq.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://clr.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rqf.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nhx.zhaomingkeji.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://okj.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gbl.zhixingplan.top

[B04] for 计数循环
来源：http://xhm.havefunace.top

Py:   for i in range(10): print(i)
来源：http://fox.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://adt.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pbo.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nfa.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xpx.jinqigfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lgs.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://ocs.zdbjq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qcs.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://drp.vehdjk.com

Py:   for item in arr: print(item)
来源：http://zxx.chenjidiqi.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dzv.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://abk.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://twn.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://wbb.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ngo.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://mls.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pyx.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://enp.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bec.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lmc.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ufu.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pev.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zhf.zdqjudy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pyz.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dce.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zqe.yongpay.top

[B07] while 循环
来源：http://rfc.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://hjz.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://joh.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://kbh.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://cro.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://ylw.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hee.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://edq.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://ijb.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://uwa.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://gsh.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://amy.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://jxf.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://pgt.shzxlz.cn

Java: do { i++; } while (i < 10);
来源：http://ibg.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bzf.jinghuilouyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://utz.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://kkw.zhixingplan.top

[B09] break 与 continue
来源：http://bcw.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gzp.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://apj.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nkf.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://znq.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjk.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lwh.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ewa.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fhs.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://tak.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://txu.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wdy.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zmp.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jft.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ovp.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nyz.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tlp.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rgb.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://gea.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://vid.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://zzt.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mgg.sufxvd.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://atc.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://swj.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oac.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://tcb.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://csf.fehbvm.com

[B12] 跳出多层循环
来源：http://wfw.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vct.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tmy.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fid.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kco.guowangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://beo.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gwo.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cld.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dqm.vqdsnc.cn

[B13] 判断是否为数字
来源：http://bbe.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://anp.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://pwy.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rzi.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ama.vqdsnc.cn

Java: x instanceof Number
来源：http://iko.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://llm.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://emu.cdnleiting.top

C#:   x is int or double or decimal
来源：http://fck.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://new.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jjx.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gas.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://dzn.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://hca.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xnn.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lsv.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://cdx.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://psj.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://bqm.sysykeji.top

Py:   a and b or not c
来源：http://vug.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://tup.hnxiangtu.top

JS:   a && b || !c
来源：http://yyl.pengpengdd.cyou

TS:   a && b || !c
来源：http://lyh.cdnleiting.top

Java: a && b || !c
来源：http://ylt.snrcjt.cn

Go:   a && b || !c
来源：http://jvg.fehbvm.com

Ruby: a && b || !c
来源：http://tnt.yj20258888.top

C#:   a && b || !c
来源：http://ncf.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://zuy.hnqzz.top

Py:   if not data: return
来源：http://iul.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://otv.yfazqb.com

JS:   if (!data) return;
来源：http://xqn.haohaochexian.top

TS:   if (!data) return;
来源：http://uje.fzhhl.top

Java: if (data == null) return;
来源：http://gon.dashuyun.cn

Go:   if data == nil { return }
来源：http://dil.cucudq.cn

Ruby: return if data.nil?
来源：http://kth.yuanzhike.top

C#:   if (data == null) return;
来源：http://flb.meibo888.top

================================================================================
来源：http://pnv.yfazqb.com

C. 函数与作用域
来源：http://xmr.jyoumei.cn

================================================================================
来源：http://vkx.zhijiandao.cn

[C01] 定义函数
来源：http://rpz.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://mzo.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jyk.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://ipm.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kxh.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://twj.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://cvt.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://gfl.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://goy.chenlongwang.top

[C02] 默认参数
来源：http://hog.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://dcv.ehwqpu.com

PHP:  function greet($name = "World") { return $name; }
来源：http://klo.daria6918.cn

JS:   function greet(name = "World") { return name; }
来源：http://dtc.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://umk.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uho.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rhq.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://nle.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://jny.smart0.xyz

[C03] 可变参数
来源：http://rai.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://kcy.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://biz.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://csf.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ieb.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xjc.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tjw.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://tmz.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rnh.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://hxg.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://etf.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vke.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pva.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://obx.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://bxr.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://dtb.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://meb.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://ihn.zdqjudy.top

[C05] 返回多个值
来源：http://fvm.ehwqpu.com

Py:   return a, b
来源：http://jwg.fzhhl.top

PHP:  return [$a, $b];
来源：http://jmn.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://sov.meibo888.top

TS:   return { a, b };
来源：http://ylf.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ycy.xylfe.cn

Go:   return a, b
来源：http://kzn.cheryme.top

Ruby: return a, b
来源：http://iui.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://qhn.tian-w.cn

[C06] 匿名函数 / lambda
来源：http://sgd.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://jky.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ndr.guowangkeji.top

JS:   const square = x => x * x;
来源：http://pkk.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://coj.tian-w.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ctt.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://uxm.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://ckg.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://nja.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://vah.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zqa.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://pwk.yanxiufei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hzf.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://orc.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qey.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fya.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://uiq.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qoo.hammf.cn

[C08] 闭包
来源：http://frz.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vks.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zfi.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zro.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rao.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nep.yonumen.top


<!-- 参考信息 -->