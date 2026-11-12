代发 wailian999

[A14] 注释写法
来源：http://iqi.zycfv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fev.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ebk.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://xqd.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://bqu.ivvv.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://obm.yonumen.top

Go:   // 单行；/* 多行 */
来源：http://qcm.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://pvl.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://spg.cqqwz.cn

[A15] 空值判断与默认值
来源：http://fqa.xziqi.cn

Py:   value = data or "默认值"
来源：http://tsx.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://yiw.snrcjt.cn

JS:   const value = data ?? "默认值";
来源：http://bxk.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://zli.0kj1m.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ndq.nwbrower.top

Go:   if data == "" { data = "默认值" }
来源：http://etr.xziqi.cn

Ruby: value = data || "默认值"
来源：http://qqy.yj20258888.top

C#:   var value = data ?? "默认值";
来源：http://wvp.vehdjk.com

[A16] 真假值判断规则
来源：http://otx.jianghu66.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jia.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://umb.yonumen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ywh.yj202588.top

TS:   if (!x) {}
来源：http://gvq.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hle.zhaomingkeji.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://giq.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://hlb.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pjn.zhaomingkeji.xyz

[A17] 位运算
来源：http://siv.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykv.aizwys.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eel.xziqi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcj.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://eob.epnwcf.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nxe.jqgfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wyo.hongshengwenyu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwn.gogol.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lhe.smart0.xyz

[A18] 字符与 ASCII 码互转
来源：http://nlx.yonumen.top

Py:   ord("A"); chr(65)
来源：http://pnc.vqdsnc.cn

PHP:  ord("A"); chr(65)
来源：http://doh.pengpengdd.cyou

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://txg.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xiq.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://apa.pengpengdd.cyou

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cqy.ybcxt.top

Ruby: "A".ord; 65.chr
来源：http://bmw.yfazqb.com

C#:   (int)'A'; (char)65
来源：http://axo.gotoacloud.top

[A19] 交换两个变量
来源：http://icz.tianlin.xyz

Py:   a, b = b, a
来源：http://xiq.316326.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://vil.cheryme.top

JS:   [a, b] = [b, a];
来源：http://uod.ctjpmb.com

TS:   [a, b] = [b, a];
来源：http://jgl.jqgufenzy.top

Java: int t = a; a = b; b = t;
来源：http://moe.fktsv.cn

Go:   a, b = b, a
来源：http://xxa.fzhhl.top

Ruby: a, b = b, a
来源：http://rcm.yonumen.top

C#:   (a, b) = (b, a);
来源：http://gmg.fktsv.cn

[A20] 读取标准输入
来源：http://mwx.hnqzz.top

Py:   name = input("请输入：")
来源：http://tpr.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ush.bbcook.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dwy.ppjwa.cn

TS:   // Node.js：readline 模块
来源：http://kkp.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://oed.uphjek.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aht.hnqzz.top

Ruby: gets.chomp
来源：http://esm.gaohongyu789.top

C#:   Console.ReadLine();
来源：http://kyp.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://vrt.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://vdb.ydjk.org.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ktk.aibaodan.cn

JS:   (3.14159).toFixed(2)
来源：http://epa.yj202588.top

TS:   (3.14159).toFixed(2)
来源：http://awb.guowangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://vqb.zycfv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gkq.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://gos.9152youxi.cn

C#:   3.14159.ToString("F2")
来源：http://gcy.9152youxi.cn

[A22] 获取字符串长度
来源：http://hjm.hfpthk.cn

Py:   len(s)
来源：http://mqh.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bxu.0kj1m.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aho.ctjpmb.com

TS:   s.length
来源：http://qxf.jqgfzy.top

Java: s.length()
来源：http://ntb.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qfr.cashguo.top

Ruby: s.length
来源：http://xci.ctjpmb.com

C#:   s.Length
来源：http://jjk.zhijiandao.cn

[A23] 大小写转换
来源：http://kxk.xylfe.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tli.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bsr.tarul.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qiv.mhx1999.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ofi.tarul.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oji.aizwys.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://squ.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lyr.ctjpmb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://kif.sjlbkw.cn

[A24] 去除首尾空白
来源：http://vrf.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wir.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zjn.yfazqb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iyx.cucudq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yzf.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vid.hesvh.cn

Go:   strings.TrimSpace(s)
来源：http://wve.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lmn.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://elw.svipenyu.cn

[A25] 字符串比较
来源：http://xid.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://rtv.fehbvm.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rtf.xinyue.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mky.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://has.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cdp.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rnx.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mqg.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pnz.hnqzz.top

[A26] 类型转换总览
来源：http://mtj.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ntg.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zvs.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rcc.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://grn.zhongyouzk.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://exj.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oju.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yqa.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zai.jinyuanbaomall.cn

================================================================================
来源：http://iba.cdnleiting.top

B. 流程控制
来源：http://xym.hnqzz.top

================================================================================
来源：http://bah.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://rpu.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qho.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ckj.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gbc.nanxuanxn.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rii.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vig.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aod.c1oappe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://unj.316326.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qxm.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://klu.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ees.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jcn.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gvv.cdnleiting.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://epy.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://prx.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xdv.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://frz.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qdq.316326.xyz

[B03] switch / match / case
来源：http://yqb.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bhp.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lqv.yj20258888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mmf.fengsongda.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rts.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nvu.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://srs.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://der.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qup.gogol.net.cn

[B04] for 计数循环
来源：http://ofl.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://tui.xuanzx.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cqt.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nri.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ftp.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://osk.zhongyouzk.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tsj.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://svo.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nfg.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://zmy.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://nkx.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gvn.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ycg.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://enu.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lxr.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ulr.gzhubu.top

Ruby: arr.each { |item| puts item }
来源：http://nqk.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vkn.xylfe.cn

[B06] 遍历字典 / 对象
来源：http://ehj.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dps.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://phk.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://znu.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jrl.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xsj.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pet.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://flm.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tfn.smart0.xyz

[B07] while 循环
来源：http://gsi.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://riq.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://hpe.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://vcb.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://rsg.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://ali.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dzf.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://nyd.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://kvw.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://sxm.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://xoo.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nmc.aibaodan.cn

JS:   do { i++; } while (i < 10);
来源：http://mmx.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://bas.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://bvt.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rwu.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://yeh.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://iow.jinqigfzy.top

[B09] break 与 continue
来源：http://ubx.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xqt.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://juu.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://phg.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://adj.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mdm.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rgj.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jcy.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sks.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://yan.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ymb.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gcf.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dmi.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eio.9152youxi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bmn.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ztt.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://thm.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bcg.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://ktk.wangdashe.top

Py:   list(range(0, 10, 2))
来源：http://uqw.zhoulong.xyz

PHP:  range(0, 10, 2);
来源：http://qzv.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lfs.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rvx.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://klo.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eyk.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://jzf.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tji.bbcook.cn

[B12] 跳出多层循环
来源：http://rci.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tdd.wangdashe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oho.316326.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iet.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://byq.feifeiyinyue.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://maq.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vsl.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vmj.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qlv.c1oappe.top

[B13] 判断是否为数字
来源：http://ggk.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://heh.c1oappe.top

PHP:  is_numeric($x)
来源：http://hno.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cmg.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xhx.fengsongda.top

Java: x instanceof Number
来源：http://wyi.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lfo.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://eac.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://kpi.xylfe.cn

[B14] 判断值是否在集合内
来源：http://lwb.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jhn.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kbq.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://rgs.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://zfs.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qvs.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tdx.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://fpr.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dar.hnqzz.top

[B15] 布尔运算与取反
来源：http://sek.jinqigfzy.top

Py:   a and b or not c
来源：http://nlh.yj20258888.top

PHP:  $a && $b || !$c
来源：http://okm.hammf.cn

JS:   a && b || !c
来源：http://dco.vqdsnc.cn

TS:   a && b || !c
来源：http://xcv.xziqi.cn

Java: a && b || !c
来源：http://fxd.cqqwz.cn

Go:   a && b || !c
来源：http://mbc.bjfxy.top

Ruby: a && b || !c
来源：http://gfz.ehwqpu.com

C#:   a && b || !c
来源：http://jsl.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bzb.ybcxt.top

Py:   if not data: return
来源：http://wry.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://wkr.yueranfly.top

JS:   if (!data) return;
来源：http://fju.zhoulong.xyz

TS:   if (!data) return;
来源：http://ncr.zhoulong.xyz

Java: if (data == null) return;
来源：http://cxd.zhengqikj.top

Go:   if data == nil { return }
来源：http://tow.jyoumei.cn

Ruby: return if data.nil?
来源：http://kpt.sweek.top

C#:   if (data == null) return;
来源：http://kht.gotoacloud.top

================================================================================
来源：http://bes.fehbvm.com

C. 函数与作用域
来源：http://lyg.hnxiangtu.top

================================================================================
来源：http://nfy.cucudq.cn

[C01] 定义函数
来源：http://pbu.yj202588.top

Py:   def add(a, b): return a + b
来源：http://imo.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixj.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://erl.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zsc.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://cin.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bag.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://cmi.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fzv.jiagoushi.top

[C02] 默认参数
来源：http://qnx.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://wnf.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zkl.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://hhv.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qlx.yvedp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oxz.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yjl.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://ksz.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://cmn.chenlongwang.top

[C03] 可变参数
来源：http://wpf.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://fhz.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://osl.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lgr.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iuk.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ayi.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://psb.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vck.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dri.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://wum.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sso.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iye.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xsl.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ptq.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://ghr.fktsv.cn


<!-- 参考信息 -->