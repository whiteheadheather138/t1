代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://otp.xziqi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dja.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sgo.vqdsnc.cn

[A17] 位运算
来源：http://trc.uphjek.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sap.andypj.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nas.jyoumei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lpw.bjfxy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://unl.gzhubu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://plp.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jat.gaohongyu789.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kom.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bgj.ydzc1.top

[A18] 字符与 ASCII 码互转
来源：http://vwi.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://yrb.yanxiufei.cn

PHP:  ord("A"); chr(65)
来源：http://via.yfazqb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wku.tarul.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kkn.xinyue.icu

Java: (int) 'A'; (char) 65
来源：http://vdk.ehwqpu.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ctk.52xcode.cn

Ruby: "A".ord; 65.chr
来源：http://xsr.xinyue.icu

C#:   (int)'A'; (char)65
来源：http://iqt.dashuyun.cn

[A19] 交换两个变量
来源：http://yhq.feifeiyinyue.top

Py:   a, b = b, a
来源：http://gpa.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xyx.hywenlv.cn

JS:   [a, b] = [b, a];
来源：http://rfh.hysaishi.cn

TS:   [a, b] = [b, a];
来源：http://vnm.shuidangran.top

Java: int t = a; a = b; b = t;
来源：http://ttm.dianchejie.cn

Go:   a, b = b, a
来源：http://dea.havefunace.top

Ruby: a, b = b, a
来源：http://ofh.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://few.fehbvm.com

[A20] 读取标准输入
来源：http://scs.jinqigufen.top

Py:   name = input("请输入：")
来源：http://ssk.yvedp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pfi.jiagoushi.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mox.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://dqo.aizwys.cn

Java: new Scanner(System.in).nextLine()
来源：http://dfh.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fej.xinyue.icu

Ruby: gets.chomp
来源：http://nbp.meibo888.top

C#:   Console.ReadLine();
来源：http://soz.xuanzx.com

[A21] 保留指定小数位输出
来源：http://gnw.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://zeq.jinqigufen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hed.shzxlz.cn

JS:   (3.14159).toFixed(2)
来源：http://kie.pycfn.com

TS:   (3.14159).toFixed(2)
来源：http://zwn.yvedp.cn

Java: String.format("%.2f", 3.14159)
来源：http://mvj.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://btt.redwolf501.top

Ruby: format("%.2f", 3.14159)
来源：http://hgz.ybcxt.top

C#:   3.14159.ToString("F2")
来源：http://gao.jlsjyb.cn

[A22] 获取字符串长度
来源：http://rim.iojbl.cn

Py:   len(s)
来源：http://qfx.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://quv.jinqigfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hzd.feifeiyinyue.top

TS:   s.length
来源：http://jav.xylfe.cn

Java: s.length()
来源：http://hru.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hhy.smart0.xyz

Ruby: s.length
来源：http://gsz.yj20258888.top

C#:   s.Length
来源：http://rlw.yongpay.top

[A23] 大小写转换
来源：http://kom.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jsv.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rhr.uphjek.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qyp.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://miv.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kvw.dashuyun.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sub.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hzr.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ara.fengsongda.top

[A24] 去除首尾空白
来源：http://bnk.yvedp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qnq.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fya.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ekr.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wxo.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blj.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://hvy.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cxb.dianchejie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gqu.cucudq.cn

[A25] 字符串比较
来源：http://qbi.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://bsr.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://myy.havefunace.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nkj.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kiu.uphjek.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pel.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cwl.birdmap.top

Ruby: s1 == s2; s1 <=> s2
来源：http://iku.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://khf.andypj.xyz

[A26] 类型转换总览
来源：http://leq.uphjek.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yit.ywan-chungtsiang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fcm.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iwv.sweek.top

TS:   Number() String() Boolean() x as number
来源：http://noz.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kxr.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jrx.xziqi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pra.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zcd.fzhhl.top

================================================================================
来源：http://rez.daxiang520.top

B. 流程控制
来源：http://tls.yuxming.cn

================================================================================
来源：http://gdo.hesvh.cn

[B01] 条件判断 if / else
来源：http://jja.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jfb.yangfankeji.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cgq.iojbl.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gbm.wangdashe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vnq.tarul.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iez.yuxming.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mby.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wio.zhiwuduotai.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rbl.shuidangran.top

[B02] 多分支 else if / elif
来源：http://jfy.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bfh.fehbvm.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bjs.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tte.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pzy.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bst.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://okp.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fcr.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ejd.vehdjk.com

[B03] switch / match / case
来源：http://ekl.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cnr.wangdashe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nyz.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://trq.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vsc.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yhv.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://znz.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zwo.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://meg.shangyingyoupin.top

[B04] for 计数循环
来源：http://jps.tarul.cn

Py:   for i in range(10): print(i)
来源：http://sve.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ccr.gotoacloud.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://igl.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mat.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kss.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uuy.birdmap.top

Ruby: 10.times { |i| puts i }
来源：http://zvh.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xwa.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://ogl.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://lzr.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hzt.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nio.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lud.fanxiaobao.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://yxy.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dnk.nanxuanxn.top

Ruby: arr.each { |item| puts item }
来源：http://snx.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dev.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://nmf.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rec.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://izc.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dxy.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tip.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dcv.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vwl.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://syk.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dqh.havefunace.top

[B07] while 循环
来源：http://mlo.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://rgy.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://itg.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://vvy.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://wks.hammf.cn

Java: while (i < 10) { i++; }
来源：http://xhv.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rqs.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://hqi.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://wbp.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://hng.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://lol.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sqz.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://tco.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://ujm.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://yiy.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nzh.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://lll.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://cek.yfazqb.com

[B09] break 与 continue
来源：http://otc.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ert.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nry.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nml.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iws.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ken.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pee.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ycq.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsw.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://sso.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rwh.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://umi.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lba.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hqm.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bpc.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pvn.jinqigfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://clk.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xkh.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://rbl.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://pqt.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://ljj.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nsm.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tzt.fktsv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xkt.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tit.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://aij.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ywl.hnxiangtu.top

[B12] 跳出多层循环
来源：http://wxp.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xkt.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://kkp.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mbl.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ydj.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lvi.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wcg.gzhubu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uyc.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bme.cheryme.top

[B13] 判断是否为数字
来源：http://twe.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://zkr.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://mgb.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rkl.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://omy.jyoumei.cn

Java: x instanceof Number
来源：http://swv.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wow.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://agx.gogol.net.cn

C#:   x is int or double or decimal
来源：http://qsj.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://fnh.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://amo.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cwg.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://drv.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://rha.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mna.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mra.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rre.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rew.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://wlg.ybcxt.top

Py:   a and b or not c
来源：http://dms.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://jic.jqgufenzy.top

JS:   a && b || !c
来源：http://zdl.xuanzx.com

TS:   a && b || !c
来源：http://lcy.fanxiaobao.xyz

Java: a && b || !c
来源：http://mqb.uphjek.com

Go:   a && b || !c
来源：http://jkf.sjlbkw.cn

Ruby: a && b || !c
来源：http://ulg.zdqjudy.top

C#:   a && b || !c
来源：http://rmf.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://xuz.yuanzhike.top

Py:   if not data: return
来源：http://iqg.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://bga.zhongyouzk.top

JS:   if (!data) return;
来源：http://lwf.yongpay.top

TS:   if (!data) return;
来源：http://piy.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://xwz.sjlbkw.cn

Go:   if data == nil { return }
来源：http://djv.zhoulong.xyz

Ruby: return if data.nil?
来源：http://yej.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://sxg.xuetiantiany.cn

================================================================================
来源：http://ogv.zdqjudy.top

C. 函数与作用域
来源：http://wzi.chenjidiqi.icu

================================================================================
来源：http://tki.ctjpmb.com

[C01] 定义函数
来源：http://hxr.cashguo.top

Py:   def add(a, b): return a + b
来源：http://oap.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cmc.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://dgm.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qal.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jgj.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kxr.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://izp.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kou.ivvv.top

[C02] 默认参数
来源：http://xgo.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://jqy.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ueg.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://gwr.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://lbs.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://skt.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zos.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://ddd.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://idv.gotoacloud.top

[C03] 可变参数
来源：http://yxr.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://mrx.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rfg.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bjd.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nkk.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jhn.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rhb.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://xod.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ddw.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://gvu.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mca.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ddx.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://opz.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://exa.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://khz.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://qdf.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://ztc.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://fro.jiagoushi.top

[C05] 返回多个值
来源：http://wvs.hcnkem.com

Py:   return a, b
来源：http://jyj.zhiwuduotai.top

PHP:  return [$a, $b];
来源：http://lym.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ebs.hywenlv.cn

TS:   return { a, b };
来源：http://csg.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rkv.kuanghao11.cn

Go:   return a, b
来源：http://jwa.hnxiangtu.top

Ruby: return a, b
来源：http://uyu.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://oyp.svipenyu.cn

[C06] 匿名函数 / lambda
来源：http://puv.yuxming.cn

Py:   square = lambda x: x * x
来源：http://jmg.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lfx.jqgfzy.top

JS:   const square = x => x * x;
来源：http://ozd.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://kxu.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://faj.cqqwz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gjw.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://dcr.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cuu.ivvv.top

[C07] 把函数作为参数传入
来源：http://fwc.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mno.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://gwp.ehwqpu.com


<!-- 参考信息 -->