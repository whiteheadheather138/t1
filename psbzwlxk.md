代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://las.sxryk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dgm.epnwcf.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qar.aibaodan.cn

[A17] 位运算
来源：http://upg.fzhhl.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://etj.hfpthk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ggo.hcnkem.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yra.andypj.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nxl.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cgk.yvedp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gmp.andypj.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iiy.yuanzhike.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nkz.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://fxp.nanxuanxn.top

Py:   ord("A"); chr(65)
来源：http://can.ywan-chungtsiang.top

PHP:  ord("A"); chr(65)
来源：http://nym.xingfuxueyuan.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qas.pengpengdd.cyou

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oxh.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://ejs.fanxiaobao.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mms.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://jmy.ivvv.top

C#:   (int)'A'; (char)65
来源：http://zln.yangfankeji.com

[A19] 交换两个变量
来源：http://emo.xziqi.cn

Py:   a, b = b, a
来源：http://pqo.hnqzz.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qcu.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://nyh.jqgfzy.top

TS:   [a, b] = [b, a];
来源：http://uuj.zdbjq.cn

Java: int t = a; a = b; b = t;
来源：http://fwz.svipenyu.cn

Go:   a, b = b, a
来源：http://eze.guannengcc.top

Ruby: a, b = b, a
来源：http://xiw.havefunace.top

C#:   (a, b) = (b, a);
来源：http://upx.zhaomingkeji.xyz

[A20] 读取标准输入
来源：http://god.sxryk.cn

Py:   name = input("请输入：")
来源：http://kzy.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://yrb.yfazqb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://czw.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://qcb.zhiwuduotai.top

Java: new Scanner(System.in).nextLine()
来源：http://ycv.daxiang520.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ydw.cucudq.cn

Ruby: gets.chomp
来源：http://lot.zdbjq.cn

C#:   Console.ReadLine();
来源：http://epl.jinyuanbaomall.cn

[A21] 保留指定小数位输出
来源：http://cbl.hfpthk.cn

Py:   f"{3.14159:.2f}"
来源：http://oek.zhaomingkeji.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kqm.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://api.316326.xyz

TS:   (3.14159).toFixed(2)
来源：http://pjq.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://zqg.andypj.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jvs.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://iyn.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://ymd.jianghu66.top

[A22] 获取字符串长度
来源：http://sxs.yj202588.top

Py:   len(s)
来源：http://nop.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lim.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vje.dashuyun.cn

TS:   s.length
来源：http://hfg.xinyue.icu

Java: s.length()
来源：http://oho.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jij.hysaishi.cn

Ruby: s.length
来源：http://kon.jianghu66.top

C#:   s.Length
来源：http://dwo.yj20258.top

[A23] 大小写转换
来源：http://njf.yfazqb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://vtg.jinqigufen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jxj.yuanzhike.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wyp.daxiang520.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cmd.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lyg.yangfankeji.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qpj.redwolf501.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zvy.hesvh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bmj.cucudq.cn

[A24] 去除首尾空白
来源：http://mft.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pmt.guowangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tso.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://npk.vqdsnc.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lnn.haohaochexian.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vid.xuetiantiany.cn

Go:   strings.TrimSpace(s)
来源：http://btm.snrcjt.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yki.fanxiaobao.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lso.zhoulong.xyz

[A25] 字符串比较
来源：http://oah.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://nst.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ucn.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ziy.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wyc.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nrk.hysaishi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://igg.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dnk.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jjy.nwbrower.top

[A26] 类型转换总览
来源：http://nhl.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lan.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ysg.gaohongyu789.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gci.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://fao.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://afc.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lqj.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://zod.uphjek.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mcr.gaohongyu789.top

================================================================================
来源：http://yai.jinyuanbaomall.cn

B. 流程控制
来源：http://bhy.hnxiangtu.top

================================================================================
来源：http://ipp.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://tst.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qbf.hnqzz.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vty.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://avy.gzhubu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zjy.nwbrower.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jgu.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://djs.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://glh.nanxuanxn.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jwt.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://txu.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://clh.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vsk.jinghuilouyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://koi.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://whd.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hld.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mav.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sag.nanxuanxn.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfq.pengpengdd.cyou

[B03] switch / match / case
来源：http://kwe.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mon.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rtn.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yff.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zvz.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cvn.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zjw.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xkl.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cdp.bjfxy.top

[B04] for 计数循环
来源：http://rrs.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://phe.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bhz.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://beg.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://awr.ydzc1.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jjo.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jex.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://knn.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gmx.cashguo.top

[B05] 遍历数组 / 列表
来源：http://oxb.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://ztv.hammf.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wgg.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tzr.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://knn.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ohx.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nqg.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://tmx.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bza.sweek.top

[B06] 遍历字典 / 对象
来源：http://fen.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ytk.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fjq.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uqv.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rgw.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bhm.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nkc.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ncs.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ecz.vqdsnc.cn

[B07] while 循环
来源：http://gzq.gotoacloud.top

Py:   while i < 10: i += 1
来源：http://lju.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://itp.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://obi.quarkkingdee.top

TS:   while (i < 10) { i++; }
来源：http://hwh.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://tpt.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ppj.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://iol.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://mna.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://thg.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://jsr.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://cjg.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://fpz.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://uhg.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://lkz.zhoulong.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ske.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://ybs.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://keo.hesvh.cn

[B09] break 与 continue
来源：http://zan.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ixj.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sgj.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqj.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yah.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nho.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cyw.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vvj.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxk.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://zrr.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ahn.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://our.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ppw.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://exi.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fpd.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bue.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ghm.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zdb.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://zrg.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://thm.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://ulj.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mbs.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vlz.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sqs.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dlh.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://cwu.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ltr.aibaodan.cn

[B12] 跳出多层循环
来源：http://wsn.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://zag.jinghuilouyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cbj.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uav.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fzl.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gbq.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://okh.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bpu.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gwk.9152youxi.cn

[B13] 判断是否为数字
来源：http://wrg.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://wkp.snrcjt.cn

PHP:  is_numeric($x)
来源：http://gqk.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dig.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wmj.zycfv.cn

Java: x instanceof Number
来源：http://dqk.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mtq.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://ppg.0kj1m.cn

C#:   x is int or double or decimal
来源：http://zfo.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://wel.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://erh.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pjw.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://bak.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://bml.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vss.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oxn.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://vyy.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://exo.birdmap.top

[B15] 布尔运算与取反
来源：http://ylm.cucudq.cn

Py:   a and b or not c
来源：http://tcb.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://zye.yangfankeji.com

JS:   a && b || !c
来源：http://xpc.yangfankeji.com

TS:   a && b || !c
来源：http://fdu.jinyuanbaomall.cn

Java: a && b || !c
来源：http://qjt.dianchejie.cn

Go:   a && b || !c
来源：http://cjw.hongshengwenyu.top

Ruby: a && b || !c
来源：http://jqa.feifeiyinyue.top

C#:   a && b || !c
来源：http://ojg.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ubd.shzxlz.cn

Py:   if not data: return
来源：http://fgu.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://ian.aizwys.cn

JS:   if (!data) return;
来源：http://zji.zhiwuduotai.top

TS:   if (!data) return;
来源：http://odj.yanxiufei.cn

Java: if (data == null) return;
来源：http://coy.uphjek.com

Go:   if data == nil { return }
来源：http://tzo.xylfe.cn

Ruby: return if data.nil?
来源：http://ruz.ywan-chungtsiang.top

C#:   if (data == null) return;
来源：http://frz.0kj1m.cn

================================================================================
来源：http://nqo.jinghuilouyu.cn

C. 函数与作用域
来源：http://chn.smart0.xyz

================================================================================
来源：http://bep.316326.xyz

[C01] 定义函数
来源：http://tut.316326.xyz

Py:   def add(a, b): return a + b
来源：http://gop.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cfm.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ttw.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvp.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://osf.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://nvy.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://ygr.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nhm.nanxuanxn.top

[C02] 默认参数
来源：http://lku.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://liv.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aqq.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://dlo.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cmh.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wql.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bxu.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://vze.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://njs.aibaodan.cn

[C03] 可变参数
来源：http://kor.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://brd.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rqk.ybcxt.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zcx.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wzj.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pgf.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zuk.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://mcm.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ubx.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://cmq.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eqn.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oxd.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ezn.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kqy.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://oks.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://zvr.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://mmb.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://fpa.quarkkingdee.top

[C05] 返回多个值
来源：http://cwh.shanyushiyangkeji.top

Py:   return a, b
来源：http://adi.iojbl.cn

PHP:  return [$a, $b];
来源：http://kym.yj20258888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qnz.wangshuangyany.cn

TS:   return { a, b };
来源：http://lua.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nyw.vehdjk.com

Go:   return a, b
来源：http://mbz.fzhhl.top

Ruby: return a, b
来源：http://ydv.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://wgk.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://ydu.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://afm.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wtp.snrcjt.cn

JS:   const square = x => x * x;
来源：http://gzj.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://eta.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zih.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://mmg.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://odn.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://sxg.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://psr.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xes.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://enx.shzxlz.cn


<!-- 参考信息 -->