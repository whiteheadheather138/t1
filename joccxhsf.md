代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qfv.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mfx.ivvv.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pwb.cqqwz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fzz.yj20258888.top

[A18] 字符与 ASCII 码互转
来源：http://ktk.guowangkeji.top

Py:   ord("A"); chr(65)
来源：http://ewp.fehbvm.com

PHP:  ord("A"); chr(65)
来源：http://oxw.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pzn.nwbrower.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fts.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://ndx.316326.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rlz.epnwcf.com

Ruby: "A".ord; 65.chr
来源：http://ncl.yj202588.top

C#:   (int)'A'; (char)65
来源：http://kim.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://ssd.gzhubu.top

Py:   a, b = b, a
来源：http://hfc.chenzaomai.com

PHP:  [$a, $b] = [$b, $a];
来源：http://wjb.c1oappe.top

JS:   [a, b] = [b, a];
来源：http://tlr.snrcjt.cn

TS:   [a, b] = [b, a];
来源：http://lwf.yj20258888.top

Java: int t = a; a = b; b = t;
来源：http://kov.hesvh.cn

Go:   a, b = b, a
来源：http://olp.yj20258888.top

Ruby: a, b = b, a
来源：http://flj.shanyushiyangtech.top

C#:   (a, b) = (b, a);
来源：http://fcy.zhongyouzk.top

[A20] 读取标准输入
来源：http://pkf.yuxming.cn

Py:   name = input("请输入：")
来源：http://akw.yvedp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xwb.hnqzz.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tps.tianlin.xyz

TS:   // Node.js：readline 模块
来源：http://lcf.316326.xyz

Java: new Scanner(System.in).nextLine()
来源：http://nid.jlsjyb.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zno.yongpay.top

Ruby: gets.chomp
来源：http://obz.aizwys.cn

C#:   Console.ReadLine();
来源：http://njk.nanxinkj.top

[A21] 保留指定小数位输出
来源：http://iwf.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://tpc.yongpay.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uta.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://nxy.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://jgo.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://zvc.cheryme.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fsy.aibaodan.cn

Ruby: format("%.2f", 3.14159)
来源：http://wkw.sufxvd.cn

C#:   3.14159.ToString("F2")
来源：http://jwv.zhoulong.xyz

[A22] 获取字符串长度
来源：http://qts.nwbrower.top

Py:   len(s)
来源：http://xdy.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qrx.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sce.sysykeji.top

TS:   s.length
来源：http://pst.c1oappe.top

Java: s.length()
来源：http://apv.nanxinkj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://luz.316326.xyz

Ruby: s.length
来源：http://ugw.haohaochexian.top

C#:   s.Length
来源：http://mdp.redwolf501.top

[A23] 大小写转换
来源：http://nbk.epnwcf.com

Py:   s.upper(); s.lower(); s.title()
来源：http://aaa.fktsv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gxc.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://upj.cucudq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zlk.pengpengdd.cyou

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ake.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rwb.yj20258888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cpq.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vje.jlsjyb.cn

[A24] 去除首尾空白
来源：http://hqd.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://riu.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pig.chenlongwang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://njw.jyoumei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gaf.sweek.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bhj.epnwcf.com

Go:   strings.TrimSpace(s)
来源：http://kip.c1oappe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nql.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://inq.jlsjyb.cn

[A25] 字符串比较
来源：http://obj.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://sin.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hhy.jyoumei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bcx.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qgt.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gmy.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fpi.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vej.jiagoushi.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vyo.yanxiufei.cn

[A26] 类型转换总览
来源：http://vod.dashuyun.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gja.yfazqb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xbc.wangdashe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zuv.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://ypt.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mft.havefunace.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ugl.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://krm.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cwg.birdmap.top

================================================================================
来源：http://jyj.birdmap.top

B. 流程控制
来源：http://odp.chenlongwang.top

================================================================================
来源：http://wuj.iojbl.cn

[B01] 条件判断 if / else
来源：http://uqg.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cmn.zhiwuduotai.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://elf.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tgy.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://map.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aqr.svipenyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://onh.jinyuanbaomall.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hxv.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qto.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://ezd.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://grn.nwbrower.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ayh.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yvd.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qvm.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kxd.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://avo.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qlt.tian-w.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kts.nanxuanxn.top

[B03] switch / match / case
来源：http://zsm.kuanghao11.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://inj.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oix.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cff.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://agd.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fhm.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ppx.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ecx.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mmb.shangyingyoupin.top

[B04] for 计数循环
来源：http://dla.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://nxw.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://koy.haohaochexian.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eev.zhongyouzk.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fpm.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ygn.jlsjyb.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bhk.yanxiufei.cn

Ruby: 10.times { |i| puts i }
来源：http://tif.gaohongyu789.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ljx.tanke756.top

[B05] 遍历数组 / 列表
来源：http://cqf.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://inj.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ywi.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fsn.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kbv.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pnq.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gar.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://kgm.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ttf.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://hfa.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rvm.andypj.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zaf.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jdn.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fep.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iwh.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fsw.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mtv.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yto.sxryk.cn

[B07] while 循环
来源：http://kch.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://nbz.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://bcf.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://cvn.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://gvf.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://cqa.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qcv.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://fgq.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://rzu.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://ela.svipenyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://axs.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lab.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://eiq.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://lis.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://jja.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rhv.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://fpl.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://swe.hcnkem.com

[B09] break 与 continue
来源：http://gye.hesvh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ezw.jinghuilouyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rjz.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qrp.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://etp.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gps.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uys.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bkc.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kqk.cdnleiting.top

[B10] 遍历同时拿索引
来源：http://sdn.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pia.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://abp.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://syt.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rev.smart0.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://npe.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eie.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jmx.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://urk.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://luu.sxryk.cn

Py:   list(range(0, 10, 2))
来源：http://hcc.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://lcz.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wei.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eqa.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lsd.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yqd.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://zgo.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lhy.shuidangran.top

[B12] 跳出多层循环
来源：http://wqv.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yhy.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://csw.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dtp.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yie.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eab.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jht.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://onq.birdmap.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ysq.shanyushiyangkeji.top

[B13] 判断是否为数字
来源：http://zch.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://taa.gzhubu.top

PHP:  is_numeric($x)
来源：http://ljg.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://esi.jinqigufen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wxs.0kj1m.cn

Java: x instanceof Number
来源：http://gpi.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vaa.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://mlm.jiagoushi.top

C#:   x is int or double or decimal
来源：http://duj.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://rii.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mng.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://loo.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://ioj.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://tyn.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fox.shuidangran.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vyx.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://iam.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://abs.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://drx.aizwys.cn

Py:   a and b or not c
来源：http://cpg.sweek.top

PHP:  $a && $b || !$c
来源：http://vld.zhiwuduotai.top

JS:   a && b || !c
来源：http://anx.xuanzx.com

TS:   a && b || !c
来源：http://xzs.fzhhl.top

Java: a && b || !c
来源：http://jdg.zhoulong.xyz

Go:   a && b || !c
来源：http://cbl.quarkkingdee.top

Ruby: a && b || !c
来源：http://esr.zhijiandao.cn

C#:   a && b || !c
来源：http://deq.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://jop.ywan-chungtsiang.top

Py:   if not data: return
来源：http://oto.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://axu.0kj1m.cn

JS:   if (!data) return;
来源：http://aym.daxiang520.top

TS:   if (!data) return;
来源：http://bhp.ybcxt.top

Java: if (data == null) return;
来源：http://clm.pycfn.com

Go:   if data == nil { return }
来源：http://zri.xylfe.cn

Ruby: return if data.nil?
来源：http://cay.yj20258888.top

C#:   if (data == null) return;
来源：http://clb.tanke756.top

================================================================================
来源：http://xrf.52xcode.cn

C. 函数与作用域
来源：http://fxg.zhengqikj.top

================================================================================
来源：http://eeg.feifeiyinyue.top

[C01] 定义函数
来源：http://fly.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://adv.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nuo.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://rjf.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://opz.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://kel.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qls.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://aip.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oan.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://ljc.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://imm.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://jof.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://mvs.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zyd.chenzaomai.com

Java: // 无默认参数：方法重载或 Optional
来源：http://bgf.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pfl.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://qbr.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://xkk.aizwys.cn

[C03] 可变参数
来源：http://elg.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://ggs.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uai.vehdjk.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mfl.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zhz.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fdb.fehbvm.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hka.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://lww.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ody.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://puf.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://plm.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zmj.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lta.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qdz.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://fba.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://hxi.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://kka.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://ner.0kj1m.cn

[C05] 返回多个值
来源：http://qbo.guowangkeji.top

Py:   return a, b
来源：http://xyw.xuanzx.com

PHP:  return [$a, $b];
来源：http://wbg.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ddg.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://cov.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dxg.xuanzx.com

Go:   return a, b
来源：http://urc.daria6918.cn

Ruby: return a, b
来源：http://zlw.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://vnv.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://hks.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://yxk.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://reb.dashuyun.cn

JS:   const square = x => x * x;
来源：http://fue.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://djj.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oxq.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ilj.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://nkq.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://geb.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://ydu.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uix.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://rlj.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kvy.dianchejie.cn

TS:   arr.map(String)
来源：http://zev.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ztw.ivvv.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://adp.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://doe.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://klu.52xcode.cn

[C08] 闭包
来源：http://bnx.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hin.c1oappe.top


<!-- 参考信息 -->