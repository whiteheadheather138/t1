代发 wailian999

Py:   "第一行\n第二行"
来源：http://ztl.sjlbkw.cn

PHP:  "第一行\n第二行"
来源：http://wyv.jinyuanbaomall.cn

JS:   "第一行\n第二行"
来源：http://ktb.ybcxt.top

TS:   "第一行\n第二行"
来源：http://dvy.0kj1m.cn

Java: "第一行\n第二行"
来源：http://cxm.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://shj.ctjpmb.com

Ruby: "第一行\n第二行"
来源：http://ptn.sxryk.cn

C#:   "第一行\n第二行"
来源：http://iqi.yvedp.cn

[A14] 注释写法
来源：http://gms.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mhd.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qti.redwolf501.top

JS:   // 单行；/* 多行 */
来源：http://sun.daxiang520.top

TS:   // 单行；/* 多行 */
来源：http://nah.nanxinkj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://got.zdqjudy.top

Go:   // 单行；/* 多行 */
来源：http://mhe.yanxiufei.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dvk.yuxming.cn

C#:   // 单行；/* 多行 */
来源：http://fxc.pycfn.com

[A15] 空值判断与默认值
来源：http://hng.jinghuilouyu.cn

Py:   value = data or "默认值"
来源：http://wnn.hongshengwenyu.top

PHP:  $value = $data ?? "默认值";
来源：http://jow.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://olq.mhx1999.top

TS:   const value = data ?? "默认值";
来源：http://llt.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dix.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://jhw.cashguo.top

Ruby: value = data || "默认值"
来源：http://nvd.shanyushiyangkeji.top

C#:   var value = data ?? "默认值";
来源：http://pfu.hysaishi.cn

[A16] 真假值判断规则
来源：http://tcj.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ukh.gaohongyu789.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ahy.ctjpmb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://exh.bjfxy.top

TS:   if (!x) {}
来源：http://ylg.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vid.gogol.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cpp.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://dtj.cdnleiting.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://moa.gaohongyu789.top

[A17] 位运算
来源：http://fgt.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rtz.meibo888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ret.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jhv.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nae.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ywh.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jkb.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bzd.wangdashe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fkc.9152youxi.cn

[A18] 字符与 ASCII 码互转
来源：http://zah.ydjk.org.cn

Py:   ord("A"); chr(65)
来源：http://kby.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://qwf.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vln.zdqjudy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://svh.tian-w.cn

Java: (int) 'A'; (char) 65
来源：http://ail.gotoacloud.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gpu.yangfankeji.com

Ruby: "A".ord; 65.chr
来源：http://fxk.fanxiaobao.xyz

C#:   (int)'A'; (char)65
来源：http://dyr.tian-w.cn

[A19] 交换两个变量
来源：http://txx.sysykeji.top

Py:   a, b = b, a
来源：http://ojv.chenzaomai.com

PHP:  [$a, $b] = [$b, $a];
来源：http://fvo.quarkkingdee.top

JS:   [a, b] = [b, a];
来源：http://eah.shanyushiyangkeji.top

TS:   [a, b] = [b, a];
来源：http://cpz.quarkkingdee.top

Java: int t = a; a = b; b = t;
来源：http://szb.aibaodan.cn

Go:   a, b = b, a
来源：http://avn.shangyingyoupin.top

Ruby: a, b = b, a
来源：http://osx.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://ult.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://lnz.zdbjq.cn

Py:   name = input("请输入：")
来源：http://wqf.kuanghao11.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hbl.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fbl.sxryk.cn

TS:   // Node.js：readline 模块
来源：http://cgg.yj20258.top

Java: new Scanner(System.in).nextLine()
来源：http://skk.jinqigufen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fxh.guannengcc.top

Ruby: gets.chomp
来源：http://uah.vehdjk.com

C#:   Console.ReadLine();
来源：http://xjf.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://wcb.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://qxo.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cuh.guowangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://jds.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://qhr.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://lbl.jinyuanbaomall.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://riz.meibo888.top

Ruby: format("%.2f", 3.14159)
来源：http://fgh.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://ahl.bjfxy.top

[A22] 获取字符串长度
来源：http://clt.nwbrower.top

Py:   len(s)
来源：http://rru.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://giy.uphjek.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oow.9152youxi.cn

TS:   s.length
来源：http://oan.tanke756.top

Java: s.length()
来源：http://pdq.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mng.daria6918.cn

Ruby: s.length
来源：http://puz.pycfn.com

C#:   s.Length
来源：http://off.pengpengdd.cyou

[A23] 大小写转换
来源：http://gyf.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dpv.xinyue.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yix.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ffc.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zzz.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xli.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lve.yuxming.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bhx.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rnl.hnqzz.top

[A24] 去除首尾空白
来源：http://edw.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://axq.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://khp.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kxn.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dfs.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qzi.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://ufx.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fti.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cze.jinghuilouyu.cn

[A25] 字符串比较
来源：http://cbd.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://exz.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wyd.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ykl.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pca.shuidangran.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ekk.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jlf.fzhhl.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uxm.epnwcf.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mti.cqqwz.cn

[A26] 类型转换总览
来源：http://zgu.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ovf.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wmp.hnxiangtu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bvg.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://lds.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wir.zhiwuduotai.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sdp.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://usd.tianlin.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bye.xuetiantiany.cn

================================================================================
来源：http://rzg.ydjk.org.cn

B. 流程控制
来源：http://uqo.gzhubu.top

================================================================================
来源：http://cpq.fehbvm.com

[B01] 条件判断 if / else
来源：http://wyt.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mnk.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://etr.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://enj.nanxuanxn.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mwp.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://kai.gogol.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lkb.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hjx.chenjidiqi.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yok.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://kvt.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cwd.chenlongwang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nxs.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jpy.hammf.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdl.sysykeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://six.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://usu.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ats.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pgw.guannengcc.top

[B03] switch / match / case
来源：http://szh.dianchejie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ylk.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dgo.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://azo.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rxb.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ykk.snrcjt.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iug.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cue.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ycn.gaohongyu789.top

[B04] for 计数循环
来源：http://lom.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://yhc.xuanzx.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kfw.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zdl.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hjf.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jpp.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mmk.ivvv.top

Ruby: 10.times { |i| puts i }
来源：http://fbt.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jdp.daria6918.cn

[B05] 遍历数组 / 列表
来源：http://vuq.ybcxt.top

Py:   for item in arr: print(item)
来源：http://nye.shanyushiyangtech.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xsv.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lig.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://slt.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dtf.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mdn.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://bfn.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kbd.cashguo.top

[B06] 遍历字典 / 对象
来源：http://xxc.zdbjq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://csh.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fvm.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://teu.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vlp.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://srs.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kkr.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vfy.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pkk.shanyushiyangkeji.top

[B07] while 循环
来源：http://qtu.daxiang520.top

Py:   while i < 10: i += 1
来源：http://uft.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nbj.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://qjf.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://upp.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://hgu.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aat.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://dcb.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://kyq.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://iow.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://skp.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zzw.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://ewx.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://dow.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://cyi.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://niz.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cza.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://ihf.sysykeji.top

[B09] break 与 continue
来源：http://uth.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xge.yanxiufei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yoh.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mop.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ktf.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qqj.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://thy.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://anv.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jiu.birdmap.top

[B10] 遍历同时拿索引
来源：http://dit.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jjo.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tnr.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wzm.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mbp.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pph.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://msf.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://njg.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xxz.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://hrf.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://mlz.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://dyq.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ral.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ixs.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dce.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wro.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://lgo.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wyo.jlsjyb.cn

[B12] 跳出多层循环
来源：http://sxf.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://lou.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nig.zhaomingkeji.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yfa.yj202588.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jrr.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mam.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rwg.zdqjudy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ofi.shuidangran.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pwc.tian-w.cn

[B13] 判断是否为数字
来源：http://uxt.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://vbs.fzhhl.top

PHP:  is_numeric($x)
来源：http://vlk.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yjp.cashguo.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zyi.jiagoushi.top

Java: x instanceof Number
来源：http://wdy.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yxz.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://niu.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://vyb.yfazqb.com

[B14] 判断值是否在集合内
来源：http://fzp.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ury.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://exr.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://xpe.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://chp.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tsd.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sdu.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://ota.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://scx.mhx1999.top

[B15] 布尔运算与取反
来源：http://gzv.zhiwuduotai.top

Py:   a and b or not c
来源：http://ksk.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://uoh.hesvh.cn

JS:   a && b || !c
来源：http://vou.ppjwa.cn

TS:   a && b || !c
来源：http://gjh.hnqzz.top

Java: a && b || !c
来源：http://qfz.xylfe.cn

Go:   a && b || !c
来源：http://vzc.hysaishi.cn

Ruby: a && b || !c
来源：http://xeo.fanxiaobao.xyz

C#:   a && b || !c
来源：http://voe.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://xqr.fanxiaobao.xyz

Py:   if not data: return
来源：http://cnc.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://htn.ybcxt.top

JS:   if (!data) return;
来源：http://pxk.zdqjudy.top

TS:   if (!data) return;
来源：http://ygf.cqqwz.cn

Java: if (data == null) return;
来源：http://sft.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://epb.fzhhl.top

Ruby: return if data.nil?
来源：http://soi.nanxinkj.top

C#:   if (data == null) return;
来源：http://jdk.hcnkem.com

================================================================================
来源：http://mnj.aibaodan.cn

C. 函数与作用域
来源：http://nld.chenzaomai.com

================================================================================
来源：http://syh.ybcxt.top

[C01] 定义函数
来源：http://tiy.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://ueb.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://btw.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://idn.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnb.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pct.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vrw.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://erx.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jkx.guannengcc.top

[C02] 默认参数
来源：http://gha.cashguo.top

Py:   def greet(name="World"): return name
来源：http://bna.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dij.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://mdn.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sqx.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gnq.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ckx.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://nro.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://aqy.fktsv.cn

[C03] 可变参数
来源：http://nnb.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://wwe.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fxz.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rim.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wjh.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qre.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rab.mhx1999.top


<!-- 参考信息 -->