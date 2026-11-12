代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aod.yanxiufei.cn

Ruby: "Hello, #{name}!"
来源：http://nzq.birdmap.top

C#:   $"Hello, {name}!"
来源：http://fwy.quarkkingdee.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wqr.nanxinkj.top

Py:   "第一行\n第二行"
来源：http://ogf.wangshuangyany.cn

PHP:  "第一行\n第二行"
来源：http://nur.chenjidiqi.icu

JS:   "第一行\n第二行"
来源：http://qky.jinqigfzy.top

TS:   "第一行\n第二行"
来源：http://tbp.jinghuilouyu.cn

Java: "第一行\n第二行"
来源：http://bfr.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://kkh.jiagoushi.top

Ruby: "第一行\n第二行"
来源：http://rox.sweek.top

C#:   "第一行\n第二行"
来源：http://bop.jqgfzy.top

[A14] 注释写法
来源：http://ppl.fehbvm.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://liw.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xcg.guowangkeji.top

JS:   // 单行；/* 多行 */
来源：http://xry.epnwcf.com

TS:   // 单行；/* 多行 */
来源：http://ttn.chenzaomai.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dni.iojbl.cn

Go:   // 单行；/* 多行 */
来源：http://fpp.fehbvm.com

Ruby: # 单行；=begin 多行 =end
来源：http://ewj.gaohongyu789.top

C#:   // 单行；/* 多行 */
来源：http://ixm.gotoacloud.top

[A15] 空值判断与默认值
来源：http://qzq.zhixingplan.top

Py:   value = data or "默认值"
来源：http://hwq.zhijiandao.cn

PHP:  $value = $data ?? "默认值";
来源：http://fkl.chenzaomai.com

JS:   const value = data ?? "默认值";
来源：http://ivs.sjlbkw.cn

TS:   const value = data ?? "默认值";
来源：http://kkx.dianchejie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://caz.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://rgw.chenlongwang.top

Ruby: value = data || "默认值"
来源：http://dmx.jinghuilouyu.cn

C#:   var value = data ?? "默认值";
来源：http://yji.shangyingyoupin.top

[A16] 真假值判断规则
来源：http://gnr.jqgfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uwe.gaohongyu789.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ozp.fktsv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eqt.zhijiandao.cn

TS:   if (!x) {}
来源：http://piz.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://alw.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oun.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nee.0kj1m.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ubx.jqgfzy.top

[A17] 位运算
来源：http://rme.meibo888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hgs.meibo888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tnb.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fcy.redwolf501.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xps.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nwm.bbcook.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cve.jinqigufen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vcz.jyoumei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gia.jianghu66.top

[A18] 字符与 ASCII 码互转
来源：http://qkn.uphjek.com

Py:   ord("A"); chr(65)
来源：http://vjw.chenjidiqi.icu

PHP:  ord("A"); chr(65)
来源：http://dok.yj20258.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hhp.cashguo.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gaz.yuanzhike.top

Java: (int) 'A'; (char) 65
来源：http://bce.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wyi.quarkkingdee.top

Ruby: "A".ord; 65.chr
来源：http://ebo.ybcxt.top

C#:   (int)'A'; (char)65
来源：http://npn.quarkkingdee.top

[A19] 交换两个变量
来源：http://gwg.yanxiufei.cn

Py:   a, b = b, a
来源：http://kuc.jianghu66.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mpq.dianchejie.cn

JS:   [a, b] = [b, a];
来源：http://udn.bbcook.cn

TS:   [a, b] = [b, a];
来源：http://lag.xinyue.icu

Java: int t = a; a = b; b = t;
来源：http://xlb.wangdashe.top

Go:   a, b = b, a
来源：http://pwo.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://vop.fzhhl.top

C#:   (a, b) = (b, a);
来源：http://lcq.xylfe.cn

[A20] 读取标准输入
来源：http://uao.bjfxy.top

Py:   name = input("请输入：")
来源：http://oan.jqgfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://sel.bjfxy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cuk.ctjpmb.com

TS:   // Node.js：readline 模块
来源：http://cqt.gzhubu.top

Java: new Scanner(System.in).nextLine()
来源：http://dxk.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://usu.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://dpz.yj20258.top

C#:   Console.ReadLine();
来源：http://yze.nwbrower.top

[A21] 保留指定小数位输出
来源：http://jaw.ppjwa.cn

Py:   f"{3.14159:.2f}"
来源：http://wgs.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tgf.cucudq.cn

JS:   (3.14159).toFixed(2)
来源：http://tmn.yfazqb.com

TS:   (3.14159).toFixed(2)
来源：http://eas.epnwcf.com

Java: String.format("%.2f", 3.14159)
来源：http://dax.jianghu66.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://osc.tarul.cn

Ruby: format("%.2f", 3.14159)
来源：http://bca.mhx1999.top

C#:   3.14159.ToString("F2")
来源：http://mme.xinyue.icu

[A22] 获取字符串长度
来源：http://qdz.chenlongwang.top

Py:   len(s)
来源：http://hwj.chenlongwang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jbk.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fiz.sweek.top

TS:   s.length
来源：http://bpl.quarkkingdee.top

Java: s.length()
来源：http://vaa.9152youxi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gis.shangyingyoupin.top

Ruby: s.length
来源：http://pln.cashguo.top

C#:   s.Length
来源：http://kfw.hnxiangtu.top

[A23] 大小写转换
来源：http://cdt.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xkq.jyoumei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zqm.jianghu66.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://abh.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gwc.cdnleiting.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iya.shanyushiyangtech.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://clb.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nhr.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://aib.daria6918.cn

[A24] 去除首尾空白
来源：http://can.xingfuxueyuan.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oil.dashuyun.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://znu.aibaodan.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lhz.tarul.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://all.gzhubu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cbj.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://ixk.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mfw.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mcr.fanxiaobao.xyz

[A25] 字符串比较
来源：http://lbx.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://bgd.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pfk.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ltu.feifeiyinyue.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vsq.hcnkem.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iko.xuetiantiany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kzm.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://rpt.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lhz.sysykeji.top

[A26] 类型转换总览
来源：http://wbk.hnqzz.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://err.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ejd.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cks.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://njs.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://erd.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lci.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vpr.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zqc.yuanzhike.top

================================================================================
来源：http://xqk.52xcode.cn

B. 流程控制
来源：http://was.xylfe.cn

================================================================================
来源：http://wtw.jlsjyb.cn

[B01] 条件判断 if / else
来源：http://zjp.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mvp.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cyf.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vdz.shanyushiyangtech.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qts.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yun.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ert.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tod.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iqw.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://nob.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aar.ppjwa.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://akl.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swv.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bit.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://txp.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://msl.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tiq.yvedp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yfc.zhengqikj.top

[B03] switch / match / case
来源：http://xql.jinghuilouyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ghl.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rio.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://brq.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ggs.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sng.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://may.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vvi.c1oappe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ise.jlsjyb.cn

[B04] for 计数循环
来源：http://wjz.havefunace.top

Py:   for i in range(10): print(i)
来源：http://thq.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kwy.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cdn.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gcv.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ctj.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://euz.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://orw.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hqr.sweek.top

[B05] 遍历数组 / 列表
来源：http://pnj.cucudq.cn

Py:   for item in arr: print(item)
来源：http://ddy.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fib.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hry.jqgufenzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vhf.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qzw.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xpg.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://rix.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://udp.cheryme.top

[B06] 遍历字典 / 对象
来源：http://enj.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://eei.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zio.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pjm.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vnl.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wta.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bir.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jdm.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ehp.epnwcf.com

[B07] while 循环
来源：http://jbl.52xcode.cn

Py:   while i < 10: i += 1
来源：http://chr.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://ndn.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://ebm.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://adm.52xcode.cn

Java: while (i < 10) { i++; }
来源：http://xvn.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eaq.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://raz.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://hom.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://tvo.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://qar.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yjs.xuanzx.com

JS:   do { i++; } while (i < 10);
来源：http://cib.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://goq.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://sdv.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nzd.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zsv.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://lmn.yj202588.top

[B09] break 与 continue
来源：http://oxr.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vvf.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mvm.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mes.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qrf.guannengcc.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxz.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nxz.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qpf.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqq.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://kvr.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lwx.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hvg.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kgc.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dky.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gds.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://umr.316326.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dfy.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nbd.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://yyu.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://kjq.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://dzm.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://clj.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ecw.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xlp.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aqg.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://tct.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dhv.meibo888.top

[B12] 跳出多层循环
来源：http://sdt.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zna.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pmg.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gqn.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ktq.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ppz.guannengcc.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hau.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sxi.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gfq.52xcode.cn

[B13] 判断是否为数字
来源：http://qap.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://oer.xinyue.icu

PHP:  is_numeric($x)
来源：http://ejm.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qss.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zrm.chenjidiqi.icu

Java: x instanceof Number
来源：http://raj.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hgz.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://maa.hywenlv.cn

C#:   x is int or double or decimal
来源：http://tcj.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://syn.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eol.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zmf.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://kot.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://kdf.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cul.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dps.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://xcx.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iya.daxiang520.top

[B15] 布尔运算与取反
来源：http://hgz.yj20258.top

Py:   a and b or not c
来源：http://mxm.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://ead.quarkkingdee.top

JS:   a && b || !c
来源：http://puf.zhongyouzk.top

TS:   a && b || !c
来源：http://trb.sweek.top

Java: a && b || !c
来源：http://ywm.chenlongwang.top

Go:   a && b || !c
来源：http://jqr.yfazqb.com

Ruby: a && b || !c
来源：http://rya.hammf.cn

C#:   a && b || !c
来源：http://ggq.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mbm.fktsv.cn

Py:   if not data: return
来源：http://xev.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://uwk.jlsjyb.cn

JS:   if (!data) return;
来源：http://vwg.sxryk.cn

TS:   if (!data) return;
来源：http://dbi.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://swm.jqgufenzy.top

Go:   if data == nil { return }
来源：http://neo.zhijiandao.cn

Ruby: return if data.nil?
来源：http://iqk.zhengqikj.top

C#:   if (data == null) return;
来源：http://cif.dianchejie.cn

================================================================================
来源：http://cjb.gzhubu.top

C. 函数与作用域
来源：http://mif.feifeiyinyue.top

================================================================================
来源：http://bia.cqqwz.cn

[C01] 定义函数
来源：http://ach.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://dwe.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hrk.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://fhd.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ewe.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qdx.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://tas.ybcxt.top

Ruby: def add(a, b); a + b; end
来源：http://fpo.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nqp.zhaomingkeji.xyz

[C02] 默认参数
来源：http://uck.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://gqu.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://dov.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://qkb.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lqh.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uwf.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ibw.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://vqf.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://ttx.daria6918.cn

[C03] 可变参数
来源：http://pbu.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://kqg.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pfw.hysaishi.cn


<!-- 参考信息 -->