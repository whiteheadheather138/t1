代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vhf.jlsjyb.cn

JS:   `Hello, ${name}!`
来源：http://vzo.epnwcf.com

TS:   `Hello, ${name}!`
来源：http://czs.ctjpmb.com

Java: "Hello, %s!".formatted(name)
来源：http://ltf.yvedp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dmk.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://hrx.uphjek.com

C#:   $"Hello, {name}!"
来源：http://sho.bbcook.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cqv.daxiang520.top

Py:   "第一行\n第二行"
来源：http://zsu.nwbrower.top

PHP:  "第一行\n第二行"
来源：http://bje.cucudq.cn

JS:   "第一行\n第二行"
来源：http://cph.hnqzz.top

TS:   "第一行\n第二行"
来源：http://hxp.dianchejie.cn

Java: "第一行\n第二行"
来源：http://vwp.epnwcf.com

Go:   "第一行\n第二行"
来源：http://ugy.316326.xyz

Ruby: "第一行\n第二行"
来源：http://oti.dashuyun.cn

C#:   "第一行\n第二行"
来源：http://epv.vqdsnc.cn

[A14] 注释写法
来源：http://ldx.zycfv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rzd.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jum.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://lqg.havefunace.top

TS:   // 单行；/* 多行 */
来源：http://evp.fehbvm.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://txn.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://pof.epnwcf.com

Ruby: # 单行；=begin 多行 =end
来源：http://eqy.xinyue.icu

C#:   // 单行；/* 多行 */
来源：http://nyw.yongpay.top

[A15] 空值判断与默认值
来源：http://crs.hfpthk.cn

Py:   value = data or "默认值"
来源：http://dll.zhixingplan.top

PHP:  $value = $data ?? "默认值";
来源：http://fdu.dashuyun.cn

JS:   const value = data ?? "默认值";
来源：http://fah.feifeiyinyue.top

TS:   const value = data ?? "默认值";
来源：http://cfp.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eok.bbcook.cn

Go:   if data == "" { data = "默认值" }
来源：http://elk.hysaishi.cn

Ruby: value = data || "默认值"
来源：http://zyj.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://dxz.zhongyouzk.top

[A16] 真假值判断规则
来源：http://ktk.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ljx.gogol.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pet.gogol.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rgx.yj20258.top

TS:   if (!x) {}
来源：http://uas.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pjt.hnqzz.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aef.fzhhl.top

Ruby: unless x            # nil 与 false 为假
来源：http://lba.sweek.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tbl.jyoumei.cn

[A17] 位运算
来源：http://rxf.dianchejie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zpt.zhijiandao.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fkw.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kay.shanyushiyangtech.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qto.dashuyun.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dsn.wangdashe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eyh.zdqjudy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pem.9152youxi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xor.zhiwuduotai.top

[A18] 字符与 ASCII 码互转
来源：http://gff.jiagoushi.top

Py:   ord("A"); chr(65)
来源：http://ozp.cashguo.top

PHP:  ord("A"); chr(65)
来源：http://kqk.tanke756.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lsh.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fqq.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://jbd.cucudq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://auw.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://dbm.sjlbkw.cn

C#:   (int)'A'; (char)65
来源：http://pmq.sufxvd.cn

[A19] 交换两个变量
来源：http://uxp.daxiang520.top

Py:   a, b = b, a
来源：http://adx.yvedp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dfm.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://hyr.epnwcf.com

TS:   [a, b] = [b, a];
来源：http://aly.chenjidiqi.icu

Java: int t = a; a = b; b = t;
来源：http://juf.gaohongyu789.top

Go:   a, b = b, a
来源：http://twx.guannengcc.top

Ruby: a, b = b, a
来源：http://ztk.zdqjudy.top

C#:   (a, b) = (b, a);
来源：http://lqm.jqgfzy.top

[A20] 读取标准输入
来源：http://lhf.yj202588.top

Py:   name = input("请输入：")
来源：http://sax.jinqigufen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hpn.redwolf501.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dfr.fzhhl.top

TS:   // Node.js：readline 模块
来源：http://rpc.kuanghao11.cn

Java: new Scanner(System.in).nextLine()
来源：http://eyd.ppjwa.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kxq.xinyue.icu

Ruby: gets.chomp
来源：http://nlo.zhengqikj.top

C#:   Console.ReadLine();
来源：http://rrt.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://kve.guannengcc.top

Py:   f"{3.14159:.2f}"
来源：http://dds.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cgc.yj20258.top

JS:   (3.14159).toFixed(2)
来源：http://vbg.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://aqq.gzhubu.top

Java: String.format("%.2f", 3.14159)
来源：http://gyh.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rbt.yongpay.top

Ruby: format("%.2f", 3.14159)
来源：http://sqi.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://ccw.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://ory.xinyue.icu

Py:   len(s)
来源：http://aki.jinghuilouyu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://waw.hywenlv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eja.nanxuanxn.top

TS:   s.length
来源：http://inn.yongpay.top

Java: s.length()
来源：http://kua.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wkh.dianchejie.cn

Ruby: s.length
来源：http://key.hongshengwenyu.top

C#:   s.Length
来源：http://vwl.ydzc1.top

[A23] 大小写转换
来源：http://fka.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://rhb.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mat.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bla.sysykeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rpl.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wyw.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://icb.nanxinkj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fox.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gxk.daxiang520.top

[A24] 去除首尾空白
来源：http://gvk.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aux.chenlongwang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nxz.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fud.feifeiyinyue.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://loq.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ark.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://xgn.dashuyun.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qls.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ibu.bbcook.cn

[A25] 字符串比较
来源：http://zkb.zdqjudy.top

Py:   s1 == s2; s1 != s2
来源：http://csv.pycfn.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xjo.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rmq.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nri.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://liv.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yih.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ipv.xuanzx.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://plq.jinyuanbaomall.cn

[A26] 类型转换总览
来源：http://ulf.guowangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nqr.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jya.guowangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wnr.wangdashe.top

TS:   Number() String() Boolean() x as number
来源：http://vbg.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://usq.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rqa.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cgq.tian-w.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vfr.hongshengwenyu.top

================================================================================
来源：http://dbs.zhoulong.xyz

B. 流程控制
来源：http://rkj.redwolf501.top

================================================================================
来源：http://yoo.yonumen.top

[B01] 条件判断 if / else
来源：http://kcq.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bqq.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qfa.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bgv.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oop.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jqh.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nuj.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ejf.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://slt.0kj1m.cn

[B02] 多分支 else if / elif
来源：http://ayl.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tiu.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ecp.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kre.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eft.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rzz.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wmu.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rdm.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqa.pengpengdd.cyou

[B03] switch / match / case
来源：http://bmt.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jxs.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://emk.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://txn.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jil.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qpo.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tfn.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hrt.52xcode.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rmk.bbcook.cn

[B04] for 计数循环
来源：http://pee.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://ona.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://thm.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ckh.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rxz.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ujg.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dzf.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://npj.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ula.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://yoa.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://pgh.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zsy.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kii.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kdp.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ylh.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mhi.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://mbt.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://trf.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://zud.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gkf.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bcf.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lzm.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xsi.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cvq.sxryk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rtt.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xbz.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ykj.xylfe.cn

[B07] while 循环
来源：http://lnw.daxiang520.top

Py:   while i < 10: i += 1
来源：http://qbe.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://bpe.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://mvn.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://nin.pycfn.com

Java: while (i < 10) { i++; }
来源：http://glp.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hpt.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://tck.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://ndn.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://deh.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://kmi.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ekb.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://xwn.nanxuanxn.top

TS:   do { i++; } while (i < 10);
来源：http://oil.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://ker.sufxvd.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fvb.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://day.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://cnf.nanxinkj.top

[B09] break 与 continue
来源：http://bla.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://biy.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zvq.hywenlv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qlt.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bbu.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wzh.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ssw.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ypc.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chb.gzhubu.top

[B10] 遍历同时拿索引
来源：http://rde.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fnf.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://acx.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sav.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://poz.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bcn.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qhq.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xsu.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zce.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://elg.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://gra.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://vls.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qbs.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jiq.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aqi.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ssi.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://fbi.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://njf.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://jkv.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://xcp.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hsv.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ugf.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zrz.fengsongda.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lnq.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qui.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yns.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tsi.hnqzz.top

[B13] 判断是否为数字
来源：http://zyu.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://rkx.cheryme.top

PHP:  is_numeric($x)
来源：http://wqh.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ubk.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gte.zhixingplan.top

Java: x instanceof Number
来源：http://cjj.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://buq.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://gzp.fktsv.cn

C#:   x is int or double or decimal
来源：http://gtk.jianghu66.top

[B14] 判断值是否在集合内
来源：http://kos.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nvn.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dgm.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://apk.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://bwl.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ysk.hnxiangtu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uhs.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://wxb.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jkq.yuxming.cn

[B15] 布尔运算与取反
来源：http://uwo.fktsv.cn

Py:   a and b or not c
来源：http://div.birdmap.top

PHP:  $a && $b || !$c
来源：http://qwc.sxryk.cn

JS:   a && b || !c
来源：http://mxg.sweek.top

TS:   a && b || !c
来源：http://xbi.yuanzhike.top

Java: a && b || !c
来源：http://sxi.tanke756.top

Go:   a && b || !c
来源：http://udx.andypj.xyz

Ruby: a && b || !c
来源：http://tbd.chenlongwang.top

C#:   a && b || !c
来源：http://bzo.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://wwm.yanxiufei.cn

Py:   if not data: return
来源：http://oxy.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://chs.fengsongda.top

JS:   if (!data) return;
来源：http://clg.aizwys.cn

TS:   if (!data) return;
来源：http://lxh.hesvh.cn

Java: if (data == null) return;
来源：http://quc.fehbvm.com

Go:   if data == nil { return }
来源：http://vcc.guowangkeji.top

Ruby: return if data.nil?
来源：http://wyx.vehdjk.com

C#:   if (data == null) return;
来源：http://gpi.yonumen.top

================================================================================
来源：http://qnv.xingfuxueyuan.xyz

C. 函数与作用域
来源：http://ixr.uphjek.com

================================================================================
来源：http://sgj.zhengqikj.top

[C01] 定义函数
来源：http://hgw.uphjek.com

Py:   def add(a, b): return a + b
来源：http://mbz.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oay.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://axr.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iyl.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tgu.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://web.ybcxt.top

Ruby: def add(a, b); a + b; end
来源：http://wzu.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fsg.mhx1999.top

[C02] 默认参数
来源：http://hyh.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://vjf.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://guy.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://gre.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pnk.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://gcg.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aef.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://hda.feifeiyinyue.top


<!-- 参考信息 -->