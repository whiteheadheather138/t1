代发 wailian999

Py:   "第一行\n第二行"
来源：http://uyq.chenjidiqi.icu

PHP:  "第一行\n第二行"
来源：http://qkn.cucudq.cn

JS:   "第一行\n第二行"
来源：http://sqb.tarul.cn

TS:   "第一行\n第二行"
来源：http://thu.cucudq.cn

Java: "第一行\n第二行"
来源：http://xpx.jinghuilouyu.cn

Go:   "第一行\n第二行"
来源：http://ndo.cqqwz.cn

Ruby: "第一行\n第二行"
来源：http://pqu.yuanzhike.top

C#:   "第一行\n第二行"
来源：http://qzt.shuidangran.top

[A14] 注释写法
来源：http://loz.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://twe.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cdh.feifeiyinyue.top

JS:   // 单行；/* 多行 */
来源：http://yfj.zhaomingkeji.xyz

TS:   // 单行；/* 多行 */
来源：http://lwa.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hyk.hongshengwenyu.top

Go:   // 单行；/* 多行 */
来源：http://qwu.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://fle.nwbrower.top

C#:   // 单行；/* 多行 */
来源：http://mma.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://wqp.fktsv.cn

Py:   value = data or "默认值"
来源：http://dyq.shuidangran.top

PHP:  $value = $data ?? "默认值";
来源：http://xfe.hcnkem.com

JS:   const value = data ?? "默认值";
来源：http://bed.feifeiyinyue.top

TS:   const value = data ?? "默认值";
来源：http://voz.dashuyun.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uhr.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://uig.yuxming.cn

Ruby: value = data || "默认值"
来源：http://aec.jqgfzy.top

C#:   var value = data ?? "默认值";
来源：http://mys.fengsongda.top

[A16] 真假值判断规则
来源：http://anp.yuanzhike.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://knq.hesvh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://svc.smart0.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xrl.yonumen.top

TS:   if (!x) {}
来源：http://puy.bbcook.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nvu.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fxn.xuanzx.com

Ruby: unless x            # nil 与 false 为假
来源：http://qpb.ydzc1.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lfr.zhongyouzk.top

[A17] 位运算
来源：http://fgj.smart0.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xic.316326.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ksu.shzxlz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ebj.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qqo.hfpthk.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dyr.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ooc.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wrw.9152youxi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pbt.cucudq.cn

[A18] 字符与 ASCII 码互转
来源：http://rom.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://ysa.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://fkg.kuanghao11.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rnh.ywan-chungtsiang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ujz.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://omb.ywan-chungtsiang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cih.shzxlz.cn

Ruby: "A".ord; 65.chr
来源：http://khq.zhiwuduotai.top

C#:   (int)'A'; (char)65
来源：http://wcj.nanxinkj.top

[A19] 交换两个变量
来源：http://qlm.c1oappe.top

Py:   a, b = b, a
来源：http://zxe.zhengqikj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://izz.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://zpi.52xcode.cn

TS:   [a, b] = [b, a];
来源：http://wrr.tianlin.xyz

Java: int t = a; a = b; b = t;
来源：http://sai.yj20258.top

Go:   a, b = b, a
来源：http://bje.fzhhl.top

Ruby: a, b = b, a
来源：http://wbu.zhijiandao.cn

C#:   (a, b) = (b, a);
来源：http://ala.fehbvm.com

[A20] 读取标准输入
来源：http://hpq.jqgfzy.top

Py:   name = input("请输入：")
来源：http://dit.hammf.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kul.zhongyouzk.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vxw.bbcook.cn

TS:   // Node.js：readline 模块
来源：http://lej.tanke756.top

Java: new Scanner(System.in).nextLine()
来源：http://vei.birdmap.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qud.zhijiandao.cn

Ruby: gets.chomp
来源：http://oaz.cheryme.top

C#:   Console.ReadLine();
来源：http://oor.cdnleiting.top

[A21] 保留指定小数位输出
来源：http://ety.jlsjyb.cn

Py:   f"{3.14159:.2f}"
来源：http://qqa.andypj.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ttv.vehdjk.com

JS:   (3.14159).toFixed(2)
来源：http://ctw.hesvh.cn

TS:   (3.14159).toFixed(2)
来源：http://swx.bjfxy.top

Java: String.format("%.2f", 3.14159)
来源：http://pbd.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gqr.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://fff.gaohongyu789.top

C#:   3.14159.ToString("F2")
来源：http://sph.guowangkeji.top

[A22] 获取字符串长度
来源：http://vcr.xylfe.cn

Py:   len(s)
来源：http://zzj.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lzb.hammf.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://obg.gaohongyu789.top

TS:   s.length
来源：http://vpt.xuanzx.com

Java: s.length()
来源：http://xhz.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qnv.chenjidiqi.icu

Ruby: s.length
来源：http://ptg.xuanzx.com

C#:   s.Length
来源：http://iem.yj202588.top

[A23] 大小写转换
来源：http://vgg.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nnm.bbcook.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://puh.andypj.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qne.zhongyouzk.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sfd.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ozw.daxiang520.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xmr.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yhd.feifeiyinyue.top

C#:   s.ToUpper(); s.ToLower()
来源：http://miz.52xcode.cn

[A24] 去除首尾空白
来源：http://udw.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mnq.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hks.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vqw.pengpengdd.cyou

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cpj.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ftw.tanke756.top

Go:   strings.TrimSpace(s)
来源：http://fsm.bjfxy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dpx.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ruo.tianlin.xyz

[A25] 字符串比较
来源：http://lfe.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://yut.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zet.fktsv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wnb.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://byi.xylfe.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nuq.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mvn.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nod.jinyuanbaomall.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wrr.xziqi.cn

[A26] 类型转换总览
来源：http://ptk.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bfl.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vqz.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ybg.0kj1m.cn

TS:   Number() String() Boolean() x as number
来源：http://ibs.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://drk.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ton.dashuyun.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://thg.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wej.tian-w.cn

================================================================================
来源：http://hvc.ydzc1.top

B. 流程控制
来源：http://dln.zhoulong.xyz

================================================================================
来源：http://tqy.gzhubu.top

[B01] 条件判断 if / else
来源：http://yjc.zhixingplan.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bsh.xylfe.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://svb.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tdb.hcnkem.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gfr.zhaomingkeji.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://utl.pengpengdd.cyou

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wex.sufxvd.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://laz.haohaochexian.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rkv.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://lqq.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ooo.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ncv.cashguo.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tew.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://skg.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bid.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xrn.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vbv.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wmp.jqgfzy.top

[B03] switch / match / case
来源：http://xvz.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xzz.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fws.chenlongwang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oca.yj20258888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xxz.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dmd.yonumen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bjg.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://shn.yj20258888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dhr.yfazqb.com

[B04] for 计数循环
来源：http://ipg.ivvv.top

Py:   for i in range(10): print(i)
来源：http://xav.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mdp.wangdashe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hjx.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lqh.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bme.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gxb.yj20258888.top

Ruby: 10.times { |i| puts i }
来源：http://yuf.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yug.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://auu.daxiang520.top

Py:   for item in arr: print(item)
来源：http://uar.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fxg.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sqe.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://oyh.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://lbw.pengpengdd.cyou

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vsg.smart0.xyz

Ruby: arr.each { |item| puts item }
来源：http://hfu.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://okr.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://hvd.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ovt.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kcn.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ftn.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jjg.zhiwuduotai.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yle.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vkw.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://myv.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://boi.hcnkem.com

[B07] while 循环
来源：http://qhp.daria6918.cn

Py:   while i < 10: i += 1
来源：http://ypz.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oqu.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://knw.cqqwz.cn

TS:   while (i < 10) { i++; }
来源：http://lvf.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://vhb.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hmb.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://sky.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://plt.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://xwy.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://wyp.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://mtm.jiagoushi.top

JS:   do { i++; } while (i < 10);
来源：http://xwo.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://ktm.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://osb.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cbc.bbcook.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pfa.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://gmu.sysykeji.top

[B09] break 与 continue
来源：http://wgp.dianchejie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rri.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gub.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dab.snrcjt.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jzg.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddo.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sgw.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uwu.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zkf.yj20258.top

[B10] 遍历同时拿索引
来源：http://son.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rek.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gkc.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zjy.xuanzx.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zoz.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qka.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ibw.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://arm.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pnz.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://yuk.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://qfr.xuetiantiany.cn

PHP:  range(0, 10, 2);
来源：http://ybc.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jsw.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nrg.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pbv.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ies.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://dvi.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jvy.jlsjyb.cn

[B12] 跳出多层循环
来源：http://ozb.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yyr.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qrs.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zoh.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tgz.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eov.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://slh.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vkt.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tro.hnxiangtu.top

[B13] 判断是否为数字
来源：http://ods.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://ako.hesvh.cn

PHP:  is_numeric($x)
来源：http://npk.jqgfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xgj.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zky.yonumen.top

Java: x instanceof Number
来源：http://vcj.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eqm.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://qvv.jianghu66.top

C#:   x is int or double or decimal
来源：http://wct.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://zgf.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://euv.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ria.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://cqz.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://eqi.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jqd.zhixingplan.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kkd.jianghu66.top

Ruby: [1, 2, 3].include?(x)
来源：http://gmg.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://clo.gogol.net.cn

[B15] 布尔运算与取反
来源：http://xko.yj20258888.top

Py:   a and b or not c
来源：http://dze.daria6918.cn

PHP:  $a && $b || !$c
来源：http://wyw.yongpay.top

JS:   a && b || !c
来源：http://gtb.pengpengdd.cyou

TS:   a && b || !c
来源：http://yhu.mhx1999.top

Java: a && b || !c
来源：http://sbo.cucudq.cn

Go:   a && b || !c
来源：http://hym.haohaochexian.top

Ruby: a && b || !c
来源：http://wjr.yuanzhike.top

C#:   a && b || !c
来源：http://szw.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://nhj.ybcxt.top

Py:   if not data: return
来源：http://biv.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://hah.sxryk.cn

JS:   if (!data) return;
来源：http://cvv.zhengqikj.top

TS:   if (!data) return;
来源：http://irt.shzxlz.cn

Java: if (data == null) return;
来源：http://mwh.sxryk.cn

Go:   if data == nil { return }
来源：http://frq.sjlbkw.cn

Ruby: return if data.nil?
来源：http://hwn.vqdsnc.cn

C#:   if (data == null) return;
来源：http://dmc.feifeiyinyue.top

================================================================================
来源：http://aub.yj202588.top

C. 函数与作用域
来源：http://wqt.gaohongyu789.top

================================================================================
来源：http://ovn.birdmap.top

[C01] 定义函数
来源：http://nax.yj202588.top

Py:   def add(a, b): return a + b
来源：http://ewb.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bsr.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://qtt.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ybo.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://epw.tianlin.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vrg.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://xud.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://csz.tian-w.cn

[C02] 默认参数
来源：http://xxk.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://hbt.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://xsu.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://sxf.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://usz.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uju.xylfe.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xyn.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://zjx.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://zli.sweek.top

[C03] 可变参数
来源：http://epc.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://ryn.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dfl.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xnr.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zcp.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qyy.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ohj.aizwys.cn


<!-- 参考信息 -->