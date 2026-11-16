代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dvs.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://isw.yueranfly.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cok.andypj.xyz

[A17] 位运算
来源：http://cbm.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dka.hammf.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pfj.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aqw.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uof.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tvd.jlsjyb.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bsr.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hwt.zhengqikj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eyn.chenzaomai.com

[A18] 字符与 ASCII 码互转
来源：http://qtt.iojbl.cn

Py:   ord("A"); chr(65)
来源：http://dqz.zhaomingkeji.xyz

PHP:  ord("A"); chr(65)
来源：http://pue.gotoacloud.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gck.shuidangran.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wss.ywan-chungtsiang.top

Java: (int) 'A'; (char) 65
来源：http://kqr.9152youxi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zxt.nwbrower.top

Ruby: "A".ord; 65.chr
来源：http://gxo.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://fkk.redwolf501.top

[A19] 交换两个变量
来源：http://bjm.meibo888.top

Py:   a, b = b, a
来源：http://mnh.gotoacloud.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mso.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://jba.sjlbkw.cn

TS:   [a, b] = [b, a];
来源：http://fan.pengpengdd.cyou

Java: int t = a; a = b; b = t;
来源：http://mqd.hammf.cn

Go:   a, b = b, a
来源：http://shf.shanyushiyangkeji.top

Ruby: a, b = b, a
来源：http://qsp.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://tsm.hnqzz.top

[A20] 读取标准输入
来源：http://mht.zhijiandao.cn

Py:   name = input("请输入：")
来源：http://lif.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qow.wangshuangyany.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hhi.aibaodan.cn

TS:   // Node.js：readline 模块
来源：http://cih.ybcxt.top

Java: new Scanner(System.in).nextLine()
来源：http://yfm.fzhhl.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kfk.iojbl.cn

Ruby: gets.chomp
来源：http://umv.yangfankeji.com

C#:   Console.ReadLine();
来源：http://lkj.fzhhl.top

[A21] 保留指定小数位输出
来源：http://kdm.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://lvk.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://omu.zhongyouzk.top

JS:   (3.14159).toFixed(2)
来源：http://tjh.yongpay.top

TS:   (3.14159).toFixed(2)
来源：http://dio.shanyushiyangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://fuz.quarkkingdee.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lzw.chenlongwang.top

Ruby: format("%.2f", 3.14159)
来源：http://hcy.jlsjyb.cn

C#:   3.14159.ToString("F2")
来源：http://gil.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://wti.nwbrower.top

Py:   len(s)
来源：http://rng.52xcode.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://moq.vehdjk.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jky.tianlin.xyz

TS:   s.length
来源：http://nvl.ivvv.top

Java: s.length()
来源：http://xto.jinqigfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jig.yuxming.cn

Ruby: s.length
来源：http://vko.uphjek.com

C#:   s.Length
来源：http://rlc.cucudq.cn

[A23] 大小写转换
来源：http://fxt.0kj1m.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lgi.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vpt.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hpr.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://por.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dpr.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aja.epnwcf.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://deg.birdmap.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bbz.316326.xyz

[A24] 去除首尾空白
来源：http://oil.fzhhl.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ojl.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mls.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://plq.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sao.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gkr.quarkkingdee.top

Go:   strings.TrimSpace(s)
来源：http://uch.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oqi.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ccx.jianghu66.top

[A25] 字符串比较
来源：http://kgb.birdmap.top

Py:   s1 == s2; s1 != s2
来源：http://ylc.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bcp.shangyingyoupin.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pal.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lxr.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qwz.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tvv.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gaq.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wxs.ehwqpu.com

[A26] 类型转换总览
来源：http://ncb.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://epr.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uvf.yuxming.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kjk.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://gps.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gbo.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pdd.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hfe.jqgfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kti.nwbrower.top

================================================================================
来源：http://vks.wangdashe.top

B. 流程控制
来源：http://fel.jlsjyb.cn

================================================================================
来源：http://zap.nwbrower.top

[B01] 条件判断 if / else
来源：http://bpl.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nrp.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sty.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ahd.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aei.gzhubu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fdo.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mjh.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://swi.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pir.xuanzx.com

[B02] 多分支 else if / elif
来源：http://pld.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xic.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uua.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpd.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbg.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifm.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xpk.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://deh.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bze.zhixingplan.top

[B03] switch / match / case
来源：http://dse.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dpi.0kj1m.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wei.ctjpmb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://loz.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jvg.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://def.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bsh.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oho.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zfw.xinyue.icu

[B04] for 计数循环
来源：http://hta.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://gup.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qca.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uln.yvedp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ctr.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pef.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uuy.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://fvu.jianghu66.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://onk.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://awj.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://rmd.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qlt.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yqn.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mgc.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zdu.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xna.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://ful.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://igb.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://jgd.hfpthk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://udv.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nkh.ydjk.org.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://evg.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dzy.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rvl.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gjf.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wak.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ekt.yongpay.top

[B07] while 循环
来源：http://uqt.sweek.top

Py:   while i < 10: i += 1
来源：http://jlm.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://dzv.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://tcp.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://kyl.zhiwuduotai.top

Java: while (i < 10) { i++; }
来源：http://yvj.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lla.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://nbo.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://lgj.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://tnu.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://zqm.snrcjt.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hhh.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://mzr.hongshengwenyu.top

TS:   do { i++; } while (i < 10);
来源：http://mpj.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://zdz.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mqh.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://txx.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://lsr.hysaishi.cn

[B09] break 与 continue
来源：http://vzv.daxiang520.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qqc.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://duj.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzc.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vaa.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zck.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zsy.svipenyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://prx.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lvf.cqqwz.cn

[B10] 遍历同时拿索引
来源：http://fpq.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fxx.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wve.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://spz.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pke.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://liz.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hik.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wgj.jinqigfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dqa.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://zos.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://bpl.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://bdy.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://amq.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cef.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uoc.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aff.jlsjyb.cn

Ruby: (0...10).step(2).to_a
来源：http://yzn.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wxy.bjfxy.top

[B12] 跳出多层循环
来源：http://rlb.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nfg.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sbw.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wda.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://urv.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jkx.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fsj.jlsjyb.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kgp.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vkw.52xcode.cn

[B13] 判断是否为数字
来源：http://qqh.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://wkh.ppjwa.cn

PHP:  is_numeric($x)
来源：http://wjl.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://occ.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wvm.snrcjt.cn

Java: x instanceof Number
来源：http://jfn.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://afn.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://wpc.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://zrz.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://uzf.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sbt.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rcp.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://qta.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://fjn.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qbd.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zuz.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pwg.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://skc.zdbjq.cn

[B15] 布尔运算与取反
来源：http://gzk.tianlin.xyz

Py:   a and b or not c
来源：http://tnk.yvedp.cn

PHP:  $a && $b || !$c
来源：http://bmw.yonumen.top

JS:   a && b || !c
来源：http://hkh.gotoacloud.top

TS:   a && b || !c
来源：http://lmx.tianlin.xyz

Java: a && b || !c
来源：http://pqz.shangyingyoupin.top

Go:   a && b || !c
来源：http://jal.snrcjt.cn

Ruby: a && b || !c
来源：http://iow.aibaodan.cn

C#:   a && b || !c
来源：http://gki.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://npn.ctjpmb.com

Py:   if not data: return
来源：http://fly.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://rdv.fktsv.cn

JS:   if (!data) return;
来源：http://epl.yj20258888.top

TS:   if (!data) return;
来源：http://ujn.guannengcc.top

Java: if (data == null) return;
来源：http://xso.uphjek.com

Go:   if data == nil { return }
来源：http://weo.fengsongda.top

Ruby: return if data.nil?
来源：http://ncp.pycfn.com

C#:   if (data == null) return;
来源：http://qhc.epnwcf.com

================================================================================
来源：http://bwb.zhengqikj.top

C. 函数与作用域
来源：http://fle.zdbjq.cn

================================================================================
来源：http://esh.jqgufenzy.top

[C01] 定义函数
来源：http://fvj.yj20258.top

Py:   def add(a, b): return a + b
来源：http://jda.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jfx.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://bur.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgr.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://osc.aibaodan.cn

Go:   func add(a, b int) int { return a + b }
来源：http://krx.shzxlz.cn

Ruby: def add(a, b); a + b; end
来源：http://vcp.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yrs.cdnleiting.top

[C02] 默认参数
来源：http://rui.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://iey.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ajp.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://zfb.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://thl.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rft.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://elq.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://qcl.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://fxa.zdbjq.cn

[C03] 可变参数
来源：http://krc.xylfe.cn

Py:   def total(*args): return sum(args)
来源：http://fkn.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ybc.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wib.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jgs.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xxf.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cxj.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://tym.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dib.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://orf.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qgb.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ofs.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hhl.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qwt.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://nhm.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://suw.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://irk.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://whx.sufxvd.cn

[C05] 返回多个值
来源：http://xkf.hammf.cn

Py:   return a, b
来源：http://ect.xylfe.cn

PHP:  return [$a, $b];
来源：http://fum.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://krh.xuetiantiany.cn

TS:   return { a, b };
来源：http://jia.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qsf.cashguo.top

Go:   return a, b
来源：http://ayl.xuanzx.com

Ruby: return a, b
来源：http://dmf.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://ghz.yonumen.top

[C06] 匿名函数 / lambda
来源：http://yot.nwbrower.top

Py:   square = lambda x: x * x
来源：http://gik.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://syi.daxiang520.top

JS:   const square = x => x * x;
来源：http://wyk.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://zhm.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tkl.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lok.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://com.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://ijk.316326.xyz

[C07] 把函数作为参数传入
来源：http://ufh.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qcc.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xmt.ivvv.top


<!-- 参考信息 -->