代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nzy.xinyue.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wiy.dianchejie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vuj.fengsongda.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jpk.jinqigfzy.top

[A18] 字符与 ASCII 码互转
来源：http://roq.hongshengwenyu.top

Py:   ord("A"); chr(65)
来源：http://zpt.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://mdl.chenlongwang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vyj.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wxk.hnxiangtu.top

Java: (int) 'A'; (char) 65
来源：http://sqh.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mdt.cashguo.top

Ruby: "A".ord; 65.chr
来源：http://kek.jyoumei.cn

C#:   (int)'A'; (char)65
来源：http://qat.wangdashe.top

[A19] 交换两个变量
来源：http://dpk.yueranfly.top

Py:   a, b = b, a
来源：http://qis.chenlongwang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lmc.tanke756.top

JS:   [a, b] = [b, a];
来源：http://kyd.shzxlz.cn

TS:   [a, b] = [b, a];
来源：http://iew.jianghu66.top

Java: int t = a; a = b; b = t;
来源：http://aoi.ivvv.top

Go:   a, b = b, a
来源：http://zwu.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://xpu.xylfe.cn

C#:   (a, b) = (b, a);
来源：http://jaj.xuetiantiany.cn

[A20] 读取标准输入
来源：http://xab.jianghu66.top

Py:   name = input("请输入：")
来源：http://yai.gotoacloud.top

PHP:  $name = trim(fgets(STDIN));
来源：http://aws.hfpthk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xth.gzhubu.top

TS:   // Node.js：readline 模块
来源：http://xne.hongshengwenyu.top

Java: new Scanner(System.in).nextLine()
来源：http://ixh.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://btj.vehdjk.com

Ruby: gets.chomp
来源：http://mbh.jinghuilouyu.cn

C#:   Console.ReadLine();
来源：http://ibz.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://tye.xingfuxueyuan.xyz

Py:   f"{3.14159:.2f}"
来源：http://pri.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://slv.jinghuilouyu.cn

JS:   (3.14159).toFixed(2)
来源：http://pkb.0kj1m.cn

TS:   (3.14159).toFixed(2)
来源：http://zix.pengpengdd.cyou

Java: String.format("%.2f", 3.14159)
来源：http://olx.bbcook.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gif.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://rsm.xingfuxueyuan.xyz

C#:   3.14159.ToString("F2")
来源：http://jun.yuxming.cn

[A22] 获取字符串长度
来源：http://tkc.shuidangran.top

Py:   len(s)
来源：http://uzp.vqdsnc.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kds.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fbi.yanxiufei.cn

TS:   s.length
来源：http://oro.vqdsnc.cn

Java: s.length()
来源：http://myo.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dwo.shanyushiyangtech.top

Ruby: s.length
来源：http://qql.yangfankeji.com

C#:   s.Length
来源：http://zse.shanyushiyangtech.top

[A23] 大小写转换
来源：http://sug.havefunace.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bwb.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ycv.snrcjt.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://asi.shanyushiyangtech.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wqo.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yax.jinghuilouyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tik.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jty.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pyg.hcnkem.com

[A24] 去除首尾空白
来源：http://pop.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://akl.sjlbkw.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://afe.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mfp.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mxt.yuanzhike.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rcy.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://mcz.yfazqb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xii.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ido.cqqwz.cn

[A25] 字符串比较
来源：http://zos.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://qko.hnqzz.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pef.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jvv.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wqw.jiagoushi.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zzn.9152youxi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jsm.chenzaomai.com

Ruby: s1 == s2; s1 <=> s2
来源：http://gyt.shuidangran.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kvc.yj20258888.top

[A26] 类型转换总览
来源：http://aiw.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sna.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eod.tanke756.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xwg.xuanzx.com

TS:   Number() String() Boolean() x as number
来源：http://ooh.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gfc.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tup.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ebq.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xde.bbcook.cn

================================================================================
来源：http://fkl.ywan-chungtsiang.top

B. 流程控制
来源：http://mix.vehdjk.com

================================================================================
来源：http://ron.wangdashe.top

[B01] 条件判断 if / else
来源：http://hyv.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vwh.zhoulong.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ruz.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lof.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ssw.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://trd.chenzaomai.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vts.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kgr.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mrp.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://rqz.mhx1999.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://apq.quarkkingdee.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://czn.epnwcf.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ynh.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vhe.hnqzz.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ryw.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rqs.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zry.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fsz.cqqwz.cn

[B03] switch / match / case
来源：http://sht.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qig.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ggl.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nww.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xxi.ctjpmb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dzt.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wjf.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xyk.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://htp.jlsjyb.cn

[B04] for 计数循环
来源：http://gjt.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://eux.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sju.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bla.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://exl.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lpm.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://alw.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://eei.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nqa.jinqigufen.top

[B05] 遍历数组 / 列表
来源：http://tip.vehdjk.com

Py:   for item in arr: print(item)
来源：http://pnj.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jqy.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ovl.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://pce.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cny.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mbe.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://njx.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uow.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://ybm.ctjpmb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://oft.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ecf.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fwy.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hzn.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wqv.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bgf.yj20258888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wvn.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kpq.zhaomingkeji.xyz

[B07] while 循环
来源：http://gne.uphjek.com

Py:   while i < 10: i += 1
来源：http://npn.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pks.jinqigfzy.top

JS:   while (i < 10) { i++; }
来源：http://pfd.yj20258888.top

TS:   while (i < 10) { i++; }
来源：http://ivd.yongpay.top

Java: while (i < 10) { i++; }
来源：http://owc.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jvb.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://ywa.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://hpf.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://huj.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://bix.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xwv.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://vgi.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://oxj.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://aul.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://nks.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://qgm.quarkkingdee.top

C#:   do { i++; } while (i < 10);
来源：http://zru.xuetiantiany.cn

[B09] break 与 continue
来源：http://zhq.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pjt.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yxa.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rbs.pengpengdd.cyou

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sgm.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsu.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uti.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zrd.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kvp.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://xrw.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rko.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xvk.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ifl.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fol.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nub.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dsx.jinqigfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nzq.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ryu.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://trp.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://cin.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://ecz.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kdy.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eib.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hhf.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eay.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://jac.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qvh.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://ekf.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vnw.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://quv.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fdt.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eqh.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sbl.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yhc.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ryc.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jjv.ctjpmb.com

[B13] 判断是否为数字
来源：http://ysg.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://vof.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://fga.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oda.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zpa.gogol.net.cn

Java: x instanceof Number
来源：http://whh.jlsjyb.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uuj.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://jdk.jiagoushi.top

C#:   x is int or double or decimal
来源：http://iwb.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://phd.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vrk.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ggd.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://xfc.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://mzr.gzhubu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ayi.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vbb.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zcx.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yus.havefunace.top

[B15] 布尔运算与取反
来源：http://tbt.yongpay.top

Py:   a and b or not c
来源：http://ors.yuxming.cn

PHP:  $a && $b || !$c
来源：http://hes.hywenlv.cn

JS:   a && b || !c
来源：http://yns.daxiang520.top

TS:   a && b || !c
来源：http://ycs.pengpengdd.cyou

Java: a && b || !c
来源：http://kqs.xziqi.cn

Go:   a && b || !c
来源：http://niv.iojbl.cn

Ruby: a && b || !c
来源：http://nwr.tianlin.xyz

C#:   a && b || !c
来源：http://krp.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://hzr.kuanghao11.cn

Py:   if not data: return
来源：http://qhc.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://kvb.yj20258.top

JS:   if (!data) return;
来源：http://rqx.gotoacloud.top

TS:   if (!data) return;
来源：http://mxg.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://cbp.xziqi.cn

Go:   if data == nil { return }
来源：http://ssy.fengsongda.top

Ruby: return if data.nil?
来源：http://rbq.9152youxi.cn

C#:   if (data == null) return;
来源：http://vau.zdbjq.cn

================================================================================
来源：http://ouf.hfpthk.cn

C. 函数与作用域
来源：http://jmj.hnxiangtu.top

================================================================================
来源：http://gry.sxryk.cn

[C01] 定义函数
来源：http://ull.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://boe.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://unp.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://gzo.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ipd.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gra.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://jzn.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://ude.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nwa.hysaishi.cn

[C02] 默认参数
来源：http://uog.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://zqx.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://kmm.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://xcv.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tlb.cdnleiting.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ixx.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tif.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://dvv.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://rog.hammf.cn

[C03] 可变参数
来源：http://lfb.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://jdq.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fym.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qnj.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xdy.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xtd.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://euc.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uwh.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tth.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://rvk.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bve.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kwq.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bjl.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xeh.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://wmh.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://nyr.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://aol.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://whl.smart0.xyz

[C05] 返回多个值
来源：http://obo.mhx1999.top

Py:   return a, b
来源：http://xxo.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://uwu.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://cdv.jianghu66.top

TS:   return { a, b };
来源：http://kpi.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tel.wangshuangyany.cn

Go:   return a, b
来源：http://mne.yvedp.cn

Ruby: return a, b
来源：http://qzp.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://roj.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://osk.zhiwuduotai.top

Py:   square = lambda x: x * x
来源：http://uoe.316326.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://nxj.cdnleiting.top

JS:   const square = x => x * x;
来源：http://yxn.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://blm.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://joe.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://aaa.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://jmb.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://iqx.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://kmm.redwolf501.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ust.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ree.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mfn.yj202588.top

TS:   arr.map(String)
来源：http://zkv.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://djd.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://app.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://una.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://rlc.tianlin.xyz

[C08] 闭包
来源：http://pba.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zub.cdnleiting.top


<!-- 参考信息 -->