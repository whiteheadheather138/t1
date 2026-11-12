代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lht.redwolf501.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ogf.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pxs.ydzc1.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ciy.gogol.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rxj.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sgy.ppjwa.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sxw.gzhubu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ude.c1oappe.top

[A18] 字符与 ASCII 码互转
来源：http://bvv.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://mth.iojbl.cn

PHP:  ord("A"); chr(65)
来源：http://svm.gaohongyu789.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://skk.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hcn.yvedp.cn

Java: (int) 'A'; (char) 65
来源：http://nnb.hywenlv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://udd.chenzaomai.com

Ruby: "A".ord; 65.chr
来源：http://teq.cheryme.top

C#:   (int)'A'; (char)65
来源：http://okn.aibaodan.cn

[A19] 交换两个变量
来源：http://pqs.jqgufenzy.top

Py:   a, b = b, a
来源：http://snt.zdbjq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qro.aibaodan.cn

JS:   [a, b] = [b, a];
来源：http://dcy.sxryk.cn

TS:   [a, b] = [b, a];
来源：http://ydk.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://azd.yuxming.cn

Go:   a, b = b, a
来源：http://fbv.zhijiandao.cn

Ruby: a, b = b, a
来源：http://xlo.cashguo.top

C#:   (a, b) = (b, a);
来源：http://rot.jqgfzy.top

[A20] 读取标准输入
来源：http://upb.yj20258.top

Py:   name = input("请输入：")
来源：http://quu.yj202588.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wvr.yfazqb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wbn.chenzaomai.com

TS:   // Node.js：readline 模块
来源：http://yie.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://cao.jinyuanbaomall.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://inl.jiagoushi.top

Ruby: gets.chomp
来源：http://hus.yuanzhike.top

C#:   Console.ReadLine();
来源：http://xxw.guowangkeji.top

[A21] 保留指定小数位输出
来源：http://tso.feifeiyinyue.top

Py:   f"{3.14159:.2f}"
来源：http://inb.zhiwuduotai.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mzc.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://hiw.cqqwz.cn

TS:   (3.14159).toFixed(2)
来源：http://mnj.yonumen.top

Java: String.format("%.2f", 3.14159)
来源：http://zud.9152youxi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://civ.nwbrower.top

Ruby: format("%.2f", 3.14159)
来源：http://cvn.cucudq.cn

C#:   3.14159.ToString("F2")
来源：http://dmi.kuanghao11.cn

[A22] 获取字符串长度
来源：http://xge.52xcode.cn

Py:   len(s)
来源：http://vnt.pengpengdd.cyou

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fhu.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qew.wangdashe.top

TS:   s.length
来源：http://pir.fengsongda.top

Java: s.length()
来源：http://mfw.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uwx.fzhhl.top

Ruby: s.length
来源：http://xmj.hysaishi.cn

C#:   s.Length
来源：http://yvr.pycfn.com

[A23] 大小写转换
来源：http://gaa.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://osa.jinyuanbaomall.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sed.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nfw.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://emz.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://izm.yfazqb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yhr.yuxming.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gva.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://fny.aibaodan.cn

[A24] 去除首尾空白
来源：http://kph.sysykeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bqw.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kcb.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://unl.hysaishi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qec.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zch.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://zkq.fktsv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uwg.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dvv.xuanzx.com

[A25] 字符串比较
来源：http://qai.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://cok.zhiwuduotai.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fut.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hmx.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xjq.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dcw.zhixingplan.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jmc.ppjwa.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cgi.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ewa.chenzaomai.com

[A26] 类型转换总览
来源：http://kgr.cucudq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mzn.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://leq.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vlo.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://hgq.tarul.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ywu.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://phj.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://xyo.pycfn.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vcx.gaohongyu789.top

================================================================================
来源：http://stl.xuetiantiany.cn

B. 流程控制
来源：http://nec.yueranfly.top

================================================================================
来源：http://uet.nanxinkj.top

[B01] 条件判断 if / else
来源：http://htv.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://btc.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nzf.ywan-chungtsiang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pel.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kyh.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://moa.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uzp.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lyq.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pdy.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://zmy.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nvh.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zzz.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqg.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vqh.wangdashe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mhq.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rhy.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pjw.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qiv.tian-w.cn

[B03] switch / match / case
来源：http://kdb.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kno.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://moi.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cuq.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fex.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://roi.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ilz.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fvs.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ali.nanxinkj.top

[B04] for 计数循环
来源：http://tzk.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://yxq.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://quw.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ckz.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oaf.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xmc.yuanzhike.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qgj.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://roq.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ybz.316326.xyz

[B05] 遍历数组 / 列表
来源：http://xaa.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://ddl.shanyushiyangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hfl.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bru.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://apf.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://efr.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mre.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://vwk.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ugn.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://trq.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bsa.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dlr.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://etj.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://alh.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lwo.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ywb.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://epb.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bdw.jyoumei.cn

[B07] while 循环
来源：http://tpy.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://gpx.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://wha.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://zqs.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://ekp.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://zhy.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pqj.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://irp.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://sxq.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://drf.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://jdg.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sgb.ppjwa.cn

JS:   do { i++; } while (i < 10);
来源：http://jjp.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://cyk.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://mrb.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rsd.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://wnd.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://qql.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://wnw.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://idv.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://asg.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eib.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dyw.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svo.ehwqpu.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cmb.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ibr.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sod.yongpay.top

[B10] 遍历同时拿索引
来源：http://uss.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mfq.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jbu.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nos.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nhq.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zpc.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://clt.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kva.jyoumei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hjc.hesvh.cn

[B11] 生成数字序列 / 区间
来源：http://qus.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://nzk.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://suj.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://igh.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zrv.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mem.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://thp.dashuyun.cn

Ruby: (0...10).step(2).to_a
来源：http://bkt.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cst.aizwys.cn

[B12] 跳出多层循环
来源：http://oqy.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kpx.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uxw.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rja.nwbrower.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hqq.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bmc.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eor.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lgf.birdmap.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nrw.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://abh.ppjwa.cn

Py:   isinstance(x, (int, float))
来源：http://eje.cashguo.top

PHP:  is_numeric($x)
来源：http://ebl.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qqe.jqgfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gvf.pycfn.com

Java: x instanceof Number
来源：http://qpl.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dea.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://ibu.daria6918.cn

C#:   x is int or double or decimal
来源：http://ezy.uphjek.com

[B14] 判断值是否在集合内
来源：http://msd.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://omr.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nil.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://xkk.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://jan.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cat.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ddc.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fsk.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pry.ctjpmb.com

[B15] 布尔运算与取反
来源：http://kcu.shangyingyoupin.top

Py:   a and b or not c
来源：http://abz.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://cag.ctjpmb.com

JS:   a && b || !c
来源：http://cez.smart0.xyz

TS:   a && b || !c
来源：http://ubh.iojbl.cn

Java: a && b || !c
来源：http://hwt.yj20258.top

Go:   a && b || !c
来源：http://yxr.xylfe.cn

Ruby: a && b || !c
来源：http://dgz.snrcjt.cn

C#:   a && b || !c
来源：http://ovn.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cnk.bbcook.cn

Py:   if not data: return
来源：http://dsx.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://yyd.quarkkingdee.top

JS:   if (!data) return;
来源：http://hge.jinqigfzy.top

TS:   if (!data) return;
来源：http://osa.hnxiangtu.top

Java: if (data == null) return;
来源：http://lkt.shzxlz.cn

Go:   if data == nil { return }
来源：http://qzv.tarul.cn

Ruby: return if data.nil?
来源：http://xne.chenlongwang.top

C#:   if (data == null) return;
来源：http://rlm.jiagoushi.top

================================================================================
来源：http://zge.hnqzz.top

C. 函数与作用域
来源：http://mqy.yuxming.cn

================================================================================
来源：http://mvp.nanxinkj.top

[C01] 定义函数
来源：http://qto.pycfn.com

Py:   def add(a, b): return a + b
来源：http://duv.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fwb.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://uhm.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jbq.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pqk.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://eeo.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://eua.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bqb.tianlin.xyz

[C02] 默认参数
来源：http://acq.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://iov.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://lvb.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://jtd.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bpw.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://huf.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eoq.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://urt.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://pqb.smart0.xyz

[C03] 可变参数
来源：http://drs.jqgufenzy.top

Py:   def total(*args): return sum(args)
来源：http://unc.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://trz.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvf.xylfe.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yez.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://chv.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ekg.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://vuv.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://emd.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://frv.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sia.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rrd.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mhj.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xpo.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://khx.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://sws.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://cme.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://abr.gzhubu.top

[C05] 返回多个值
来源：http://cbo.gaohongyu789.top

Py:   return a, b
来源：http://ycj.meibo888.top

PHP:  return [$a, $b];
来源：http://osb.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hah.zhoulong.xyz

TS:   return { a, b };
来源：http://uzz.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jfq.shanyushiyangkeji.top

Go:   return a, b
来源：http://xja.daria6918.cn

Ruby: return a, b
来源：http://miq.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://fkq.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://qhh.yj20258888.top

Py:   square = lambda x: x * x
来源：http://rqy.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qzx.bbcook.cn

JS:   const square = x => x * x;
来源：http://qql.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ncf.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yev.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://nfo.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://ydu.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://ntc.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://csg.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ten.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://dps.cqqwz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ulp.gaohongyu789.top

TS:   arr.map(String)
来源：http://nth.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wpc.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ppz.yueranfly.top


<!-- 参考信息 -->