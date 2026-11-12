代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://gjc.jqgfzy.top

Py:   ord("A"); chr(65)
来源：http://erc.316326.xyz

PHP:  ord("A"); chr(65)
来源：http://cxm.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iit.hfpthk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tzm.zdbjq.cn

Java: (int) 'A'; (char) 65
来源：http://bwu.jqgfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jwz.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://inh.tian-w.cn

C#:   (int)'A'; (char)65
来源：http://kcu.yueranfly.top

[A19] 交换两个变量
来源：http://cam.vehdjk.com

Py:   a, b = b, a
来源：http://csl.snrcjt.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lhk.dashuyun.cn

JS:   [a, b] = [b, a];
来源：http://gmc.jlsjyb.cn

TS:   [a, b] = [b, a];
来源：http://ybp.chenlongwang.top

Java: int t = a; a = b; b = t;
来源：http://zgb.ybcxt.top

Go:   a, b = b, a
来源：http://kkd.kuanghao11.cn

Ruby: a, b = b, a
来源：http://wzf.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://hoq.yueranfly.top

[A20] 读取标准输入
来源：http://mtw.tarul.cn

Py:   name = input("请输入：")
来源：http://ook.aizwys.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xqv.hysaishi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ved.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://krr.ybcxt.top

Java: new Scanner(System.in).nextLine()
来源：http://xqy.sufxvd.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ena.gogol.net.cn

Ruby: gets.chomp
来源：http://uyn.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://wbx.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://ycd.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://ndr.hnqzz.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hqe.fktsv.cn

JS:   (3.14159).toFixed(2)
来源：http://zio.daxiang520.top

TS:   (3.14159).toFixed(2)
来源：http://led.yvedp.cn

Java: String.format("%.2f", 3.14159)
来源：http://gdp.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gpv.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://vew.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://afu.bbcook.cn

[A22] 获取字符串长度
来源：http://zuq.316326.xyz

Py:   len(s)
来源：http://xbh.0kj1m.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tgh.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kpu.shuidangran.top

TS:   s.length
来源：http://kxo.hcnkem.com

Java: s.length()
来源：http://ujp.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://caf.xuanzx.com

Ruby: s.length
来源：http://emh.haohaochexian.top

C#:   s.Length
来源：http://uzp.cashguo.top

[A23] 大小写转换
来源：http://mva.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mzy.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vzp.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tio.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ges.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dki.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://evz.svipenyu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jmy.zdqjudy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://teh.nwbrower.top

[A24] 去除首尾空白
来源：http://zmt.dashuyun.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nvv.jqgufenzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://khu.guannengcc.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sgh.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqm.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kuj.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://cvt.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lak.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xfo.jlsjyb.cn

[A25] 字符串比较
来源：http://kuq.daria6918.cn

Py:   s1 == s2; s1 != s2
来源：http://pzd.jianghu66.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bic.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gel.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ciz.yongpay.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://azp.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hfg.zhengqikj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://avy.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fow.sysykeji.top

[A26] 类型转换总览
来源：http://ahw.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rik.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yhg.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jlj.hcnkem.com

TS:   Number() String() Boolean() x as number
来源：http://ftb.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hfz.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://erb.316326.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://nzt.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eof.zhiwuduotai.top

================================================================================
来源：http://imn.nanxuanxn.top

B. 流程控制
来源：http://ktp.haohaochexian.top

================================================================================
来源：http://xmx.yj20258888.top

[B01] 条件判断 if / else
来源：http://ytb.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lyw.zhiwuduotai.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ofe.ivvv.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tos.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wxm.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hrh.cucudq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yxa.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vbj.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bhd.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://lkz.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cuk.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wzt.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dtc.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdb.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sxk.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gig.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gzo.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hke.tanke756.top

[B03] switch / match / case
来源：http://ymw.jinyuanbaomall.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lnp.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qrz.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://svl.ydzc1.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wrm.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sqe.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lkw.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yqb.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://elo.cqqwz.cn

[B04] for 计数循环
来源：http://qpg.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://bco.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://exc.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://thn.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ixh.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zqa.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kmp.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://bxr.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rsh.iojbl.cn

[B05] 遍历数组 / 列表
来源：http://bou.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://irc.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hwf.9152youxi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://enl.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://dyz.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gut.jinghuilouyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pdz.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://bkg.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aqd.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://liz.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sii.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ypk.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ptc.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yre.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xkh.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bon.316326.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vkh.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://itd.guannengcc.top

[B07] while 循环
来源：http://umt.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://gvw.vehdjk.com

PHP:  while ($i < 10) { $i++; }
来源：http://lau.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://wll.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://vhy.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://xyj.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ubv.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://ttt.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://daq.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://zuz.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://cqc.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nnq.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://kcn.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://tld.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://fyg.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://oum.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pwz.zhiwuduotai.top

C#:   do { i++; } while (i < 10);
来源：http://fdn.dianchejie.cn

[B09] break 与 continue
来源：http://hri.shangyingyoupin.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://icd.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qtp.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svi.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dla.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dyx.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kod.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yub.meibo888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbj.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://irv.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rif.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xuv.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rmt.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vbb.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iko.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rva.yanxiufei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wnp.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pds.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://jhd.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://jds.tarul.cn

PHP:  range(0, 10, 2);
来源：http://xkf.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sjk.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kkc.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hct.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pqy.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://ehd.fehbvm.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pjj.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://vzj.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://buu.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mzq.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://osu.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://apy.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vcb.zhoulong.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gdj.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qet.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nip.52xcode.cn

[B13] 判断是否为数字
来源：http://rgk.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://emr.yuanzhike.top

PHP:  is_numeric($x)
来源：http://fgx.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kgm.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fwp.jlsjyb.cn

Java: x instanceof Number
来源：http://tfi.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://teb.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://alc.yuanzhike.top

C#:   x is int or double or decimal
来源：http://hom.xylfe.cn

[B14] 判断值是否在集合内
来源：http://tgw.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lre.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://awu.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://dhv.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://vph.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mcg.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yvk.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://bsa.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ded.xziqi.cn

[B15] 布尔运算与取反
来源：http://aja.cheryme.top

Py:   a and b or not c
来源：http://bfc.smart0.xyz

PHP:  $a && $b || !$c
来源：http://xpe.sweek.top

JS:   a && b || !c
来源：http://ddd.jiagoushi.top

TS:   a && b || !c
来源：http://frd.zhaomingkeji.xyz

Java: a && b || !c
来源：http://bzl.jiagoushi.top

Go:   a && b || !c
来源：http://yqz.yj202588.top

Ruby: a && b || !c
来源：http://dgx.nanxuanxn.top

C#:   a && b || !c
来源：http://izj.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://lcz.ywan-chungtsiang.top

Py:   if not data: return
来源：http://xgx.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://eaq.cheryme.top

JS:   if (!data) return;
来源：http://irz.yanxiufei.cn

TS:   if (!data) return;
来源：http://yyi.tarul.cn

Java: if (data == null) return;
来源：http://ngg.shuidangran.top

Go:   if data == nil { return }
来源：http://vis.havefunace.top

Ruby: return if data.nil?
来源：http://fnc.chenzaomai.com

C#:   if (data == null) return;
来源：http://axq.vqdsnc.cn

================================================================================
来源：http://akv.hnxiangtu.top

C. 函数与作用域
来源：http://aaf.nwbrower.top

================================================================================
来源：http://ijv.gogol.net.cn

[C01] 定义函数
来源：http://czj.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://zei.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ftb.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://byz.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxk.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aja.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://vrm.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://cnn.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://awd.uphjek.com

[C02] 默认参数
来源：http://dfa.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://btu.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ijf.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://hbz.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ztu.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://vpd.ywan-chungtsiang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qiy.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://jgx.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://tys.ywan-chungtsiang.top

[C03] 可变参数
来源：http://ink.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://nyo.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://arc.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vjm.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tor.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zrr.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wha.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hlg.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kii.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://rcb.shuidangran.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ibm.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vvn.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fpz.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://upy.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://uef.bbcook.cn

Go:   // 无：用配置结构体参数
来源：http://jjp.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://uqi.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://euv.feifeiyinyue.top

[C05] 返回多个值
来源：http://bcj.ctjpmb.com

Py:   return a, b
来源：http://mqr.tianlin.xyz

PHP:  return [$a, $b];
来源：http://mmb.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jto.chenlongwang.top

TS:   return { a, b };
来源：http://smr.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qbb.zhiwuduotai.top

Go:   return a, b
来源：http://gjm.yangfankeji.com

Ruby: return a, b
来源：http://wun.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://fmc.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://arh.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://ief.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://npq.snrcjt.cn

JS:   const square = x => x * x;
来源：http://fqt.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://uke.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rzs.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://own.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://tpw.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://uyk.ydzc1.top

[C07] 把函数作为参数传入
来源：http://btc.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ayt.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://pzt.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lxn.snrcjt.cn

TS:   arr.map(String)
来源：http://ubi.zhaomingkeji.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vtr.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fam.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://dzd.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vxw.dianchejie.cn

[C08] 闭包
来源：http://pig.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dgk.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://akf.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cxl.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gao.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mie.shuidangran.top


<!-- 参考信息 -->