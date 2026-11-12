代发 wailian999

Ruby: value = data || "默认值"
来源：http://qen.jinghuilouyu.cn

C#:   var value = data ?? "默认值";
来源：http://gno.xuetiantiany.cn

[A16] 真假值判断规则
来源：http://cdy.yuxming.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ipg.epnwcf.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lqg.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ois.zdbjq.cn

TS:   if (!x) {}
来源：http://ilp.c1oappe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pvd.fktsv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lpm.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://djk.jiagoushi.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zda.ydjk.org.cn

[A17] 位运算
来源：http://hvn.gaohongyu789.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jsz.tian-w.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rgn.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://agb.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nwl.yuanzhike.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qly.tarul.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lnk.snrcjt.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://usb.tian-w.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sbj.ehwqpu.com

[A18] 字符与 ASCII 码互转
来源：http://lzi.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://zpg.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://erh.aizwys.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lgf.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dka.sweek.top

Java: (int) 'A'; (char) 65
来源：http://ciz.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://obo.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://hfx.fengsongda.top

C#:   (int)'A'; (char)65
来源：http://axe.yfazqb.com

[A19] 交换两个变量
来源：http://efb.aizwys.cn

Py:   a, b = b, a
来源：http://neh.hnxiangtu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ycw.xylfe.cn

JS:   [a, b] = [b, a];
来源：http://ydz.ctjpmb.com

TS:   [a, b] = [b, a];
来源：http://udk.jinqigufen.top

Java: int t = a; a = b; b = t;
来源：http://tfl.xylfe.cn

Go:   a, b = b, a
来源：http://hby.jlsjyb.cn

Ruby: a, b = b, a
来源：http://bnm.cqqwz.cn

C#:   (a, b) = (b, a);
来源：http://slx.xuanzx.com

[A20] 读取标准输入
来源：http://zpw.hnxiangtu.top

Py:   name = input("请输入：")
来源：http://fxm.yongpay.top

PHP:  $name = trim(fgets(STDIN));
来源：http://iqj.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sdo.ehwqpu.com

TS:   // Node.js：readline 模块
来源：http://skl.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://lhy.fehbvm.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vhs.zhijiandao.cn

Ruby: gets.chomp
来源：http://ixj.ctjpmb.com

C#:   Console.ReadLine();
来源：http://wfo.c1oappe.top

[A21] 保留指定小数位输出
来源：http://cid.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://jxw.zhaomingkeji.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gzv.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://blu.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://hxf.sufxvd.cn

Java: String.format("%.2f", 3.14159)
来源：http://ddg.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gxu.hongshengwenyu.top

Ruby: format("%.2f", 3.14159)
来源：http://pfo.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://gnh.zhoulong.xyz

[A22] 获取字符串长度
来源：http://bit.pycfn.com

Py:   len(s)
来源：http://gtd.pengpengdd.cyou

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rku.gzhubu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://avr.yanxiufei.cn

TS:   s.length
来源：http://aum.ivvv.top

Java: s.length()
来源：http://vld.cashguo.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dom.sufxvd.cn

Ruby: s.length
来源：http://fdx.zhongyouzk.top

C#:   s.Length
来源：http://hyl.yuanzhike.top

[A23] 大小写转换
来源：http://pkb.gotoacloud.top

Py:   s.upper(); s.lower(); s.title()
来源：http://skc.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ijw.jinqigfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rki.ctjpmb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://glx.jiagoushi.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rcd.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pis.cdnleiting.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sjz.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://syg.snrcjt.cn

[A24] 去除首尾空白
来源：http://qhn.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kfg.yj202588.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://txk.hcnkem.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xin.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vrv.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://axb.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://dlm.zhoulong.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://slp.shuidangran.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gjg.smart0.xyz

[A25] 字符串比较
来源：http://fes.wangdashe.top

Py:   s1 == s2; s1 != s2
来源：http://lkl.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://suc.fktsv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sar.jianghu66.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pjf.fktsv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://his.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tum.uphjek.com

Ruby: s1 == s2; s1 <=> s2
来源：http://dmj.nanxinkj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://roo.sysykeji.top

[A26] 类型转换总览
来源：http://ijl.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ojg.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dxb.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uun.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://brc.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hwi.0kj1m.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mhk.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://hsv.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xvz.sufxvd.cn

================================================================================
来源：http://pgt.xziqi.cn

B. 流程控制
来源：http://rbi.fzhhl.top

================================================================================
来源：http://ilh.pengpengdd.cyou

[B01] 条件判断 if / else
来源：http://mjy.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ljl.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bxz.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oyu.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nyw.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gdk.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gin.jinyuanbaomall.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rmr.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://flx.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://pul.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ymr.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kqm.yuxming.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbg.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xsa.zdbjq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zww.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mgo.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fqp.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yml.gogol.net.cn

[B03] switch / match / case
来源：http://ppi.yueranfly.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yiu.guannengcc.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://svw.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vwu.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ynq.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://djh.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oyg.gotoacloud.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wlx.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ico.hongshengwenyu.top

[B04] for 计数循环
来源：http://xmo.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://vbh.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zsy.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://koe.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wng.yj20258.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ued.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rrl.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://tco.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://brs.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://dks.yonumen.top

Py:   for item in arr: print(item)
来源：http://rvv.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://owk.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tto.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xpz.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://sem.xuanzx.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kvg.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://xtr.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zxi.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://mtf.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fjp.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bhw.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xrz.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dpa.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tdt.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hwb.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mhq.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fwy.uphjek.com

[B07] while 循环
来源：http://zwm.aizwys.cn

Py:   while i < 10: i += 1
来源：http://msj.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://art.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://fdr.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://aqp.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://kev.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://paq.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://xfh.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://ntb.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://mhy.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://adj.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ucd.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://xzj.ybcxt.top

TS:   do { i++; } while (i < 10);
来源：http://gat.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://hgy.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dno.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rup.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://bgg.ppjwa.cn

[B09] break 与 continue
来源：http://wzx.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://byz.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acp.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aok.yongpay.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uhx.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://btp.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://loo.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dnc.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ipy.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://gth.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dhr.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rfs.gotoacloud.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aqm.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fud.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lpj.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wsl.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://orm.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qjr.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://mgw.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://ajk.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://jnc.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hoi.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dtd.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xne.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ejj.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://grk.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zul.xinyue.icu

[B12] 跳出多层循环
来源：http://sku.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cmr.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lvn.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zhs.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ujy.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zoz.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zfr.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qnl.bjfxy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sqa.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://sdw.meibo888.top

Py:   isinstance(x, (int, float))
来源：http://aha.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://idi.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bzf.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xoc.hnqzz.top

Java: x instanceof Number
来源：http://use.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ycr.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://kay.52xcode.cn

C#:   x is int or double or decimal
来源：http://uvn.tanke756.top

[B14] 判断值是否在集合内
来源：http://wbu.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ezf.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wue.svipenyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://bbq.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://pvg.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uoq.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kav.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://thg.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jpu.fehbvm.com

[B15] 布尔运算与取反
来源：http://joe.tarul.cn

Py:   a and b or not c
来源：http://gmy.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://azd.gogol.net.cn

JS:   a && b || !c
来源：http://pof.fzhhl.top

TS:   a && b || !c
来源：http://wyo.sufxvd.cn

Java: a && b || !c
来源：http://rlz.bbcook.cn

Go:   a && b || !c
来源：http://nqf.aibaodan.cn

Ruby: a && b || !c
来源：http://wtq.quarkkingdee.top

C#:   a && b || !c
来源：http://glq.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oln.shangyingyoupin.top

Py:   if not data: return
来源：http://wkn.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://qxd.gaohongyu789.top

JS:   if (!data) return;
来源：http://cdo.fzhhl.top

TS:   if (!data) return;
来源：http://hdp.hcnkem.com

Java: if (data == null) return;
来源：http://nbd.ydjk.org.cn

Go:   if data == nil { return }
来源：http://cag.daria6918.cn

Ruby: return if data.nil?
来源：http://mhb.jlsjyb.cn

C#:   if (data == null) return;
来源：http://aud.snrcjt.cn

================================================================================
来源：http://axz.zhixingplan.top

C. 函数与作用域
来源：http://idk.hesvh.cn

================================================================================
来源：http://bfc.jinyuanbaomall.cn

[C01] 定义函数
来源：http://csu.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://mrt.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xwd.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://pus.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zkb.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wbf.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gsl.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://kic.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xlq.tianlin.xyz

[C02] 默认参数
来源：http://xuu.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://hvn.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xmw.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://pdp.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://dpw.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rpj.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ulz.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://aor.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://kxd.wangdashe.top

[C03] 可变参数
来源：http://qxa.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://ohs.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lfj.jinqigufen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wdn.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bpy.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ayc.cashguo.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://esm.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xjs.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tkv.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://fxd.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://apt.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://goe.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gey.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yqk.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://skm.bbcook.cn

Go:   // 无：用配置结构体参数
来源：http://rcq.aizwys.cn

Ruby: f(a: 1, b: 2)
来源：http://doz.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://hjg.yuxming.cn

[C05] 返回多个值
来源：http://ybx.xinyue.icu

Py:   return a, b
来源：http://iov.hysaishi.cn

PHP:  return [$a, $b];
来源：http://knw.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ehj.ppjwa.cn

TS:   return { a, b };
来源：http://glq.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lcj.cashguo.top

Go:   return a, b
来源：http://sbh.hongshengwenyu.top

Ruby: return a, b
来源：http://tes.zhijiandao.cn

C#:   return (a, b);              // ValueTuple
来源：http://zvc.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://wmi.ppjwa.cn

Py:   square = lambda x: x * x
来源：http://wqe.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lav.jianghu66.top

JS:   const square = x => x * x;
来源：http://xmd.shzxlz.cn


<!-- 参考信息 -->