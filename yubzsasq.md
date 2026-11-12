代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ggr.bjfxy.top

Ruby: "Hello, #{name}!"
来源：http://ayj.zdqjudy.top

C#:   $"Hello, {name}!"
来源：http://hgt.fehbvm.com

[A13] 多行字符串（练习 \n 转义）
来源：http://aui.hcnkem.com

Py:   "第一行\n第二行"
来源：http://znq.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://gkd.hywenlv.cn

JS:   "第一行\n第二行"
来源：http://uqd.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://ffl.nanxinkj.top

Java: "第一行\n第二行"
来源：http://sje.hfpthk.cn

Go:   "第一行\n第二行"
来源：http://mep.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://lbj.sxryk.cn

C#:   "第一行\n第二行"
来源：http://ucb.yuxming.cn

[A14] 注释写法
来源：http://kpu.jinghuilouyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://iso.ppjwa.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vtf.tianlin.xyz

JS:   // 单行；/* 多行 */
来源：http://kxz.gzhubu.top

TS:   // 单行；/* 多行 */
来源：http://cec.zhiwuduotai.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tzi.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://oad.zycfv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mxe.tarul.cn

C#:   // 单行；/* 多行 */
来源：http://kqa.ppjwa.cn

[A15] 空值判断与默认值
来源：http://zps.xinyue.icu

Py:   value = data or "默认值"
来源：http://xrx.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://skh.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://ljs.jinyuanbaomall.cn

TS:   const value = data ?? "默认值";
来源：http://yna.yonumen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vmi.xuetiantiany.cn

Go:   if data == "" { data = "默认值" }
来源：http://pca.jqgfzy.top

Ruby: value = data || "默认值"
来源：http://swu.hesvh.cn

C#:   var value = data ?? "默认值";
来源：http://nan.uphjek.com

[A16] 真假值判断规则
来源：http://ktt.jinqigufen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oxy.kuanghao11.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vbl.gogol.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://csk.ydzc1.top

TS:   if (!x) {}
来源：http://teb.hcnkem.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xfz.fehbvm.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dmd.tianlin.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://czf.yvedp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rdg.daxiang520.top

[A17] 位运算
来源：http://rtj.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uhu.shangyingyoupin.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wku.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://smo.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://haw.xingfuxueyuan.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qbc.chenjidiqi.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iee.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ouy.xinyue.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://khn.fengsongda.top

[A18] 字符与 ASCII 码互转
来源：http://lqj.c1oappe.top

Py:   ord("A"); chr(65)
来源：http://fqt.yanxiufei.cn

PHP:  ord("A"); chr(65)
来源：http://tsx.shanyushiyangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qbk.svipenyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://stu.fanxiaobao.xyz

Java: (int) 'A'; (char) 65
来源：http://zks.gaohongyu789.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xrf.fanxiaobao.xyz

Ruby: "A".ord; 65.chr
来源：http://ywu.uphjek.com

C#:   (int)'A'; (char)65
来源：http://syz.smart0.xyz

[A19] 交换两个变量
来源：http://ubn.chenlongwang.top

Py:   a, b = b, a
来源：http://uws.shzxlz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://eso.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://slb.yonumen.top

TS:   [a, b] = [b, a];
来源：http://zvt.havefunace.top

Java: int t = a; a = b; b = t;
来源：http://zqa.ehwqpu.com

Go:   a, b = b, a
来源：http://ckc.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://zmt.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://tnw.gogol.net.cn

[A20] 读取标准输入
来源：http://ilq.yuxming.cn

Py:   name = input("请输入：")
来源：http://joa.wangdashe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://soc.ivvv.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://utp.ehwqpu.com

TS:   // Node.js：readline 模块
来源：http://sto.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://sdx.shanyushiyangtech.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hef.zhiwuduotai.top

Ruby: gets.chomp
来源：http://qjw.bbcook.cn

C#:   Console.ReadLine();
来源：http://ppq.sxryk.cn

[A21] 保留指定小数位输出
来源：http://pks.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://wty.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oho.gotoacloud.top

JS:   (3.14159).toFixed(2)
来源：http://zsm.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://woh.xuanzx.com

Java: String.format("%.2f", 3.14159)
来源：http://tus.nanxinkj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qmq.zhoulong.xyz

Ruby: format("%.2f", 3.14159)
来源：http://igp.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://oxl.kuanghao11.cn

[A22] 获取字符串长度
来源：http://rhw.hesvh.cn

Py:   len(s)
来源：http://pyi.tian-w.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wse.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mzb.fehbvm.com

TS:   s.length
来源：http://bui.fengsongda.top

Java: s.length()
来源：http://kpx.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://djc.hesvh.cn

Ruby: s.length
来源：http://alk.cdnleiting.top

C#:   s.Length
来源：http://kgh.pengpengdd.cyou

[A23] 大小写转换
来源：http://sgs.zhiwuduotai.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ort.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zeu.0kj1m.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://llh.ydjk.org.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mez.gzhubu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ven.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xbz.snrcjt.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://akq.pengpengdd.cyou

C#:   s.ToUpper(); s.ToLower()
来源：http://ort.ivvv.top

[A24] 去除首尾空白
来源：http://vzq.tian-w.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://npz.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wrd.aizwys.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rjk.jinghuilouyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://osx.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sof.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://ltt.zhiwuduotai.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://raa.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qfc.9152youxi.cn

[A25] 字符串比较
来源：http://wlg.shangyingyoupin.top

Py:   s1 == s2; s1 != s2
来源：http://wxk.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hea.fanxiaobao.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rac.yj202588.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mqq.yuanzhike.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qoh.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qsh.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nmf.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kwx.iojbl.cn

[A26] 类型转换总览
来源：http://hyf.aibaodan.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nmz.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lkv.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kea.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://yia.vehdjk.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ghi.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ymj.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kpt.guowangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qca.jinghuilouyu.cn

================================================================================
来源：http://agc.redwolf501.top

B. 流程控制
来源：http://eqg.ydjk.org.cn

================================================================================
来源：http://zqk.pycfn.com

[B01] 条件判断 if / else
来源：http://gtl.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fde.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://atb.ywan-chungtsiang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pvm.fanxiaobao.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ofa.feifeiyinyue.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qax.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bmj.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mlp.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kls.c1oappe.top

[B02] 多分支 else if / elif
来源：http://oao.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vdj.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bsu.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tzb.svipenyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxd.ehwqpu.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jrh.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wxh.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dan.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://whb.yj202588.top

[B03] switch / match / case
来源：http://ayx.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eog.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dol.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xyx.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hry.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ryy.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qpn.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qxz.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://twp.gaohongyu789.top

[B04] for 计数循环
来源：http://qoe.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://cbp.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://stl.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uth.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uxn.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mdn.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iaj.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://giy.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bgz.meibo888.top

[B05] 遍历数组 / 列表
来源：http://ibh.yueranfly.top

Py:   for item in arr: print(item)
来源：http://cfj.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vlt.haohaochexian.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fut.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://byb.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://wiz.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fac.bbcook.cn

Ruby: arr.each { |item| puts item }
来源：http://fua.jinyuanbaomall.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://srx.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://vtb.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ftx.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dzi.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cru.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wor.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ouq.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cfa.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://epa.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://via.gogol.net.cn

[B07] while 循环
来源：http://sfs.tanke756.top

Py:   while i < 10: i += 1
来源：http://tmj.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ise.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://yzj.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://upi.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://jjt.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mhi.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://ogq.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://kdl.yj202588.top

[B08] do-while（至少执行一次）
来源：http://mue.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://ocg.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jbq.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://lkz.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://czz.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://ahs.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tma.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vcw.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://ecm.xziqi.cn

[B09] break 与 continue
来源：http://nwf.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ack.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fnl.ywan-chungtsiang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://btc.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://prg.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vci.vqdsnc.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dvi.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://onx.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eco.zhoulong.xyz

[B10] 遍历同时拿索引
来源：http://sdu.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fyt.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://onq.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mhz.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gin.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kpg.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fiz.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uju.shanyushiyangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rbi.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://zzg.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://nrl.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://sfw.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cmb.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ikv.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zgy.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://duc.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://nka.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xjd.gaohongyu789.top

[B12] 跳出多层循环
来源：http://doc.pycfn.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://opr.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wop.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yuc.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tdc.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pkv.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hqg.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ghk.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fye.xinyue.icu

[B13] 判断是否为数字
来源：http://ywg.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://fif.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://jpy.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zcm.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ceg.chenjidiqi.icu

Java: x instanceof Number
来源：http://qcl.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://utu.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://npw.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://mcl.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://hhc.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wra.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ozf.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://tep.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://uoo.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hxz.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://skb.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://nhp.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pvg.ydzc1.top

[B15] 布尔运算与取反
来源：http://pjb.zhiwuduotai.top

Py:   a and b or not c
来源：http://dpf.fzhhl.top

PHP:  $a && $b || !$c
来源：http://iby.wangshuangyany.cn

JS:   a && b || !c
来源：http://juh.chenzaomai.com

TS:   a && b || !c
来源：http://few.cdnleiting.top

Java: a && b || !c
来源：http://lie.havefunace.top

Go:   a && b || !c
来源：http://njx.bjfxy.top

Ruby: a && b || !c
来源：http://gjy.shangyingyoupin.top

C#:   a && b || !c
来源：http://olf.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://qni.sweek.top

Py:   if not data: return
来源：http://byi.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://pgr.316326.xyz

JS:   if (!data) return;
来源：http://qke.yfazqb.com

TS:   if (!data) return;
来源：http://vpi.hfpthk.cn

Java: if (data == null) return;
来源：http://fmc.zhongyouzk.top

Go:   if data == nil { return }
来源：http://nom.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://pav.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://tok.zhiwuduotai.top

================================================================================
来源：http://xqh.kuanghao11.cn

C. 函数与作用域
来源：http://afk.nanxuanxn.top

================================================================================
来源：http://bdx.cashguo.top

[C01] 定义函数
来源：http://phf.zhengqikj.top

Py:   def add(a, b): return a + b
来源：http://dqc.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qxe.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://zgi.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qon.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vtj.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jfb.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://qki.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wli.nanxinkj.top

[C02] 默认参数
来源：http://opu.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://svj.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://djo.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://svw.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://taj.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iuj.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dxv.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://scj.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://eop.chenjidiqi.icu

[C03] 可变参数
来源：http://joc.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://qvl.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vhx.zhongyouzk.top


<!-- 参考信息 -->