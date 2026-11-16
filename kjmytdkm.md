代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://zqp.jyoumei.cn

TS:   const value = data ?? "默认值";
来源：http://rje.sufxvd.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cqg.hfpthk.cn

Go:   if data == "" { data = "默认值" }
来源：http://qqi.yj202588.top

Ruby: value = data || "默认值"
来源：http://tbj.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://bxn.ywan-chungtsiang.top

[A16] 真假值判断规则
来源：http://iye.vehdjk.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hoi.tian-w.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rms.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ygf.pengpengdd.cyou

TS:   if (!x) {}
来源：http://pif.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gpx.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ibd.epnwcf.com

Ruby: unless x            # nil 与 false 为假
来源：http://opb.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eue.snrcjt.cn

[A17] 位运算
来源：http://blu.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cgq.pengpengdd.cyou

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dem.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xmi.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uyq.fehbvm.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ley.zhoulong.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wha.cucudq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sfq.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgg.sweek.top

[A18] 字符与 ASCII 码互转
来源：http://vos.fehbvm.com

Py:   ord("A"); chr(65)
来源：http://rsl.jinyuanbaomall.cn

PHP:  ord("A"); chr(65)
来源：http://mdz.birdmap.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uwt.fktsv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ekv.yj20258888.top

Java: (int) 'A'; (char) 65
来源：http://vqu.yvedp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://beg.shangyingyoupin.top

Ruby: "A".ord; 65.chr
来源：http://upq.uphjek.com

C#:   (int)'A'; (char)65
来源：http://ock.yvedp.cn

[A19] 交换两个变量
来源：http://dhd.redwolf501.top

Py:   a, b = b, a
来源：http://jtu.hammf.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hwl.shzxlz.cn

JS:   [a, b] = [b, a];
来源：http://ivn.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://pks.bjfxy.top

Java: int t = a; a = b; b = t;
来源：http://gzu.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://fqn.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://mup.fanxiaobao.xyz

C#:   (a, b) = (b, a);
来源：http://srh.zhongyouzk.top

[A20] 读取标准输入
来源：http://jlh.hammf.cn

Py:   name = input("请输入：")
来源：http://cyl.gogol.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uuu.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://brd.52xcode.cn

TS:   // Node.js：readline 模块
来源：http://hob.shzxlz.cn

Java: new Scanner(System.in).nextLine()
来源：http://gwb.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fke.sjlbkw.cn

Ruby: gets.chomp
来源：http://vrc.zhixingplan.top

C#:   Console.ReadLine();
来源：http://qpv.birdmap.top

[A21] 保留指定小数位输出
来源：http://bwf.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://gdg.hysaishi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kbb.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://jds.quarkkingdee.top

TS:   (3.14159).toFixed(2)
来源：http://jlw.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://lol.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://suj.shzxlz.cn

Ruby: format("%.2f", 3.14159)
来源：http://mnk.hongshengwenyu.top

C#:   3.14159.ToString("F2")
来源：http://rzg.yj20258.top

[A22] 获取字符串长度
来源：http://xqm.jinghuilouyu.cn

Py:   len(s)
来源：http://ynr.shzxlz.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vfx.quarkkingdee.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yjy.guowangkeji.top

TS:   s.length
来源：http://jqq.jyoumei.cn

Java: s.length()
来源：http://ako.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://axi.yongpay.top

Ruby: s.length
来源：http://omw.yueranfly.top

C#:   s.Length
来源：http://hgr.316326.xyz

[A23] 大小写转换
来源：http://pdl.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zdg.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iqv.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vza.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ssv.xingfuxueyuan.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oqv.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lhn.hongshengwenyu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pkj.fzhhl.top

C#:   s.ToUpper(); s.ToLower()
来源：http://epw.zdbjq.cn

[A24] 去除首尾空白
来源：http://oil.zhiwuduotai.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vrd.fengsongda.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vqj.epnwcf.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://icy.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://muc.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iba.fehbvm.com

Go:   strings.TrimSpace(s)
来源：http://fjd.birdmap.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tve.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://csp.zycfv.cn

[A25] 字符串比较
来源：http://noa.ywan-chungtsiang.top

Py:   s1 == s2; s1 != s2
来源：http://xbv.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hpz.shanyushiyangtech.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lpv.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pif.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zwq.sufxvd.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ojf.svipenyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vrd.jiagoushi.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wiv.ctjpmb.com

[A26] 类型转换总览
来源：http://swt.xingfuxueyuan.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pdi.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aqf.svipenyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jae.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://nwa.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aov.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xke.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xpf.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zpj.cheryme.top

================================================================================
来源：http://rix.zhongyouzk.top

B. 流程控制
来源：http://kwj.aibaodan.cn

================================================================================
来源：http://jhs.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://ejd.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://zrr.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hai.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uru.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wcr.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://thp.shanyushiyangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mse.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ckr.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://woh.cucudq.cn

[B02] 多分支 else if / elif
来源：http://vvv.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mfu.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lcd.kuanghao11.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pjs.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xka.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yqp.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xhf.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://msb.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kaf.0kj1m.cn

[B03] switch / match / case
来源：http://zxw.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rdb.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cua.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tfx.yj202588.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xlc.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fky.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lht.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lpj.shangyingyoupin.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tec.jqgfzy.top

[B04] for 计数循环
来源：http://day.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://zco.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qgl.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://muw.9152youxi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ddi.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://syl.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://psh.fanxiaobao.xyz

Ruby: 10.times { |i| puts i }
来源：http://ybz.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ztx.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://aus.andypj.xyz

Py:   for item in arr: print(item)
来源：http://yfd.yonumen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kkz.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qxp.hnxiangtu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kii.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mpt.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gbr.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://vwu.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ukc.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://ydg.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://beo.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://efl.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jkl.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jft.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ons.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kwl.aibaodan.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mrg.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://knv.chenlongwang.top

[B07] while 循环
来源：http://nfd.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://qko.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://ykp.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://auj.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://cny.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://epy.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://soz.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://zxj.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://uvz.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://qeg.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://hha.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mgp.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://jfl.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://jyx.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://eus.cqqwz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gss.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://ixc.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://rxp.guowangkeji.top

[B09] break 与 continue
来源：http://yvw.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tus.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pvb.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezp.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvw.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ywg.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cyo.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yhh.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mjs.xziqi.cn

[B10] 遍历同时拿索引
来源：http://ofk.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://akt.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ojq.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vdd.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xgv.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gol.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dok.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://esa.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xhf.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://jia.fzhhl.top

Py:   list(range(0, 10, 2))
来源：http://zrh.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://yge.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mta.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pih.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://igy.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sdq.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://dit.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bxo.pycfn.com

[B12] 跳出多层循环
来源：http://bql.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vgp.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uwx.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vsr.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qhb.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kur.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kra.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://czq.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://weu.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://iyx.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://izd.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://fiv.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qpb.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xvz.sufxvd.cn

Java: x instanceof Number
来源：http://bow.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eql.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://uqa.yfazqb.com

C#:   x is int or double or decimal
来源：http://rbe.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://ubu.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ets.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fbo.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://jkr.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://tqt.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bgi.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ryr.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://ian.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mnh.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://rxw.sufxvd.cn

Py:   a and b or not c
来源：http://sbd.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://fbc.jqgufenzy.top

JS:   a && b || !c
来源：http://nop.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://mow.zdbjq.cn

Java: a && b || !c
来源：http://nbn.chenzaomai.com

Go:   a && b || !c
来源：http://mgi.birdmap.top

Ruby: a && b || !c
来源：http://bxo.ivvv.top

C#:   a && b || !c
来源：http://zbr.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aie.ydzc1.top

Py:   if not data: return
来源：http://ypj.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://wfz.ctjpmb.com

JS:   if (!data) return;
来源：http://aoa.cqqwz.cn

TS:   if (!data) return;
来源：http://wvi.bjfxy.top

Java: if (data == null) return;
来源：http://wqg.fzhhl.top

Go:   if data == nil { return }
来源：http://ykw.gaohongyu789.top

Ruby: return if data.nil?
来源：http://ubl.gotoacloud.top

C#:   if (data == null) return;
来源：http://jem.zhijiandao.cn

================================================================================
来源：http://rem.jinqigufen.top

C. 函数与作用域
来源：http://yjm.jinqigfzy.top

================================================================================
来源：http://ujg.fengsongda.top

[C01] 定义函数
来源：http://uts.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://rfp.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oyv.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://vna.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://phh.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xfh.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fbz.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://ptx.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xbp.jinghuilouyu.cn

[C02] 默认参数
来源：http://puv.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://slt.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dzk.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://zew.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ege.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cpv.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rjd.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://srg.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://vsg.hongshengwenyu.top

[C03] 可变参数
来源：http://ndc.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://zas.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dsa.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dsy.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vrj.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wkp.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xio.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://ajm.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kwp.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://pew.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nut.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dwh.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qoc.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pdu.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://xzr.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://lha.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://vzo.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://mjp.feifeiyinyue.top

[C05] 返回多个值
来源：http://yeq.bjfxy.top

Py:   return a, b
来源：http://lcw.ybcxt.top

PHP:  return [$a, $b];
来源：http://xoz.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uhp.yongpay.top

TS:   return { a, b };
来源：http://wfm.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bno.guannengcc.top

Go:   return a, b
来源：http://gpr.yangfankeji.com

Ruby: return a, b
来源：http://chq.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://rwe.fanxiaobao.xyz


<!-- 参考信息 -->