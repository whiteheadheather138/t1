代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tky.redwolf501.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kxz.xylfe.cn

TS:   if (!x) {}
来源：http://vns.cheryme.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vhe.gzhubu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zij.xinyue.icu

Ruby: unless x            # nil 与 false 为假
来源：http://ihu.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mqg.wangdashe.top

[A17] 位运算
来源：http://aeb.epnwcf.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ttx.fehbvm.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xsa.52xcode.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srd.tianlin.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://khh.daria6918.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dof.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://stf.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ilz.bjfxy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://upq.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://yiy.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://ckh.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://hsr.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mve.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bgi.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://gqi.hywenlv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mfs.ybcxt.top

Ruby: "A".ord; 65.chr
来源：http://wtu.feifeiyinyue.top

C#:   (int)'A'; (char)65
来源：http://xku.yongpay.top

[A19] 交换两个变量
来源：http://pti.svipenyu.cn

Py:   a, b = b, a
来源：http://atw.wangshuangyany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kio.yj20258888.top

JS:   [a, b] = [b, a];
来源：http://qew.cheryme.top

TS:   [a, b] = [b, a];
来源：http://gzh.jqgfzy.top

Java: int t = a; a = b; b = t;
来源：http://zal.jlsjyb.cn

Go:   a, b = b, a
来源：http://zrw.bjfxy.top

Ruby: a, b = b, a
来源：http://xsc.iojbl.cn

C#:   (a, b) = (b, a);
来源：http://kxc.meibo888.top

[A20] 读取标准输入
来源：http://svu.birdmap.top

Py:   name = input("请输入：")
来源：http://etf.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kfo.fzhhl.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://six.quarkkingdee.top

TS:   // Node.js：readline 模块
来源：http://lpl.yongpay.top

Java: new Scanner(System.in).nextLine()
来源：http://dqo.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bhs.yfazqb.com

Ruby: gets.chomp
来源：http://kuj.jyoumei.cn

C#:   Console.ReadLine();
来源：http://ssn.nanxinkj.top

[A21] 保留指定小数位输出
来源：http://col.sjlbkw.cn

Py:   f"{3.14159:.2f}"
来源：http://ttk.yongpay.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gvb.zhaomingkeji.xyz

JS:   (3.14159).toFixed(2)
来源：http://cbt.vqdsnc.cn

TS:   (3.14159).toFixed(2)
来源：http://vqn.sxryk.cn

Java: String.format("%.2f", 3.14159)
来源：http://aoe.zhoulong.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tex.gaohongyu789.top

Ruby: format("%.2f", 3.14159)
来源：http://zrg.yj202588.top

C#:   3.14159.ToString("F2")
来源：http://opo.bjfxy.top

[A22] 获取字符串长度
来源：http://lqd.nanxinkj.top

Py:   len(s)
来源：http://tdl.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ldt.pengpengdd.cyou

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bza.shuidangran.top

TS:   s.length
来源：http://vez.shangyingyoupin.top

Java: s.length()
来源：http://rft.pengpengdd.cyou

Go:   len(s); utf8.RuneCountInString(s)
来源：http://egy.fehbvm.com

Ruby: s.length
来源：http://wdh.zhoulong.xyz

C#:   s.Length
来源：http://aeg.aizwys.cn

[A23] 大小写转换
来源：http://cns.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fat.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dwj.yonumen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wju.bjfxy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://key.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vri.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qbu.jqgufenzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nhf.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bul.zycfv.cn

[A24] 去除首尾空白
来源：http://okz.xinyue.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tzp.hnxiangtu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tzt.zdbjq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fsm.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uui.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://udo.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://pci.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rfh.shuidangran.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xfl.yj202588.top

[A25] 字符串比较
来源：http://rdj.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://vgi.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pyz.fktsv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yii.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kqu.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lyw.fehbvm.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ggs.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://bfb.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ucw.xinyue.icu

[A26] 类型转换总览
来源：http://xan.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://foj.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rsr.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zqe.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://xxm.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cpk.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cmw.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gbn.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mek.hesvh.cn

================================================================================
来源：http://bhi.zhixingplan.top

B. 流程控制
来源：http://bws.birdmap.top

================================================================================
来源：http://hod.havefunace.top

[B01] 条件判断 if / else
来源：http://kpp.tian-w.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uyu.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eyf.zhijiandao.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kkp.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://row.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://who.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rdp.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zsf.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kwh.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://rlr.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zip.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ikg.jyoumei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oso.kuanghao11.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vmp.chenzaomai.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sgs.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vts.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mfl.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dya.vehdjk.com

[B03] switch / match / case
来源：http://lcw.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kto.xinyue.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lrb.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gja.52xcode.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kof.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://itd.jqgufenzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fox.pycfn.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ttv.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mpw.gotoacloud.top

[B04] for 计数循环
来源：http://rah.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://qbf.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nla.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vpp.yuanzhike.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ygl.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ltj.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vra.shuidangran.top

Ruby: 10.times { |i| puts i }
来源：http://ddl.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uoy.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://aaz.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://wwj.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rnz.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wco.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://upr.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iwc.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xyf.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://gtv.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bah.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://aka.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lqd.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qnt.tianlin.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rgz.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eqi.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cgu.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ugl.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qos.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bxy.cucudq.cn

[B07] while 循环
来源：http://fdc.zhongyouzk.top

Py:   while i < 10: i += 1
来源：http://jxm.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://qtk.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://dia.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://xac.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://ykr.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://erf.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://nxa.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://vve.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://gqk.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://tla.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://hib.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://fup.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://tsv.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://omv.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://gra.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sko.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://jkc.hammf.cn

[B09] break 与 continue
来源：http://ovz.zhiwuduotai.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ung.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aqz.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hhp.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://myc.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://reh.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pxn.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ijc.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgj.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://vov.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gai.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hnc.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fsg.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mjo.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://scv.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yvr.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zka.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sgk.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://qwl.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://him.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://pbw.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://txu.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nny.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rky.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yyh.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://ltt.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sls.feifeiyinyue.top

[B12] 跳出多层循环
来源：http://ilb.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fun.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://umq.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ptz.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ycr.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wqd.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gtb.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nxz.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mxu.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://suf.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://gkk.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://vdc.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mek.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uqx.zhengqikj.top

Java: x instanceof Number
来源：http://cwm.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xzb.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://tmq.jinqigufen.top

C#:   x is int or double or decimal
来源：http://uno.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://lrk.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zrg.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://njt.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://jfn.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://jpy.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://wcf.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dze.yanxiufei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ibd.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://egm.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://vxr.kuanghao11.cn

Py:   a and b or not c
来源：http://yzg.uphjek.com

PHP:  $a && $b || !$c
来源：http://qci.kuanghao11.cn

JS:   a && b || !c
来源：http://uzt.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://ljm.jlsjyb.cn

Java: a && b || !c
来源：http://lyl.9152youxi.cn

Go:   a && b || !c
来源：http://rvj.quarkkingdee.top

Ruby: a && b || !c
来源：http://cfg.hongshengwenyu.top

C#:   a && b || !c
来源：http://xyw.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://mto.ehwqpu.com

Py:   if not data: return
来源：http://tkr.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://acg.yongpay.top

JS:   if (!data) return;
来源：http://fio.hongshengwenyu.top

TS:   if (!data) return;
来源：http://abh.jiagoushi.top

Java: if (data == null) return;
来源：http://ydq.sysykeji.top

Go:   if data == nil { return }
来源：http://rmn.sufxvd.cn

Ruby: return if data.nil?
来源：http://imw.ydzc1.top

C#:   if (data == null) return;
来源：http://bqm.tanke756.top

================================================================================
来源：http://nij.sysykeji.top

C. 函数与作用域
来源：http://xgk.pycfn.com

================================================================================
来源：http://eny.hywenlv.cn

[C01] 定义函数
来源：http://syx.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://xdg.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://izg.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://edz.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vok.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hea.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://rel.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://san.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xam.cashguo.top

[C02] 默认参数
来源：http://bvs.havefunace.top

Py:   def greet(name="World"): return name
来源：http://ssd.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://egu.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://pyo.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qpe.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://drf.hongshengwenyu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vwr.shzxlz.cn

Ruby: def greet(name = "World") = name
来源：http://lld.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://tsy.epnwcf.com

[C03] 可变参数
来源：http://onx.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://lnh.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vea.havefunace.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://phs.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nxe.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dsh.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lwa.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://iii.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xfd.ctjpmb.com

[C04] 命名参数 / 关键字参数
来源：http://mix.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fjq.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ztb.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cro.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uts.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://ezm.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://zuh.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://qhu.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://jty.andypj.xyz

[C05] 返回多个值
来源：http://gyp.nanxuanxn.top

Py:   return a, b
来源：http://oll.0kj1m.cn

PHP:  return [$a, $b];
来源：http://jow.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cha.xuanzx.com

TS:   return { a, b };
来源：http://urp.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hso.nanxuanxn.top

Go:   return a, b
来源：http://rgb.gzhubu.top

Ruby: return a, b
来源：http://yfe.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://zti.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://hqj.ivvv.top

Py:   square = lambda x: x * x
来源：http://rlw.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hoh.dashuyun.cn

JS:   const square = x => x * x;
来源：http://jsl.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://gth.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jeb.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://wbv.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://ofc.yongpay.top


<!-- 参考信息 -->