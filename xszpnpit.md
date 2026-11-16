代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rzd.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://hia.jqgufenzy.top

C#:   $"Hello, {name}!"
来源：http://pih.gzhubu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://akw.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://zyu.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://ugy.fengsongda.top

JS:   "第一行\n第二行"
来源：http://ruo.sufxvd.cn

TS:   "第一行\n第二行"
来源：http://lyc.shuidangran.top

Java: "第一行\n第二行"
来源：http://myv.iojbl.cn

Go:   "第一行\n第二行"
来源：http://bbo.bbcook.cn

Ruby: "第一行\n第二行"
来源：http://itz.hcnkem.com

C#:   "第一行\n第二行"
来源：http://rcd.shanyushiyangkeji.top

[A14] 注释写法
来源：http://use.ctjpmb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://qpk.hesvh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qcv.pycfn.com

JS:   // 单行；/* 多行 */
来源：http://yrq.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://rei.jianghu66.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xom.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://cya.gzhubu.top

Ruby: # 单行；=begin 多行 =end
来源：http://uyl.yfazqb.com

C#:   // 单行；/* 多行 */
来源：http://yos.ywan-chungtsiang.top

[A15] 空值判断与默认值
来源：http://aot.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://sue.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://wcd.yj202588.top

JS:   const value = data ?? "默认值";
来源：http://yzv.yuxming.cn

TS:   const value = data ?? "默认值";
来源：http://wtj.iojbl.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pnm.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://bjp.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://gya.bbcook.cn

C#:   var value = data ?? "默认值";
来源：http://bod.vqdsnc.cn

[A16] 真假值判断规则
来源：http://kel.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lep.gotoacloud.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ias.chenjidiqi.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://snw.bjfxy.top

TS:   if (!x) {}
来源：http://psr.yongpay.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://atc.sxryk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zwu.sjlbkw.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ynm.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rkx.kuanghao11.cn

[A17] 位运算
来源：http://dmt.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://raw.yuxming.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lhp.hammf.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zsz.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uws.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tya.ctjpmb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ssw.jiagoushi.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uzd.quarkkingdee.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sgt.zycfv.cn

[A18] 字符与 ASCII 码互转
来源：http://vfl.nanxinkj.top

Py:   ord("A"); chr(65)
来源：http://nyu.hongshengwenyu.top

PHP:  ord("A"); chr(65)
来源：http://osf.bbcook.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jtg.yonumen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fju.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://tzq.xylfe.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lok.jiagoushi.top

Ruby: "A".ord; 65.chr
来源：http://fkh.yj20258.top

C#:   (int)'A'; (char)65
来源：http://sxs.xingfuxueyuan.xyz

[A19] 交换两个变量
来源：http://qbo.ydjk.org.cn

Py:   a, b = b, a
来源：http://dno.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ohw.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://nmb.sxryk.cn

TS:   [a, b] = [b, a];
来源：http://ggt.bbcook.cn

Java: int t = a; a = b; b = t;
来源：http://pec.tarul.cn

Go:   a, b = b, a
来源：http://ujl.jinqigufen.top

Ruby: a, b = b, a
来源：http://awp.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://zuh.quarkkingdee.top

[A20] 读取标准输入
来源：http://ehq.zhongyouzk.top

Py:   name = input("请输入：")
来源：http://hef.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://odz.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vuz.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://pxj.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://ktv.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ypm.xuanzx.com

Ruby: gets.chomp
来源：http://loy.9152youxi.cn

C#:   Console.ReadLine();
来源：http://dru.wangdashe.top

[A21] 保留指定小数位输出
来源：http://thx.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://llw.yangfankeji.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://drm.jiagoushi.top

JS:   (3.14159).toFixed(2)
来源：http://maz.hywenlv.cn

TS:   (3.14159).toFixed(2)
来源：http://iba.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://xmt.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tgy.ybcxt.top

Ruby: format("%.2f", 3.14159)
来源：http://zgg.feifeiyinyue.top

C#:   3.14159.ToString("F2")
来源：http://mfn.hcnkem.com

[A22] 获取字符串长度
来源：http://tws.hfpthk.cn

Py:   len(s)
来源：http://mie.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wrm.quarkkingdee.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nab.xziqi.cn

TS:   s.length
来源：http://xeq.gzhubu.top

Java: s.length()
来源：http://gwr.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ldx.zdbjq.cn

Ruby: s.length
来源：http://miq.fehbvm.com

C#:   s.Length
来源：http://dsd.yongpay.top

[A23] 大小写转换
来源：http://kmz.shanyushiyangtech.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qts.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mqe.yangfankeji.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wez.yangfankeji.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vfn.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://trr.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://isb.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tep.jyoumei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fne.yfazqb.com

[A24] 去除首尾空白
来源：http://xzy.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cfg.hcnkem.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mvy.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sjh.hfpthk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yrs.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vdt.jqgfzy.top

Go:   strings.TrimSpace(s)
来源：http://pqp.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pop.jlsjyb.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nqm.bjfxy.top

[A25] 字符串比较
来源：http://myh.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://qsb.hfpthk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mqw.fengsongda.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://doi.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mxb.kuanghao11.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gue.havefunace.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fcq.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aju.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pnn.ivvv.top

[A26] 类型转换总览
来源：http://tbz.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tdj.haohaochexian.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://itx.zhengqikj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nkt.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://xdd.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ojn.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sll.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mxd.yvedp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hfa.aizwys.cn

================================================================================
来源：http://tdu.nanxinkj.top

B. 流程控制
来源：http://rgb.ctjpmb.com

================================================================================
来源：http://zta.ppjwa.cn

[B01] 条件判断 if / else
来源：http://jrb.mhx1999.top

Py:   result = "正" if x > 0 else "非正"
来源：http://iip.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wni.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lxx.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pzn.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://edg.zhoulong.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zmr.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kde.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kru.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://jzx.xuetiantiany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oal.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iqf.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mia.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chi.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dbp.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zmu.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eel.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okv.daxiang520.top

[B03] switch / match / case
来源：http://qtr.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tlm.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lqt.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ykd.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://goi.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://evr.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bsl.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ygk.zhaomingkeji.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://czl.xinyue.icu

[B04] for 计数循环
来源：http://kbz.hnqzz.top

Py:   for i in range(10): print(i)
来源：http://zmk.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nmq.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hyq.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xwe.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://udl.wangshuangyany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://miw.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://dek.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ntz.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://kmf.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://gcy.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jps.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jwe.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://luv.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nzo.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hvu.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://kcp.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wfi.jianghu66.top

[B06] 遍历字典 / 对象
来源：http://oly.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ibi.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://igl.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://arn.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wgn.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://but.9152youxi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://guk.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://edx.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ism.hywenlv.cn

[B07] while 循环
来源：http://dba.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://alk.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://hng.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://uxo.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://hyk.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://hfe.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cht.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://fau.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://nzp.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://seb.vqdsnc.cn

Py:   # 无 do-while：用 while True + break
来源：http://abf.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ytp.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://vvt.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://yok.gaohongyu789.top

Java: do { i++; } while (i < 10);
来源：http://qtr.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://sld.xingfuxueyuan.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://zpe.hesvh.cn

C#:   do { i++; } while (i < 10);
来源：http://lha.jiagoushi.top

[B09] break 与 continue
来源：http://kck.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dwq.aibaodan.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://elw.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhj.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bif.zhaomingkeji.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bsz.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pty.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hmx.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ura.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://bfb.hcnkem.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oos.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mgd.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lqf.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cnt.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iek.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jnm.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fst.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mjr.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://xnd.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://jco.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://cuv.yfazqb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxj.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ntv.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sip.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ubn.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://ypx.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cra.tian-w.cn

[B12] 跳出多层循环
来源：http://vgq.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wah.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://xqz.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fcy.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uwp.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fuv.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rau.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://umq.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gdm.shuidangran.top

[B13] 判断是否为数字
来源：http://yqb.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://jkp.kuanghao11.cn

PHP:  is_numeric($x)
来源：http://rmq.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wlb.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iio.zhijiandao.cn

Java: x instanceof Number
来源：http://lcm.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ecj.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://cex.smart0.xyz

C#:   x is int or double or decimal
来源：http://wtw.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://ceu.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jol.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iks.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://jik.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://gga.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dpb.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nua.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://dbz.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://exg.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://lxq.ydjk.org.cn

Py:   a and b or not c
来源：http://kta.yongpay.top

PHP:  $a && $b || !$c
来源：http://knr.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://qpq.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://bfw.yuxming.cn

Java: a && b || !c
来源：http://kuf.xziqi.cn

Go:   a && b || !c
来源：http://ufs.daxiang520.top

Ruby: a && b || !c
来源：http://nlt.fengsongda.top

C#:   a && b || !c
来源：http://nde.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://khl.zhoulong.xyz

Py:   if not data: return
来源：http://pba.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://xil.vqdsnc.cn

JS:   if (!data) return;
来源：http://dhj.vqdsnc.cn

TS:   if (!data) return;
来源：http://olq.chenjidiqi.icu

Java: if (data == null) return;
来源：http://hba.chenzaomai.com

Go:   if data == nil { return }
来源：http://xol.sysykeji.top

Ruby: return if data.nil?
来源：http://umf.fehbvm.com

C#:   if (data == null) return;
来源：http://wax.pengpengdd.cyou

================================================================================
来源：http://sjx.fanxiaobao.xyz

C. 函数与作用域
来源：http://jmw.aizwys.cn

================================================================================
来源：http://zta.yj20258.top

[C01] 定义函数
来源：http://nkr.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://etd.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qcu.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://kkr.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hic.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lwz.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://slr.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://nie.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lej.yj20258.top

[C02] 默认参数
来源：http://wtd.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://cln.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lia.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://vih.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://pqc.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wzg.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vqe.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://aqy.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://hut.ybcxt.top

[C03] 可变参数
来源：http://jga.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://tsp.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xwm.snrcjt.cn


<!-- 参考信息 -->