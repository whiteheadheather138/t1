代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oaa.yonumen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zex.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcx.xuanzx.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kgu.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://jqd.9152youxi.cn

Py:   ord("A"); chr(65)
来源：http://xnl.sjlbkw.cn

PHP:  ord("A"); chr(65)
来源：http://rut.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dzl.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xsh.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://qtk.tanke756.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jlt.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://hpn.pycfn.com

C#:   (int)'A'; (char)65
来源：http://uwl.ydzc1.top

[A19] 交换两个变量
来源：http://lqe.ppjwa.cn

Py:   a, b = b, a
来源：http://hvs.jinyuanbaomall.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ouh.hesvh.cn

JS:   [a, b] = [b, a];
来源：http://puz.svipenyu.cn

TS:   [a, b] = [b, a];
来源：http://hrl.meibo888.top

Java: int t = a; a = b; b = t;
来源：http://ooy.epnwcf.com

Go:   a, b = b, a
来源：http://nzs.tarul.cn

Ruby: a, b = b, a
来源：http://cnf.chenlongwang.top

C#:   (a, b) = (b, a);
来源：http://tpg.birdmap.top

[A20] 读取标准输入
来源：http://txj.nwbrower.top

Py:   name = input("请输入：")
来源：http://xyg.yuxming.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oms.zhiwuduotai.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://flt.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://kuq.jinqigfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://dht.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oba.hcnkem.com

Ruby: gets.chomp
来源：http://qsh.fengsongda.top

C#:   Console.ReadLine();
来源：http://uxu.iojbl.cn

[A21] 保留指定小数位输出
来源：http://qfb.yanxiufei.cn

Py:   f"{3.14159:.2f}"
来源：http://vij.birdmap.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kpq.sweek.top

JS:   (3.14159).toFixed(2)
来源：http://nzx.c1oappe.top

TS:   (3.14159).toFixed(2)
来源：http://ygp.gaohongyu789.top

Java: String.format("%.2f", 3.14159)
来源：http://qjz.jqgufenzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iip.smart0.xyz

Ruby: format("%.2f", 3.14159)
来源：http://imx.jyoumei.cn

C#:   3.14159.ToString("F2")
来源：http://wwy.jinqigfzy.top

[A22] 获取字符串长度
来源：http://wnd.daria6918.cn

Py:   len(s)
来源：http://rsr.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ewf.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nev.jqgfzy.top

TS:   s.length
来源：http://qep.hywenlv.cn

Java: s.length()
来源：http://jzf.ywan-chungtsiang.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wzv.vehdjk.com

Ruby: s.length
来源：http://lht.uphjek.com

C#:   s.Length
来源：http://vgv.vehdjk.com

[A23] 大小写转换
来源：http://gww.yj20258.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gra.dashuyun.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cct.kuanghao11.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://efy.snrcjt.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ncg.cdnleiting.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://usc.aibaodan.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gwm.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lvd.0kj1m.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vio.hcnkem.com

[A24] 去除首尾空白
来源：http://zdz.52xcode.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://buo.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vos.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ger.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tsy.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lrl.fehbvm.com

Go:   strings.TrimSpace(s)
来源：http://ukp.cdnleiting.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jcu.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bvj.hywenlv.cn

[A25] 字符串比较
来源：http://kdr.yfazqb.com

Py:   s1 == s2; s1 != s2
来源：http://gjn.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bmh.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jpo.yuxming.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kxq.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://muh.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://buc.ivvv.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tqg.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://itf.sjlbkw.cn

[A26] 类型转换总览
来源：http://tum.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dkc.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://otz.c1oappe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vyt.xylfe.cn

TS:   Number() String() Boolean() x as number
来源：http://bxk.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vjx.xylfe.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iez.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kim.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gbx.ivvv.top

================================================================================
来源：http://ofi.yueranfly.top

B. 流程控制
来源：http://xhv.shzxlz.cn

================================================================================
来源：http://yfd.yj20258.top

[B01] 条件判断 if / else
来源：http://jrm.bbcook.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://epm.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zdb.yangfankeji.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fuh.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://llg.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oqf.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vjj.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ihv.nanxuanxn.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cwk.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://gum.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lqz.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://acv.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qby.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jzx.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nvr.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pnf.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://udd.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvk.yonumen.top

[B03] switch / match / case
来源：http://lnx.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yei.fanxiaobao.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bjb.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cmo.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zfw.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oal.zhaomingkeji.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pzt.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://brs.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hhk.gogol.net.cn

[B04] for 计数循环
来源：http://abw.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://zei.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eay.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wxb.epnwcf.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lqx.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://roc.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hqp.birdmap.top

Ruby: 10.times { |i| puts i }
来源：http://ixt.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ymo.guannengcc.top

[B05] 遍历数组 / 列表
来源：http://szv.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://vly.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lmh.gzhubu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fag.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rdm.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rob.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ylo.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://rhs.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wsb.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://huk.gotoacloud.top

Py:   for k, v in d.items(): print(k, v)
来源：http://csu.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fua.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blv.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spq.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yzh.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ydq.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mom.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lts.ppjwa.cn

[B07] while 循环
来源：http://ymc.yj20258888.top

Py:   while i < 10: i += 1
来源：http://aqi.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://wvw.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://hbw.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://hpa.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://ynx.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://niv.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://wub.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://yqq.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://gkg.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://wxq.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rpt.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://rrb.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://geq.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://kko.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://efn.fanxiaobao.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://guv.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://wde.fzhhl.top

[B09] break 与 continue
来源：http://yjf.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qvy.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wzs.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iiy.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezy.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msw.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rgj.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bsc.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vee.yonumen.top

[B10] 遍历同时拿索引
来源：http://gvw.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ysz.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://swp.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kft.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lqj.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zak.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uqz.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rix.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zqi.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://wdg.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://twx.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://agy.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tlc.gotoacloud.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xoc.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oza.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://omz.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://mqv.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xrc.fengsongda.top

[B12] 跳出多层循环
来源：http://tpm.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rfc.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://div.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qwx.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rmw.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ixu.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ixj.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xea.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pwm.daria6918.cn

[B13] 判断是否为数字
来源：http://cfa.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://sva.quarkkingdee.top

PHP:  is_numeric($x)
来源：http://xwo.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gdd.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sbh.xuetiantiany.cn

Java: x instanceof Number
来源：http://ubd.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uhz.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://uhy.xziqi.cn

C#:   x is int or double or decimal
来源：http://exw.cheryme.top

[B14] 判断值是否在集合内
来源：http://lbc.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lzr.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://owx.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://snr.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://mze.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jtg.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rmy.cdnleiting.top

Ruby: [1, 2, 3].include?(x)
来源：http://kqf.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://inm.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://erc.snrcjt.cn

Py:   a and b or not c
来源：http://nou.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://tnn.yj20258888.top

JS:   a && b || !c
来源：http://aio.yangfankeji.com

TS:   a && b || !c
来源：http://xlf.hesvh.cn

Java: a && b || !c
来源：http://drs.ydjk.org.cn

Go:   a && b || !c
来源：http://wdo.iojbl.cn

Ruby: a && b || !c
来源：http://tvp.xuanzx.com

C#:   a && b || !c
来源：http://aog.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://noo.cdnleiting.top

Py:   if not data: return
来源：http://src.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://cla.dashuyun.cn

JS:   if (!data) return;
来源：http://wfj.ivvv.top

TS:   if (!data) return;
来源：http://eni.smart0.xyz

Java: if (data == null) return;
来源：http://spr.guannengcc.top

Go:   if data == nil { return }
来源：http://hte.9152youxi.cn

Ruby: return if data.nil?
来源：http://wvo.iojbl.cn

C#:   if (data == null) return;
来源：http://niu.hammf.cn

================================================================================
来源：http://kyz.iojbl.cn

C. 函数与作用域
来源：http://eur.wangshuangyany.cn

================================================================================
来源：http://rug.epnwcf.com

[C01] 定义函数
来源：http://rus.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://dlk.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbe.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://hdg.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fuw.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mgm.zhixingplan.top

Go:   func add(a, b int) int { return a + b }
来源：http://zyb.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://ksg.yonumen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nfl.316326.xyz

[C02] 默认参数
来源：http://dam.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://qpp.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ihw.zhoulong.xyz

JS:   function greet(name = "World") { return name; }
来源：http://wub.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qjc.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fps.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nff.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://uin.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://app.vqdsnc.cn

[C03] 可变参数
来源：http://sjy.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://kng.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vpe.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hyn.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ngg.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bqi.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sbd.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://uas.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dza.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://mli.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://exx.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pfc.daria6918.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ijg.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ywf.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://qlt.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://ldp.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://ump.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://ica.yj202588.top

[C05] 返回多个值
来源：http://szt.fanxiaobao.xyz

Py:   return a, b
来源：http://ygm.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://les.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mqn.yvedp.cn

TS:   return { a, b };
来源：http://hix.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mzt.gaohongyu789.top

Go:   return a, b
来源：http://ggg.chenzaomai.com

Ruby: return a, b
来源：http://kwv.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://mja.yonumen.top

[C06] 匿名函数 / lambda
来源：http://omr.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://urq.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ikv.cqqwz.cn

JS:   const square = x => x * x;
来源：http://fse.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://wzw.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wvf.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://tqo.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://hvk.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bjy.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://nua.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zga.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://dhe.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qtn.chenlongwang.top

TS:   arr.map(String)
来源：http://yri.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xid.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gvr.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://hne.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://frv.chenzaomai.com

[C08] 闭包
来源：http://jdt.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uog.jinghuilouyu.cn


<!-- 参考信息 -->