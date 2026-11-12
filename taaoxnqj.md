代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ycg.0kj1m.cn

Ruby: "Hello, #{name}!"
来源：http://wty.jyoumei.cn

C#:   $"Hello, {name}!"
来源：http://ovh.ppjwa.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hvg.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://fqs.guannengcc.top

PHP:  "第一行\n第二行"
来源：http://usu.gaohongyu789.top

JS:   "第一行\n第二行"
来源：http://vov.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://mti.hongshengwenyu.top

Java: "第一行\n第二行"
来源：http://dwc.haohaochexian.top

Go:   "第一行\n第二行"
来源：http://ipv.aizwys.cn

Ruby: "第一行\n第二行"
来源：http://mgk.redwolf501.top

C#:   "第一行\n第二行"
来源：http://tgg.jqgufenzy.top

[A14] 注释写法
来源：http://csc.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://bce.ydjk.org.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dzd.cdnleiting.top

JS:   // 单行；/* 多行 */
来源：http://ira.shanyushiyangkeji.top

TS:   // 单行；/* 多行 */
来源：http://bwt.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mos.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://yih.guannengcc.top

Ruby: # 单行；=begin 多行 =end
来源：http://aoo.fengsongda.top

C#:   // 单行；/* 多行 */
来源：http://ovc.yj20258888.top

[A15] 空值判断与默认值
来源：http://cpe.andypj.xyz

Py:   value = data or "默认值"
来源：http://xwt.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://djw.gogol.net.cn

JS:   const value = data ?? "默认值";
来源：http://gxj.hfpthk.cn

TS:   const value = data ?? "默认值";
来源：http://lcj.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qfp.ywan-chungtsiang.top

Go:   if data == "" { data = "默认值" }
来源：http://wgg.xingfuxueyuan.xyz

Ruby: value = data || "默认值"
来源：http://tlo.wangshuangyany.cn

C#:   var value = data ?? "默认值";
来源：http://caj.hnxiangtu.top

[A16] 真假值判断规则
来源：http://yob.mhx1999.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nkp.fktsv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wea.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://son.zycfv.cn

TS:   if (!x) {}
来源：http://pri.zhoulong.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rgp.zhaomingkeji.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://puv.smart0.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://qnm.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pes.cdnleiting.top

[A17] 位运算
来源：http://mix.birdmap.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mcm.yj20258888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wtr.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xvx.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wuj.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nsz.sxryk.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ncr.tarul.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wzx.zhiwuduotai.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://llf.gzhubu.top

[A18] 字符与 ASCII 码互转
来源：http://iob.chenjidiqi.icu

Py:   ord("A"); chr(65)
来源：http://vwo.sjlbkw.cn

PHP:  ord("A"); chr(65)
来源：http://mzd.52xcode.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cbb.andypj.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://onl.fzhhl.top

Java: (int) 'A'; (char) 65
来源：http://yrl.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tyv.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://rho.xuetiantiany.cn

C#:   (int)'A'; (char)65
来源：http://xcs.ehwqpu.com

[A19] 交换两个变量
来源：http://mea.wangdashe.top

Py:   a, b = b, a
来源：http://hhv.zdqjudy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bke.hnxiangtu.top

JS:   [a, b] = [b, a];
来源：http://tok.ivvv.top

TS:   [a, b] = [b, a];
来源：http://mbk.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://bsa.aibaodan.cn

Go:   a, b = b, a
来源：http://alw.yongpay.top

Ruby: a, b = b, a
来源：http://kdv.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://lyj.jinyuanbaomall.cn

[A20] 读取标准输入
来源：http://gxf.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://mxd.aizwys.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fop.aibaodan.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lzn.yvedp.cn

TS:   // Node.js：readline 模块
来源：http://qeq.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://pbz.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sbz.quarkkingdee.top

Ruby: gets.chomp
来源：http://yaj.ydzc1.top

C#:   Console.ReadLine();
来源：http://uzz.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://efj.yangfankeji.com

Py:   f"{3.14159:.2f}"
来源：http://xxt.tanke756.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kvs.chenlongwang.top

JS:   (3.14159).toFixed(2)
来源：http://abr.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://ybm.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://vto.tian-w.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://axq.jqgufenzy.top

Ruby: format("%.2f", 3.14159)
来源：http://opt.dianchejie.cn

C#:   3.14159.ToString("F2")
来源：http://glh.hnqzz.top

[A22] 获取字符串长度
来源：http://myp.tian-w.cn

Py:   len(s)
来源：http://jfv.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dpu.bjfxy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://afp.svipenyu.cn

TS:   s.length
来源：http://bxb.sxryk.cn

Java: s.length()
来源：http://vyn.cashguo.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wei.feifeiyinyue.top

Ruby: s.length
来源：http://qmk.hnxiangtu.top

C#:   s.Length
来源：http://lsp.zdqjudy.top

[A23] 大小写转换
来源：http://jdn.0kj1m.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://byk.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dpz.fktsv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rbt.52xcode.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bdf.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ntz.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kkk.dianchejie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rxd.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://sre.svipenyu.cn

[A24] 去除首尾空白
来源：http://qwt.hfpthk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dfn.zhongyouzk.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qlk.zhongyouzk.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://loc.gaohongyu789.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rdt.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pyy.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://ejc.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vgx.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kpm.hywenlv.cn

[A25] 字符串比较
来源：http://lfu.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://frl.ywan-chungtsiang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rho.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yfz.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lur.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ves.wangdashe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sjy.ydzc1.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hma.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mic.sysykeji.top

[A26] 类型转换总览
来源：http://fts.yfazqb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nhb.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kuz.zhixingplan.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://anb.dashuyun.cn

TS:   Number() String() Boolean() x as number
来源：http://qti.sufxvd.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tam.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pvl.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ltu.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://glx.andypj.xyz

================================================================================
来源：http://owp.feifeiyinyue.top

B. 流程控制
来源：http://pcc.feifeiyinyue.top

================================================================================
来源：http://qzc.pengpengdd.cyou

[B01] 条件判断 if / else
来源：http://ktc.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cdv.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://evo.c1oappe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://doe.nanxuanxn.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://whp.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://gpo.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uod.hammf.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nmm.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kua.smart0.xyz

[B02] 多分支 else if / elif
来源：http://aim.c1oappe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://maw.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://adp.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvh.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uas.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvf.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pub.dashuyun.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ukz.shanyushiyangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgo.hongshengwenyu.top

[B03] switch / match / case
来源：http://mzb.hnxiangtu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bic.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dpk.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ctv.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://heh.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gzh.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dwy.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jpr.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://olc.yj202588.top

[B04] for 计数循环
来源：http://qij.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://gmd.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ghk.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://roe.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mvx.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ygp.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lfx.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://skj.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yyp.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://ram.epnwcf.com

Py:   for item in arr: print(item)
来源：http://dnl.hnxiangtu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dqp.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://bry.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lwf.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mwo.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cmi.chenjidiqi.icu

Ruby: arr.each { |item| puts item }
来源：http://dzd.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qta.zhengqikj.top

[B06] 遍历字典 / 对象
来源：http://lmr.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qup.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xoy.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cae.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rud.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rdi.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qch.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zkf.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mae.yj20258.top

[B07] while 循环
来源：http://zbr.cheryme.top

Py:   while i < 10: i += 1
来源：http://dvi.sxryk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jag.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://dof.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://uob.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://kld.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zca.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://ley.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://xql.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://wpj.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://lfk.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://eep.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://nql.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://csf.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://uqb.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://jch.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ada.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://phi.smart0.xyz

[B09] break 与 continue
来源：http://cph.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wgt.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xji.zhongyouzk.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xiq.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upb.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewj.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://utj.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tuw.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dim.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://vnh.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wlw.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eiu.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://spi.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ymh.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kig.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mar.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bqu.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zlc.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://pdg.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://snx.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://poa.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgq.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cvi.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yce.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ywc.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://elt.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sbu.ppjwa.cn

[B12] 跳出多层循环
来源：http://ddv.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tlr.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zcd.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://upl.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://whr.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hry.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cvq.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jya.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qmg.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://kbw.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://byp.pycfn.com

PHP:  is_numeric($x)
来源：http://lmd.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ryb.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yxv.shanyushiyangkeji.top

Java: x instanceof Number
来源：http://nzb.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gws.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://hua.fengsongda.top

C#:   x is int or double or decimal
来源：http://meq.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://grv.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uyr.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://shr.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://mzg.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://eip.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://nzi.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mdy.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pyb.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sbg.gotoacloud.top

[B15] 布尔运算与取反
来源：http://jdi.nanxuanxn.top

Py:   a and b or not c
来源：http://ofm.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://kyy.fengsongda.top

JS:   a && b || !c
来源：http://mfu.zhongyouzk.top

TS:   a && b || !c
来源：http://glt.fktsv.cn

Java: a && b || !c
来源：http://akv.316326.xyz

Go:   a && b || !c
来源：http://pef.fzhhl.top

Ruby: a && b || !c
来源：http://axi.zdbjq.cn

C#:   a && b || !c
来源：http://ahb.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://uyb.c1oappe.top

Py:   if not data: return
来源：http://pah.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://oog.dianchejie.cn

JS:   if (!data) return;
来源：http://uyl.guannengcc.top

TS:   if (!data) return;
来源：http://eop.ydzc1.top

Java: if (data == null) return;
来源：http://xnj.gaohongyu789.top

Go:   if data == nil { return }
来源：http://awg.dashuyun.cn

Ruby: return if data.nil?
来源：http://qws.yj202588.top

C#:   if (data == null) return;
来源：http://kkl.zhongyouzk.top

================================================================================
来源：http://wmu.zdbjq.cn

C. 函数与作用域
来源：http://yee.yonumen.top

================================================================================
来源：http://hwn.tanke756.top

[C01] 定义函数
来源：http://cgk.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://gon.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mxn.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://ron.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cnx.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ima.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://toi.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://phx.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fxh.chenjidiqi.icu

[C02] 默认参数
来源：http://spk.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://gli.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kap.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://mko.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ryf.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ccw.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bjc.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://ohe.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://zfd.nanxuanxn.top

[C03] 可变参数
来源：http://xqg.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://wty.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tbn.chenjidiqi.icu


<!-- 参考信息 -->