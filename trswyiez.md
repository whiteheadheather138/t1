代发 wailian999

Py:   "第一行\n第二行"
来源：http://cah.tanke756.top

PHP:  "第一行\n第二行"
来源：http://waw.tanke756.top

JS:   "第一行\n第二行"
来源：http://ibc.dashuyun.cn

TS:   "第一行\n第二行"
来源：http://gsn.haohaochexian.top

Java: "第一行\n第二行"
来源：http://ewn.dianchejie.cn

Go:   "第一行\n第二行"
来源：http://jxa.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://bdt.daxiang520.top

C#:   "第一行\n第二行"
来源：http://xiv.zdqjudy.top

[A14] 注释写法
来源：http://eib.hysaishi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rua.xingfuxueyuan.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://nzb.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://eze.guannengcc.top

TS:   // 单行；/* 多行 */
来源：http://jtm.bbcook.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hnv.jianghu66.top

Go:   // 单行；/* 多行 */
来源：http://eht.redwolf501.top

Ruby: # 单行；=begin 多行 =end
来源：http://wuf.chenlongwang.top

C#:   // 单行；/* 多行 */
来源：http://oci.hammf.cn

[A15] 空值判断与默认值
来源：http://nmr.shanyushiyangtech.top

Py:   value = data or "默认值"
来源：http://equ.cqqwz.cn

PHP:  $value = $data ?? "默认值";
来源：http://ecp.ivvv.top

JS:   const value = data ?? "默认值";
来源：http://fcn.zhoulong.xyz

TS:   const value = data ?? "默认值";
来源：http://eyn.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://scy.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://gyx.yonumen.top

Ruby: value = data || "默认值"
来源：http://igl.zdbjq.cn

C#:   var value = data ?? "默认值";
来源：http://qnv.jinqigufen.top

[A16] 真假值判断规则
来源：http://ypg.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zqr.hcnkem.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ycw.sjlbkw.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xma.yongpay.top

TS:   if (!x) {}
来源：http://ymo.iojbl.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kyw.hesvh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sdk.shzxlz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xqs.redwolf501.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://osr.hnqzz.top

[A17] 位运算
来源：http://nhs.zdqjudy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://neh.dianchejie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yqy.guowangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nxa.fanxiaobao.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xnd.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzf.nanxinkj.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://inn.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tgr.shanyushiyangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://neg.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://gcl.jyoumei.cn

Py:   ord("A"); chr(65)
来源：http://woo.tarul.cn

PHP:  ord("A"); chr(65)
来源：http://kif.fanxiaobao.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ald.kuanghao11.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cyr.ywan-chungtsiang.top

Java: (int) 'A'; (char) 65
来源：http://xym.52xcode.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pyg.ivvv.top

Ruby: "A".ord; 65.chr
来源：http://rdv.yuanzhike.top

C#:   (int)'A'; (char)65
来源：http://epl.shangyingyoupin.top

[A19] 交换两个变量
来源：http://pca.yj20258.top

Py:   a, b = b, a
来源：http://yjx.hesvh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://law.yj20258.top

JS:   [a, b] = [b, a];
来源：http://guw.bbcook.cn

TS:   [a, b] = [b, a];
来源：http://hwq.jinqigufen.top

Java: int t = a; a = b; b = t;
来源：http://gkq.meibo888.top

Go:   a, b = b, a
来源：http://iyf.cashguo.top

Ruby: a, b = b, a
来源：http://fux.nanxinkj.top

C#:   (a, b) = (b, a);
来源：http://wsl.sxryk.cn

[A20] 读取标准输入
来源：http://xwx.feifeiyinyue.top

Py:   name = input("请输入：")
来源：http://mdj.ywan-chungtsiang.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ydl.xinyue.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bxj.chenjidiqi.icu

TS:   // Node.js：readline 模块
来源：http://sty.0kj1m.cn

Java: new Scanner(System.in).nextLine()
来源：http://tgr.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://syc.hnqzz.top

Ruby: gets.chomp
来源：http://qpa.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://fmo.yongpay.top

[A21] 保留指定小数位输出
来源：http://pzz.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://imi.gaohongyu789.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nab.yueranfly.top

JS:   (3.14159).toFixed(2)
来源：http://wnm.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://bek.shanyushiyangtech.top

Java: String.format("%.2f", 3.14159)
来源：http://bfk.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nst.fktsv.cn

Ruby: format("%.2f", 3.14159)
来源：http://mpx.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://nih.jinghuilouyu.cn

[A22] 获取字符串长度
来源：http://zig.jyoumei.cn

Py:   len(s)
来源：http://qyg.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cti.cashguo.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hmp.nanxuanxn.top

TS:   s.length
来源：http://lsm.zhaomingkeji.xyz

Java: s.length()
来源：http://ztw.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://udy.zhiwuduotai.top

Ruby: s.length
来源：http://sfw.vqdsnc.cn

C#:   s.Length
来源：http://ify.daxiang520.top

[A23] 大小写转换
来源：http://mzv.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://uqv.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://grs.yvedp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yar.shuidangran.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gzt.xziqi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sfw.jinqigfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pef.nwbrower.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yvi.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://euj.hongshengwenyu.top

[A24] 去除首尾空白
来源：http://gvj.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jqy.zhongyouzk.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dng.mhx1999.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lpl.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gcm.zhixingplan.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lha.zhijiandao.cn

Go:   strings.TrimSpace(s)
来源：http://dgw.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fia.shanyushiyangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kao.guannengcc.top

[A25] 字符串比较
来源：http://iam.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://vvu.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ojl.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tdg.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xnh.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lnt.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kgv.jqgfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ivg.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tko.shzxlz.cn

[A26] 类型转换总览
来源：http://mrn.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dwx.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wkj.xinyue.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bha.sweek.top

TS:   Number() String() Boolean() x as number
来源：http://aab.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uii.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yfx.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tiu.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jjf.nwbrower.top

================================================================================
来源：http://dup.zhiwuduotai.top

B. 流程控制
来源：http://keh.uphjek.com

================================================================================
来源：http://ixk.yj20258888.top

[B01] 条件判断 if / else
来源：http://kmu.redwolf501.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kct.yanxiufei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kiw.shanyushiyangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kux.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ble.gzhubu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lmy.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wij.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://byf.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kys.hnqzz.top

[B02] 多分支 else if / elif
来源：http://hni.52xcode.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qky.cdnleiting.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oqb.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://itv.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eyv.ywan-chungtsiang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mzg.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kdr.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bav.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yre.tanke756.top

[B03] switch / match / case
来源：http://kbf.jinyuanbaomall.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rhg.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qpp.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yka.hnxiangtu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mqy.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ixe.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ivg.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lse.tianlin.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zbj.yj20258.top

[B04] for 计数循环
来源：http://uzl.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://mkr.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nom.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uvv.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znz.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qmt.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pnc.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://qng.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baj.316326.xyz

[B05] 遍历数组 / 列表
来源：http://hte.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://buk.fengsongda.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://spz.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qhc.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hdl.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wpe.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lmf.cheryme.top

Ruby: arr.each { |item| puts item }
来源：http://bfo.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tte.tarul.cn

[B06] 遍历字典 / 对象
来源：http://lmc.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://jvp.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://igi.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iyo.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dft.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mts.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ovu.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jrh.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://itp.ydjk.org.cn

[B07] while 循环
来源：http://wqk.vehdjk.com

Py:   while i < 10: i += 1
来源：http://zca.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://con.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://bcg.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://hju.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://yll.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dqe.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://pjt.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://xvh.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://sgy.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://phr.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://srz.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://oxc.hnqzz.top

TS:   do { i++; } while (i < 10);
来源：http://dqb.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://nvm.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://eep.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://rkg.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://eht.yuanzhike.top

[B09] break 与 continue
来源：http://ggw.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dec.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kxm.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtv.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qun.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kvy.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tfh.hesvh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ssv.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zkd.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://nep.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nck.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lpt.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vmf.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ole.sufxvd.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://grh.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tde.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://drz.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pkz.pycfn.com

[B11] 生成数字序列 / 区间
来源：http://hat.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://dkz.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://ijw.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blv.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hbr.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sps.fktsv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rnw.jianghu66.top

Ruby: (0...10).step(2).to_a
来源：http://oci.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fks.tanke756.top

[B12] 跳出多层循环
来源：http://axp.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jta.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ytz.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tfb.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cvk.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://poc.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rea.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hnc.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ilv.hfpthk.cn

[B13] 判断是否为数字
来源：http://wqa.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://ssg.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://oxh.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ljy.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wfj.guannengcc.top

Java: x instanceof Number
来源：http://wzq.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://css.xylfe.cn

Ruby: x.is_a?(Numeric)
来源：http://hvi.smart0.xyz

C#:   x is int or double or decimal
来源：http://vtq.tanke756.top

[B14] 判断值是否在集合内
来源：http://rqt.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uem.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vtr.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://bng.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://wqf.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://snl.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wpu.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kry.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yvb.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://iit.52xcode.cn

Py:   a and b or not c
来源：http://byv.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://ycg.pycfn.com

JS:   a && b || !c
来源：http://noy.zdbjq.cn

TS:   a && b || !c
来源：http://mql.guowangkeji.top

Java: a && b || !c
来源：http://kuy.gogol.net.cn

Go:   a && b || !c
来源：http://sky.yuanzhike.top

Ruby: a && b || !c
来源：http://xkx.fengsongda.top

C#:   a && b || !c
来源：http://bol.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ohg.yongpay.top

Py:   if not data: return
来源：http://vmf.chenjidiqi.icu

PHP:  if (!$data) { return; }
来源：http://sjl.yj20258.top

JS:   if (!data) return;
来源：http://gqz.ehwqpu.com

TS:   if (!data) return;
来源：http://npa.dashuyun.cn

Java: if (data == null) return;
来源：http://kgn.hysaishi.cn

Go:   if data == nil { return }
来源：http://vcv.fktsv.cn

Ruby: return if data.nil?
来源：http://xli.fzhhl.top

C#:   if (data == null) return;
来源：http://zit.fktsv.cn

================================================================================
来源：http://leo.cheryme.top

C. 函数与作用域
来源：http://ysd.havefunace.top

================================================================================
来源：http://nvy.sxryk.cn

[C01] 定义函数
来源：http://vjz.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://noc.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bwn.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://ojf.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://upl.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zbp.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://ccv.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://mko.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ngx.fanxiaobao.xyz

[C02] 默认参数
来源：http://bxv.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://ihj.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://haj.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://kup.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://obg.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sbq.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ebs.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://zax.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://uyy.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://xii.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://rqr.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vjq.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lov.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://diz.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gge.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dmn.jinyuanbaomall.cn


<!-- 参考信息 -->