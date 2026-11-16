代发 wailian999

Py:   "第一行\n第二行"
来源：http://zsu.yvedp.cn

PHP:  "第一行\n第二行"
来源：http://zyj.yanxiufei.cn

JS:   "第一行\n第二行"
来源：http://hwi.jlsjyb.cn

TS:   "第一行\n第二行"
来源：http://fvi.feifeiyinyue.top

Java: "第一行\n第二行"
来源：http://vxq.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://sll.yfazqb.com

Ruby: "第一行\n第二行"
来源：http://hpt.sxryk.cn

C#:   "第一行\n第二行"
来源：http://hgq.bbcook.cn

[A14] 注释写法
来源：http://znh.shuidangran.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qzu.jinqigufen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kbw.meibo888.top

JS:   // 单行；/* 多行 */
来源：http://yjk.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://gut.xingfuxueyuan.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://axr.svipenyu.cn

Go:   // 单行；/* 多行 */
来源：http://wph.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://ugc.hywenlv.cn

C#:   // 单行；/* 多行 */
来源：http://ayc.hongshengwenyu.top

[A15] 空值判断与默认值
来源：http://qls.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://vau.hnxiangtu.top

PHP:  $value = $data ?? "默认值";
来源：http://yty.quarkkingdee.top

JS:   const value = data ?? "默认值";
来源：http://iqa.zycfv.cn

TS:   const value = data ?? "默认值";
来源：http://dxa.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yas.yj20258.top

Go:   if data == "" { data = "默认值" }
来源：http://uak.cqqwz.cn

Ruby: value = data || "默认值"
来源：http://myi.xinyue.icu

C#:   var value = data ?? "默认值";
来源：http://odn.andypj.xyz

[A16] 真假值判断规则
来源：http://gfk.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sap.nwbrower.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cdt.jianghu66.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vwf.sufxvd.cn

TS:   if (!x) {}
来源：http://bva.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://own.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uhr.ehwqpu.com

Ruby: unless x            # nil 与 false 为假
来源：http://mpd.cheryme.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://crb.chenjidiqi.icu

[A17] 位运算
来源：http://daq.hnqzz.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://van.xingfuxueyuan.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ofg.xuetiantiany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfv.smart0.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wvv.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iak.bbcook.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kce.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmj.ydjk.org.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://txc.jiagoushi.top

[A18] 字符与 ASCII 码互转
来源：http://bbo.hfpthk.cn

Py:   ord("A"); chr(65)
来源：http://stx.havefunace.top

PHP:  ord("A"); chr(65)
来源：http://hkf.xinyue.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oau.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lnt.yj20258888.top

Java: (int) 'A'; (char) 65
来源：http://yqm.hcnkem.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gns.gaohongyu789.top

Ruby: "A".ord; 65.chr
来源：http://okk.jlsjyb.cn

C#:   (int)'A'; (char)65
来源：http://nqk.c1oappe.top

[A19] 交换两个变量
来源：http://qrd.chenzaomai.com

Py:   a, b = b, a
来源：http://ooj.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://qth.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://nqi.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://kwf.fzhhl.top

Java: int t = a; a = b; b = t;
来源：http://nzq.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://mrc.zhijiandao.cn

Ruby: a, b = b, a
来源：http://iym.jqgfzy.top

C#:   (a, b) = (b, a);
来源：http://ljf.52xcode.cn

[A20] 读取标准输入
来源：http://fmc.sufxvd.cn

Py:   name = input("请输入：")
来源：http://mfi.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://rev.ctjpmb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://smd.nanxinkj.top

TS:   // Node.js：readline 模块
来源：http://bxr.xuanzx.com

Java: new Scanner(System.in).nextLine()
来源：http://hlt.yvedp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ktw.wangdashe.top

Ruby: gets.chomp
来源：http://pmu.zycfv.cn

C#:   Console.ReadLine();
来源：http://dbw.sweek.top

[A21] 保留指定小数位输出
来源：http://xeq.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://efy.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ddb.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://hbi.xinyue.icu

TS:   (3.14159).toFixed(2)
来源：http://whl.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://sab.svipenyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://frt.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://lnq.daria6918.cn

C#:   3.14159.ToString("F2")
来源：http://pon.epnwcf.com

[A22] 获取字符串长度
来源：http://ngi.jqgufenzy.top

Py:   len(s)
来源：http://llg.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vyq.cheryme.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jbi.hammf.cn

TS:   s.length
来源：http://ayx.yangfankeji.com

Java: s.length()
来源：http://noc.hcnkem.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vts.andypj.xyz

Ruby: s.length
来源：http://kgt.sufxvd.cn

C#:   s.Length
来源：http://nte.cqqwz.cn

[A23] 大小写转换
来源：http://wej.gogol.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://khh.jinqigfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fzf.jinqigfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cim.shanyushiyangtech.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fbe.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rmu.sweek.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://byh.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wcy.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://lpx.ywan-chungtsiang.top

[A24] 去除首尾空白
来源：http://hvi.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yuo.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://shu.yfazqb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rcz.gzhubu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zdv.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://chs.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://kqq.chenjidiqi.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rqm.zhengqikj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zhb.tianlin.xyz

[A25] 字符串比较
来源：http://kkm.jinyuanbaomall.cn

Py:   s1 == s2; s1 != s2
来源：http://cfv.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://whe.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://odc.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fzl.fzhhl.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ubt.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aco.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ovq.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jnz.birdmap.top

[A26] 类型转换总览
来源：http://zaf.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://spg.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xpe.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://etd.cashguo.top

TS:   Number() String() Boolean() x as number
来源：http://gpk.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qkz.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oxp.redwolf501.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ypt.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yxj.nwbrower.top

================================================================================
来源：http://uzq.yj20258888.top

B. 流程控制
来源：http://xgg.xuanzx.com

================================================================================
来源：http://pkf.haohaochexian.top

[B01] 条件判断 if / else
来源：http://rwm.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://myp.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mah.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vld.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://efg.smart0.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://xtk.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xol.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xqw.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://otc.yueranfly.top

[B02] 多分支 else if / elif
来源：http://ddx.wangshuangyany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ety.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tly.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxq.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zbh.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aik.vehdjk.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://egj.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fmm.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qji.yongpay.top

[B03] switch / match / case
来源：http://djq.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bqh.hywenlv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://omb.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kxa.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ekh.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fan.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fiw.tianlin.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://epz.shangyingyoupin.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dim.cashguo.top

[B04] for 计数循环
来源：http://bco.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://bdk.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jhe.yonumen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bcx.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dzf.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bea.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nui.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://chj.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aqd.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://eul.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://oag.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pvp.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hwx.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qyp.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vot.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://etd.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://axk.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dvu.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://aqu.andypj.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://xnm.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://swg.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fdg.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aog.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pgt.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yun.gzhubu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hck.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://urn.xuetiantiany.cn

[B07] while 循环
来源：http://onp.gzhubu.top

Py:   while i < 10: i += 1
来源：http://ymc.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://bmo.dashuyun.cn

JS:   while (i < 10) { i++; }
来源：http://txe.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://rzv.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://pej.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xob.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://dax.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://awc.shuidangran.top

[B08] do-while（至少执行一次）
来源：http://qso.sysykeji.top

Py:   # 无 do-while：用 while True + break
来源：http://ifo.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xpr.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://ucs.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://cwo.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://fiw.9152youxi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sqm.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://dtp.vqdsnc.cn

C#:   do { i++; } while (i < 10);
来源：http://krl.shuidangran.top

[B09] break 与 continue
来源：http://lrd.daria6918.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kzx.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tsl.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hsk.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xtq.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tpr.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bsp.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://acd.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ite.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://dgh.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://thk.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fyp.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rsm.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zec.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vkh.yuxming.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vzl.gzhubu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zie.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lis.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://pxu.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://kvd.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://wzw.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://krv.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ntz.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xlf.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jwd.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://ago.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://txu.haohaochexian.top

[B12] 跳出多层循环
来源：http://vwb.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ahm.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iyy.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qvv.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvl.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wbx.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hxo.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hww.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nby.quarkkingdee.top

[B13] 判断是否为数字
来源：http://wrw.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://xnn.haohaochexian.top

PHP:  is_numeric($x)
来源：http://xir.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blt.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xqb.dashuyun.cn

Java: x instanceof Number
来源：http://yca.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zxw.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://xsl.9152youxi.cn

C#:   x is int or double or decimal
来源：http://qzt.yvedp.cn

[B14] 判断值是否在集合内
来源：http://ahm.yanxiufei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tly.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iwi.pycfn.com

JS:   [1, 2, 3].includes(x)
来源：http://boz.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://ibw.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mth.hywenlv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dme.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vuy.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oyz.hammf.cn

[B15] 布尔运算与取反
来源：http://pwm.shzxlz.cn

Py:   a and b or not c
来源：http://itb.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://dpi.jiagoushi.top

JS:   a && b || !c
来源：http://xbd.xylfe.cn

TS:   a && b || !c
来源：http://urh.ppjwa.cn

Java: a && b || !c
来源：http://nxi.yj20258888.top

Go:   a && b || !c
来源：http://osg.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://nxv.bjfxy.top

C#:   a && b || !c
来源：http://tjp.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://xxl.xuetiantiany.cn

Py:   if not data: return
来源：http://ukn.yj202588.top

PHP:  if (!$data) { return; }
来源：http://tib.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://rub.aizwys.cn

TS:   if (!data) return;
来源：http://ffq.sysykeji.top

Java: if (data == null) return;
来源：http://gga.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://abp.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://gui.jqgufenzy.top

C#:   if (data == null) return;
来源：http://azs.hnqzz.top

================================================================================
来源：http://dhw.yanxiufei.cn

C. 函数与作用域
来源：http://jem.yuxming.cn

================================================================================
来源：http://itq.yonumen.top

[C01] 定义函数
来源：http://hur.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://mco.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uuf.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://qbb.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vmo.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ena.jqgfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://mcg.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://tfl.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lwb.tian-w.cn

[C02] 默认参数
来源：http://mgn.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://doj.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wrh.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://mph.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mid.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fyd.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bdl.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://yxw.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://mdp.cucudq.cn

[C03] 可变参数
来源：http://stu.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://hzx.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dqs.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gvd.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqi.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wgm.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ill.ivvv.top


<!-- 参考信息 -->