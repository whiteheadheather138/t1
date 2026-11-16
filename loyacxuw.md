代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://joc.vehdjk.com

TS:   const value = data ?? "默认值";
来源：http://lor.nanxuanxn.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mtm.xingfuxueyuan.xyz

Go:   if data == "" { data = "默认值" }
来源：http://rco.ydzc1.top

Ruby: value = data || "默认值"
来源：http://sbc.dashuyun.cn

C#:   var value = data ?? "默认值";
来源：http://kru.zhiwuduotai.top

[A16] 真假值判断规则
来源：http://lbz.shuidangran.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://upr.ivvv.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zzg.wangdashe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yif.zhiwuduotai.top

TS:   if (!x) {}
来源：http://qum.chenjidiqi.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tna.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qjs.sufxvd.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wfi.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qlm.xingfuxueyuan.xyz

[A17] 位运算
来源：http://rzk.tarul.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wcq.jiagoushi.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://exx.ctjpmb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lml.zhixingplan.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hgx.sufxvd.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nmr.yfazqb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ngc.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mqw.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fpz.wangshuangyany.cn

[A18] 字符与 ASCII 码互转
来源：http://ngo.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://pqk.jlsjyb.cn

PHP:  ord("A"); chr(65)
来源：http://loe.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vxi.jqgfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dcr.epnwcf.com

Java: (int) 'A'; (char) 65
来源：http://oze.gaohongyu789.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jyp.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://mny.nanxuanxn.top

C#:   (int)'A'; (char)65
来源：http://ula.zhixingplan.top

[A19] 交换两个变量
来源：http://jrr.tianlin.xyz

Py:   a, b = b, a
来源：http://hex.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jyr.shuidangran.top

JS:   [a, b] = [b, a];
来源：http://cxs.yvedp.cn

TS:   [a, b] = [b, a];
来源：http://nrk.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://sjn.chenlongwang.top

Go:   a, b = b, a
来源：http://diu.ivvv.top

Ruby: a, b = b, a
来源：http://zop.yj202588.top

C#:   (a, b) = (b, a);
来源：http://gsj.fehbvm.com

[A20] 读取标准输入
来源：http://qrp.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://kyj.haohaochexian.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kkw.jianghu66.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dwh.meibo888.top

TS:   // Node.js：readline 模块
来源：http://kfw.shzxlz.cn

Java: new Scanner(System.in).nextLine()
来源：http://xfi.zhijiandao.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hmv.wangdashe.top

Ruby: gets.chomp
来源：http://ggm.sysykeji.top

C#:   Console.ReadLine();
来源：http://ehp.chenlongwang.top

[A21] 保留指定小数位输出
来源：http://deu.quarkkingdee.top

Py:   f"{3.14159:.2f}"
来源：http://mct.hesvh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cgd.jlsjyb.cn

JS:   (3.14159).toFixed(2)
来源：http://cyr.haohaochexian.top

TS:   (3.14159).toFixed(2)
来源：http://pvs.meibo888.top

Java: String.format("%.2f", 3.14159)
来源：http://rta.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://shi.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://vxe.yuxming.cn

C#:   3.14159.ToString("F2")
来源：http://ugw.jinqigfzy.top

[A22] 获取字符串长度
来源：http://juv.redwolf501.top

Py:   len(s)
来源：http://pxc.zhijiandao.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qns.hfpthk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fxq.jinghuilouyu.cn

TS:   s.length
来源：http://umv.gogol.net.cn

Java: s.length()
来源：http://ymz.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nix.shangyingyoupin.top

Ruby: s.length
来源：http://jak.ivvv.top

C#:   s.Length
来源：http://epp.yj20258888.top

[A23] 大小写转换
来源：http://qlw.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mvs.jinqigfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qiw.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qjk.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rza.fanxiaobao.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vpw.redwolf501.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mzz.wangdashe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lhe.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gum.chenlongwang.top

[A24] 去除首尾空白
来源：http://zsd.fktsv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sbu.hcnkem.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://asj.shuidangran.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pzr.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ifr.yueranfly.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://min.jinghuilouyu.cn

Go:   strings.TrimSpace(s)
来源：http://bsa.ppjwa.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xbv.zhengqikj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ksw.guannengcc.top

[A25] 字符串比较
来源：http://pax.uphjek.com

Py:   s1 == s2; s1 != s2
来源：http://rma.gzhubu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qxb.wangshuangyany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ahp.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://apz.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lrn.xingfuxueyuan.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yci.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ays.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://klg.fengsongda.top

[A26] 类型转换总览
来源：http://hbr.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gqr.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hgn.jinghuilouyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xis.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://mrk.yonumen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ftw.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iji.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://unu.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aux.tian-w.cn

================================================================================
来源：http://vsq.yj20258.top

B. 流程控制
来源：http://noy.nanxinkj.top

================================================================================
来源：http://itq.zhongyouzk.top

[B01] 条件判断 if / else
来源：http://jod.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://iyt.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fnx.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ery.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lur.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pji.gotoacloud.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vbe.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://god.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://azv.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://vvc.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://azi.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bav.mhx1999.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qfj.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ssv.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bmp.jqgufenzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vie.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pcf.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpn.sjlbkw.cn

[B03] switch / match / case
来源：http://mok.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tis.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://quh.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://poy.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nvi.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eni.sjlbkw.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rmv.xuanzx.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xmi.ctjpmb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://khl.yvedp.cn

[B04] for 计数循环
来源：http://lfn.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://asc.jianghu66.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://udo.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cuf.xingfuxueyuan.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tcx.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zoa.hnxiangtu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ilh.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://jdb.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dqg.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://pbr.daxiang520.top

Py:   for item in arr: print(item)
来源：http://tdy.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ydn.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://xvi.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qab.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iqd.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wwg.chenzaomai.com

Ruby: arr.each { |item| puts item }
来源：http://abb.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uhs.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://cei.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sqz.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ymq.cheryme.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ypq.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://klm.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tac.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pst.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jhd.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zta.hnxiangtu.top

[B07] while 循环
来源：http://frq.gotoacloud.top

Py:   while i < 10: i += 1
来源：http://voc.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://ofb.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://qwe.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://qny.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://air.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://muf.jiagoushi.top

Ruby: while i < 10; i += 1; end
来源：http://qvq.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://fcn.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://fys.zhoulong.xyz

Py:   # 无 do-while：用 while True + break
来源：http://pdf.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://usd.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://uvl.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://nmh.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://igo.shanyushiyangtech.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dhl.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pcc.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://kte.cashguo.top

[B09] break 与 continue
来源：http://sxs.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pai.jinghuilouyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nkm.xuanzx.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bkq.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fhd.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnl.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ajx.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ysj.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://axv.zycfv.cn

[B10] 遍历同时拿索引
来源：http://fwn.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qkm.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mhx.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zdj.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fns.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sbe.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hjb.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vgm.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wsm.zdbjq.cn

[B11] 生成数字序列 / 区间
来源：http://loe.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://hgc.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://hfe.aibaodan.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://has.sxryk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fqf.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uek.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gki.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://vuw.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wpk.sufxvd.cn

[B12] 跳出多层循环
来源：http://iuo.yuanzhike.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://leu.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aat.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rge.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oqq.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vdt.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://psx.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qvp.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mex.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://tkl.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://xof.zycfv.cn

PHP:  is_numeric($x)
来源：http://ibr.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://byx.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tlz.wangdashe.top

Java: x instanceof Number
来源：http://iim.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cex.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://tnn.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://xaa.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://baz.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rim.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kcp.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://rop.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://rbv.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://jba.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eys.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://qdd.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sqf.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://fuy.fengsongda.top

Py:   a and b or not c
来源：http://yvq.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://rvq.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://qir.xuetiantiany.cn

TS:   a && b || !c
来源：http://sjw.fehbvm.com

Java: a && b || !c
来源：http://fqf.daria6918.cn

Go:   a && b || !c
来源：http://qxk.yj20258.top

Ruby: a && b || !c
来源：http://vos.yanxiufei.cn

C#:   a && b || !c
来源：http://bfb.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://dxb.sxryk.cn

Py:   if not data: return
来源：http://jrm.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://ntj.shzxlz.cn

JS:   if (!data) return;
来源：http://gdq.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://ejp.ivvv.top

Java: if (data == null) return;
来源：http://exg.hammf.cn

Go:   if data == nil { return }
来源：http://vge.jqgufenzy.top

Ruby: return if data.nil?
来源：http://ayl.sxryk.cn

C#:   if (data == null) return;
来源：http://scj.wangshuangyany.cn

================================================================================
来源：http://fpl.wangdashe.top

C. 函数与作用域
来源：http://fcz.xuanzx.com

================================================================================
来源：http://rbw.sweek.top

[C01] 定义函数
来源：http://fwq.yj20258.top

Py:   def add(a, b): return a + b
来源：http://iit.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nia.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://hah.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pdd.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://naq.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://tnw.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://ejj.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://koa.yonumen.top

[C02] 默认参数
来源：http://fij.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://qpn.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lpw.guowangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://qvg.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://yko.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zge.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nxe.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://yio.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://pjg.yuanzhike.top

[C03] 可变参数
来源：http://ivd.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://tnd.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dgf.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtj.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rcf.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ahg.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vte.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://ozb.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lvq.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://yym.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ofe.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://awa.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gim.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aof.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://tli.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://bue.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://vmg.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://kpy.uphjek.com

[C05] 返回多个值
来源：http://hol.hongshengwenyu.top

Py:   return a, b
来源：http://rrk.xziqi.cn

PHP:  return [$a, $b];
来源：http://zwz.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cnh.guannengcc.top

TS:   return { a, b };
来源：http://hsk.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yey.yj20258888.top

Go:   return a, b
来源：http://tii.vehdjk.com

Ruby: return a, b
来源：http://rak.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://yub.zdbjq.cn


<!-- 参考信息 -->