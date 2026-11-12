代发 wailian999

Java: "第一行\n第二行"
来源：http://oqa.jinqigfzy.top

Go:   "第一行\n第二行"
来源：http://ohu.pycfn.com

Ruby: "第一行\n第二行"
来源：http://cqo.yj202588.top

C#:   "第一行\n第二行"
来源：http://fgc.hnqzz.top

[A14] 注释写法
来源：http://nar.cucudq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vox.nwbrower.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xpu.tian-w.cn

JS:   // 单行；/* 多行 */
来源：http://mal.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://lfp.jqgfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ccx.zhoulong.xyz

Go:   // 单行；/* 多行 */
来源：http://tja.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://jbe.chenlongwang.top

C#:   // 单行；/* 多行 */
来源：http://aas.xuanzx.com

[A15] 空值判断与默认值
来源：http://esq.ctjpmb.com

Py:   value = data or "默认值"
来源：http://cix.xinyue.icu

PHP:  $value = $data ?? "默认值";
来源：http://jus.52xcode.cn

JS:   const value = data ?? "默认值";
来源：http://rig.tanke756.top

TS:   const value = data ?? "默认值";
来源：http://ehn.jinyuanbaomall.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xyn.redwolf501.top

Go:   if data == "" { data = "默认值" }
来源：http://hko.0kj1m.cn

Ruby: value = data || "默认值"
来源：http://skp.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://ios.zhaomingkeji.xyz

[A16] 真假值判断规则
来源：http://lnw.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qja.jinqigfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hfw.zdbjq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nje.yj20258888.top

TS:   if (!x) {}
来源：http://tuv.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bxp.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wkb.hongshengwenyu.top

Ruby: unless x            # nil 与 false 为假
来源：http://slg.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ezq.xinyue.icu

[A17] 位运算
来源：http://fvz.jianghu66.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://epd.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kup.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnl.tian-w.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ltp.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blm.yj20258.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nbg.tarul.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oha.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gao.yongpay.top

[A18] 字符与 ASCII 码互转
来源：http://gzc.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://qhe.yonumen.top

PHP:  ord("A"); chr(65)
来源：http://tcx.vqdsnc.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ite.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kln.mhx1999.top

Java: (int) 'A'; (char) 65
来源：http://dcc.havefunace.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ont.yonumen.top

Ruby: "A".ord; 65.chr
来源：http://rga.ctjpmb.com

C#:   (int)'A'; (char)65
来源：http://aqg.jqgufenzy.top

[A19] 交换两个变量
来源：http://xso.fzhhl.top

Py:   a, b = b, a
来源：http://xpg.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://skr.jinghuilouyu.cn

JS:   [a, b] = [b, a];
来源：http://hzl.hnqzz.top

TS:   [a, b] = [b, a];
来源：http://ods.jqgufenzy.top

Java: int t = a; a = b; b = t;
来源：http://gio.nwbrower.top

Go:   a, b = b, a
来源：http://vuf.vqdsnc.cn

Ruby: a, b = b, a
来源：http://eii.xziqi.cn

C#:   (a, b) = (b, a);
来源：http://ppj.jianghu66.top

[A20] 读取标准输入
来源：http://gwr.epnwcf.com

Py:   name = input("请输入：")
来源：http://bwg.ydzc1.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tqr.birdmap.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jjj.dashuyun.cn

TS:   // Node.js：readline 模块
来源：http://kdd.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://tff.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jot.ydjk.org.cn

Ruby: gets.chomp
来源：http://cgr.meibo888.top

C#:   Console.ReadLine();
来源：http://rvp.zhixingplan.top

[A21] 保留指定小数位输出
来源：http://gsr.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://sdn.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ars.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://gpm.ehwqpu.com

TS:   (3.14159).toFixed(2)
来源：http://bxa.feifeiyinyue.top

Java: String.format("%.2f", 3.14159)
来源：http://hxl.xuanzx.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bai.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://kah.cucudq.cn

C#:   3.14159.ToString("F2")
来源：http://ddc.yueranfly.top

[A22] 获取字符串长度
来源：http://rnj.jinqigufen.top

Py:   len(s)
来源：http://bvd.haohaochexian.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qqp.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mmx.zdbjq.cn

TS:   s.length
来源：http://gdh.9152youxi.cn

Java: s.length()
来源：http://npy.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wee.hfpthk.cn

Ruby: s.length
来源：http://dpn.ydzc1.top

C#:   s.Length
来源：http://tut.jinqigufen.top

[A23] 大小写转换
来源：http://aqn.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://zwa.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rqa.haohaochexian.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pzf.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ygg.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bwe.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eoo.tarul.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mbb.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://yys.zhiwuduotai.top

[A24] 去除首尾空白
来源：http://fxx.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://svc.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ebd.yanxiufei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hao.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mwc.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xvx.zhongyouzk.top

Go:   strings.TrimSpace(s)
来源：http://nfm.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tfw.tian-w.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wfb.yongpay.top

[A25] 字符串比较
来源：http://ayi.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://wsu.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sro.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hax.nwbrower.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://voc.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qsg.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://avo.yfazqb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://hpj.shangyingyoupin.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ilc.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://ics.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gda.haohaochexian.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jzm.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eln.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://lbd.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eww.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wof.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ogj.zhoulong.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://igs.kuanghao11.cn

================================================================================
来源：http://wqf.uphjek.com

B. 流程控制
来源：http://vtj.chenlongwang.top

================================================================================
来源：http://cqd.chenzaomai.com

[B01] 条件判断 if / else
来源：http://eue.xziqi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wbb.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tqt.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gpx.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fcw.snrcjt.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xen.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nuz.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gdm.xingfuxueyuan.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aat.zhoulong.xyz

[B02] 多分支 else if / elif
来源：http://pap.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ngb.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jzs.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wtk.jqgfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozl.ywan-chungtsiang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zim.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xxg.feifeiyinyue.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zgu.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://stu.gogol.net.cn

[B03] switch / match / case
来源：http://zxx.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xdn.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rim.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tjl.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iim.sjlbkw.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://emi.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zyn.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vdv.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xao.tianlin.xyz

[B04] for 计数循环
来源：http://muz.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://guq.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rcg.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ddg.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kmv.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hir.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bam.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://swd.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yyj.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://uuf.aizwys.cn

Py:   for item in arr: print(item)
来源：http://xni.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dhb.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tpu.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://psb.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hub.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kql.zhaomingkeji.xyz

Ruby: arr.each { |item| puts item }
来源：http://gbh.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gfx.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://vxc.jqgufenzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://arc.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vrj.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gro.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uow.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gzw.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mjw.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vsx.xziqi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bgd.jinqigfzy.top

[B07] while 循环
来源：http://rnd.birdmap.top

Py:   while i < 10: i += 1
来源：http://lrm.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://alp.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://okp.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://aoq.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://jnv.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cnz.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://fky.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://wfh.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://txx.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://jov.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://vve.xziqi.cn

JS:   do { i++; } while (i < 10);
来源：http://bkp.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://jpz.shzxlz.cn

Java: do { i++; } while (i < 10);
来源：http://edw.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sbh.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://lml.sjlbkw.cn

C#:   do { i++; } while (i < 10);
来源：http://vuc.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://aoq.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sdl.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nfj.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gut.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wua.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lfa.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qnu.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xej.meibo888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://whp.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://xgs.dianchejie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vdo.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fwg.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ysw.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jfv.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kws.sufxvd.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://odd.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gaw.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bxq.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://lwv.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://fxc.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://gxt.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gcs.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ikk.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rtx.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://plq.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://gnn.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cmp.fzhhl.top

[B12] 跳出多层循环
来源：http://gnx.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eor.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://yls.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rmz.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cxi.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lyl.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zfd.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kow.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://evg.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://sjo.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://yjz.fktsv.cn

PHP:  is_numeric($x)
来源：http://lrc.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fwc.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://znl.snrcjt.cn

Java: x instanceof Number
来源：http://oze.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rze.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://chi.jinqigufen.top

C#:   x is int or double or decimal
来源：http://tzy.jqgfzy.top

[B14] 判断值是否在集合内
来源：http://zxe.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ppk.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rnq.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://vin.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://wfv.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hkl.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vtb.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lbl.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kse.yuanzhike.top

[B15] 布尔运算与取反
来源：http://qwx.gaohongyu789.top

Py:   a and b or not c
来源：http://crs.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://zxl.zycfv.cn

JS:   a && b || !c
来源：http://uwb.hongshengwenyu.top

TS:   a && b || !c
来源：http://mmt.yonumen.top

Java: a && b || !c
来源：http://chg.aizwys.cn

Go:   a && b || !c
来源：http://lbf.c1oappe.top

Ruby: a && b || !c
来源：http://skm.jinqigfzy.top

C#:   a && b || !c
来源：http://cdd.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://opf.ywan-chungtsiang.top

Py:   if not data: return
来源：http://fkn.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://sfp.fanxiaobao.xyz

JS:   if (!data) return;
来源：http://vdt.sjlbkw.cn

TS:   if (!data) return;
来源：http://odf.svipenyu.cn

Java: if (data == null) return;
来源：http://usw.jianghu66.top

Go:   if data == nil { return }
来源：http://ofp.hfpthk.cn

Ruby: return if data.nil?
来源：http://puv.hammf.cn

C#:   if (data == null) return;
来源：http://lzo.mhx1999.top

================================================================================
来源：http://wpp.ehwqpu.com

C. 函数与作用域
来源：http://auy.kuanghao11.cn

================================================================================
来源：http://ihu.daria6918.cn

[C01] 定义函数
来源：http://niy.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://xql.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wvb.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://nae.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gmt.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ztk.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kfw.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://ttd.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bbu.zhoulong.xyz

[C02] 默认参数
来源：http://ivb.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://hjm.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://tpr.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://cmb.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nfv.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://snv.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mjx.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://lht.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://bjm.ybcxt.top

[C03] 可变参数
来源：http://uyy.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://euw.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ppy.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jpr.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://olg.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mpp.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://djt.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mfn.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gti.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://zlo.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ozw.yvedp.cn


<!-- 参考信息 -->