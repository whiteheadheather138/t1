代发 wailian999

Py:   "第一行\n第二行"
来源：http://dao.snrcjt.cn

PHP:  "第一行\n第二行"
来源：http://gce.zhaomingkeji.xyz

JS:   "第一行\n第二行"
来源：http://yhm.zhiwuduotai.top

TS:   "第一行\n第二行"
来源：http://snd.sysykeji.top

Java: "第一行\n第二行"
来源：http://xjt.aizwys.cn

Go:   "第一行\n第二行"
来源：http://kua.zhijiandao.cn

Ruby: "第一行\n第二行"
来源：http://zki.uphjek.com

C#:   "第一行\n第二行"
来源：http://ubs.daria6918.cn

[A14] 注释写法
来源：http://amv.guowangkeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ays.birdmap.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mdl.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://qrv.cdnleiting.top

TS:   // 单行；/* 多行 */
来源：http://yle.yuanzhike.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nwb.jiagoushi.top

Go:   // 单行；/* 多行 */
来源：http://zmr.xinyue.icu

Ruby: # 单行；=begin 多行 =end
来源：http://ubg.xuetiantiany.cn

C#:   // 单行；/* 多行 */
来源：http://hjl.hnqzz.top

[A15] 空值判断与默认值
来源：http://ftz.sjlbkw.cn

Py:   value = data or "默认值"
来源：http://vzu.havefunace.top

PHP:  $value = $data ?? "默认值";
来源：http://icw.fanxiaobao.xyz

JS:   const value = data ?? "默认值";
来源：http://qgp.sxryk.cn

TS:   const value = data ?? "默认值";
来源：http://bdl.havefunace.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gyb.gzhubu.top

Go:   if data == "" { data = "默认值" }
来源：http://gfw.hysaishi.cn

Ruby: value = data || "默认值"
来源：http://lfa.pycfn.com

C#:   var value = data ?? "默认值";
来源：http://xqm.jyoumei.cn

[A16] 真假值判断规则
来源：http://kim.xuetiantiany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://std.shanyushiyangtech.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nct.quarkkingdee.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oua.nanxinkj.top

TS:   if (!x) {}
来源：http://die.jinyuanbaomall.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://unz.zhixingplan.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zeh.yfazqb.com

Ruby: unless x            # nil 与 false 为假
来源：http://zow.yonumen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ffk.sufxvd.cn

[A17] 位运算
来源：http://xyz.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hat.xingfuxueyuan.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jkh.svipenyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ejs.fengsongda.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hfh.zhoulong.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://foe.ywan-chungtsiang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://npb.chenjidiqi.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eof.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jgh.vehdjk.com

[A18] 字符与 ASCII 码互转
来源：http://phe.yueranfly.top

Py:   ord("A"); chr(65)
来源：http://fvq.gaohongyu789.top

PHP:  ord("A"); chr(65)
来源：http://zwq.tarul.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xib.fanxiaobao.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lop.andypj.xyz

Java: (int) 'A'; (char) 65
来源：http://uvr.xziqi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://skn.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://ldu.birdmap.top

C#:   (int)'A'; (char)65
来源：http://set.jlsjyb.cn

[A19] 交换两个变量
来源：http://evk.nanxinkj.top

Py:   a, b = b, a
来源：http://fwu.wangdashe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lzz.xuetiantiany.cn

JS:   [a, b] = [b, a];
来源：http://mqr.fzhhl.top

TS:   [a, b] = [b, a];
来源：http://tsp.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://ylx.svipenyu.cn

Go:   a, b = b, a
来源：http://ser.gotoacloud.top

Ruby: a, b = b, a
来源：http://axk.hfpthk.cn

C#:   (a, b) = (b, a);
来源：http://vif.gzhubu.top

[A20] 读取标准输入
来源：http://xba.zhengqikj.top

Py:   name = input("请输入：")
来源：http://cus.vehdjk.com

PHP:  $name = trim(fgets(STDIN));
来源：http://krk.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bgn.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://hsr.meibo888.top

Java: new Scanner(System.in).nextLine()
来源：http://biv.ppjwa.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fqz.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://yhj.cdnleiting.top

C#:   Console.ReadLine();
来源：http://gbz.daria6918.cn

[A21] 保留指定小数位输出
来源：http://ree.daxiang520.top

Py:   f"{3.14159:.2f}"
来源：http://lqs.shanyushiyangtech.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://efs.vehdjk.com

JS:   (3.14159).toFixed(2)
来源：http://ipl.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://blu.zhiwuduotai.top

Java: String.format("%.2f", 3.14159)
来源：http://rls.guowangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://izj.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://tvj.bbcook.cn

C#:   3.14159.ToString("F2")
来源：http://xnz.wangdashe.top

[A22] 获取字符串长度
来源：http://tsk.jinqigfzy.top

Py:   len(s)
来源：http://tbz.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tyb.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fok.zhijiandao.cn

TS:   s.length
来源：http://lei.zhongyouzk.top

Java: s.length()
来源：http://lgx.jinqigufen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bxj.yongpay.top

Ruby: s.length
来源：http://sjp.haohaochexian.top

C#:   s.Length
来源：http://fiu.shanyushiyangtech.top

[A23] 大小写转换
来源：http://axg.chenzaomai.com

Py:   s.upper(); s.lower(); s.title()
来源：http://fkw.shanyushiyangtech.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zgv.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zou.sufxvd.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rtz.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hjh.shangyingyoupin.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mmt.cheryme.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kxf.bbcook.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://avx.hammf.cn

[A24] 去除首尾空白
来源：http://qtt.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://twk.ivvv.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fgp.tanke756.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oqc.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://azz.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ekq.jinqigufen.top

Go:   strings.TrimSpace(s)
来源：http://qnz.aizwys.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qvz.yuxming.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jet.cdnleiting.top

[A25] 字符串比较
来源：http://shd.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://iyz.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://igo.zhixingplan.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qcx.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lqt.zhongyouzk.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://whh.jinyuanbaomall.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://axk.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ibc.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cww.ivvv.top

[A26] 类型转换总览
来源：http://qsf.tianlin.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://odm.ywan-chungtsiang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sko.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qol.dianchejie.cn

TS:   Number() String() Boolean() x as number
来源：http://oub.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qko.fktsv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jjg.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fxf.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vzk.tarul.cn

================================================================================
来源：http://imk.cqqwz.cn

B. 流程控制
来源：http://nsb.jyoumei.cn

================================================================================
来源：http://ipi.fengsongda.top

[B01] 条件判断 if / else
来源：http://mac.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yqn.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oen.pengpengdd.cyou

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dam.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ltr.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ogo.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cwi.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ljy.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ghe.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://aet.vehdjk.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eic.uphjek.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zvc.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kkn.yj20258.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqk.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qys.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aqb.ydjk.org.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fjn.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fuy.0kj1m.cn

[B03] switch / match / case
来源：http://epl.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fya.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uan.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://she.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bio.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ggu.dianchejie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ajh.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mll.yangfankeji.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mmp.sweek.top

[B04] for 计数循环
来源：http://jee.cashguo.top

Py:   for i in range(10): print(i)
来源：http://lpj.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jbj.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xzr.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pde.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kfg.vqdsnc.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rxa.zhengqikj.top

Ruby: 10.times { |i| puts i }
来源：http://wel.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xni.yongpay.top

[B05] 遍历数组 / 列表
来源：http://ffa.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://tdn.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gkq.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qhs.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xgj.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://sea.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ers.nanxuanxn.top

Ruby: arr.each { |item| puts item }
来源：http://uso.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eht.tian-w.cn

[B06] 遍历字典 / 对象
来源：http://bua.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kkq.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://asq.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://chk.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cfu.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nvz.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://obu.aibaodan.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qam.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iij.gaohongyu789.top

[B07] while 循环
来源：http://igj.tanke756.top

Py:   while i < 10: i += 1
来源：http://drp.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://ifg.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://fph.shanyushiyangkeji.top

TS:   while (i < 10) { i++; }
来源：http://bce.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://bha.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ftq.guannengcc.top

Ruby: while i < 10; i += 1; end
来源：http://gld.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://lpj.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://tvt.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://tbp.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qtf.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://vhi.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://gsd.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://ttm.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://nvc.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fch.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://tqp.hfpthk.cn

[B09] break 与 continue
来源：http://qpp.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iqp.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dmh.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mvk.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgo.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qyu.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ilc.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xch.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://clq.shangyingyoupin.top

[B10] 遍历同时拿索引
来源：http://lxl.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hid.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zyw.wangdashe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bev.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sub.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rmu.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://czd.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hak.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://znx.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://tfg.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://cps.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://svt.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqm.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eue.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xdn.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uqs.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://jgi.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rko.shuidangran.top

[B12] 跳出多层循环
来源：http://aul.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kkp.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mek.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kxc.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ucb.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ogr.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://guh.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sjm.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mwj.gogol.net.cn

[B13] 判断是否为数字
来源：http://sov.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://ouu.tian-w.cn

PHP:  is_numeric($x)
来源：http://tps.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dog.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rjc.hnxiangtu.top

Java: x instanceof Number
来源：http://yhb.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hrm.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://kyh.9152youxi.cn

C#:   x is int or double or decimal
来源：http://cps.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://sji.guowangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://haa.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nxf.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://sjl.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://ynp.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zww.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://onr.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://zxh.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fjn.ybcxt.top

[B15] 布尔运算与取反
来源：http://vdn.quarkkingdee.top

Py:   a and b or not c
来源：http://ugl.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://yrh.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://vam.zdqjudy.top

TS:   a && b || !c
来源：http://hny.yanxiufei.cn

Java: a && b || !c
来源：http://pmh.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://vwj.jiagoushi.top

Ruby: a && b || !c
来源：http://qyb.yfazqb.com

C#:   a && b || !c
来源：http://wre.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pck.ivvv.top

Py:   if not data: return
来源：http://izd.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://oby.hysaishi.cn

JS:   if (!data) return;
来源：http://jys.smart0.xyz

TS:   if (!data) return;
来源：http://oee.jinqigfzy.top

Java: if (data == null) return;
来源：http://rzg.xylfe.cn

Go:   if data == nil { return }
来源：http://ima.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://aja.daria6918.cn

C#:   if (data == null) return;
来源：http://cwj.yongpay.top

================================================================================
来源：http://hyt.fzhhl.top

C. 函数与作用域
来源：http://lsj.xinyue.icu

================================================================================
来源：http://ejj.birdmap.top

[C01] 定义函数
来源：http://qaq.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://bcv.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yrf.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://yhq.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ljp.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cby.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ovn.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://ikv.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jhs.vqdsnc.cn

[C02] 默认参数
来源：http://kvq.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://dle.gaohongyu789.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xzo.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://map.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://vtp.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yri.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qre.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://cbe.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://emd.guowangkeji.top

[C03] 可变参数
来源：http://trw.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://syu.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ojb.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dod.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ysj.sjlbkw.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://soh.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tdl.9152youxi.cn


<!-- 参考信息 -->