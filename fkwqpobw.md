代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://dpr.shuidangran.top

TS:   x > 0 ? "yes" : "no"
来源：http://ngf.hcnkem.com

Java: x > 0 ? "yes" : "no"
来源：http://omv.xinyue.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://hux.cdnleiting.top

Ruby: x > 0 ? "yes" : "no"
来源：http://noq.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://orv.havefunace.top

[A12] 字符串插值 / 格式化
来源：http://fkn.yvedp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bnl.ydjk.org.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xvf.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://ain.zhoulong.xyz

TS:   `Hello, ${name}!`
来源：http://ryx.xingfuxueyuan.xyz

Java: "Hello, %s!".formatted(name)
来源：http://bas.sysykeji.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://svm.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://rwp.bbcook.cn

C#:   $"Hello, {name}!"
来源：http://fix.birdmap.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ghj.xuanzx.com

Py:   "第一行\n第二行"
来源：http://qlp.iojbl.cn

PHP:  "第一行\n第二行"
来源：http://mjr.fehbvm.com

JS:   "第一行\n第二行"
来源：http://aud.jiagoushi.top

TS:   "第一行\n第二行"
来源：http://dzc.yanxiufei.cn

Java: "第一行\n第二行"
来源：http://ipz.fengsongda.top

Go:   "第一行\n第二行"
来源：http://mrs.yongpay.top

Ruby: "第一行\n第二行"
来源：http://xko.daria6918.cn

C#:   "第一行\n第二行"
来源：http://cds.shzxlz.cn

[A14] 注释写法
来源：http://due.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wsq.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ocm.ehwqpu.com

JS:   // 单行；/* 多行 */
来源：http://oax.hongshengwenyu.top

TS:   // 单行；/* 多行 */
来源：http://ayz.yuxming.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jyz.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://dax.wangdashe.top

Ruby: # 单行；=begin 多行 =end
来源：http://dye.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://ftf.ydzc1.top

[A15] 空值判断与默认值
来源：http://hwm.zdbjq.cn

Py:   value = data or "默认值"
来源：http://pnj.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://zpk.birdmap.top

JS:   const value = data ?? "默认值";
来源：http://hiq.hesvh.cn

TS:   const value = data ?? "默认值";
来源：http://nfo.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dpp.tian-w.cn

Go:   if data == "" { data = "默认值" }
来源：http://ccv.shuidangran.top

Ruby: value = data || "默认值"
来源：http://qrc.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://ton.fanxiaobao.xyz

[A16] 真假值判断规则
来源：http://sxi.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eho.daria6918.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aai.nanxuanxn.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eca.cdnleiting.top

TS:   if (!x) {}
来源：http://rvy.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mks.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wnh.hesvh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zto.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yoq.gogol.net.cn

[A17] 位运算
来源：http://awf.jqgfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pat.xuetiantiany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bgg.ivvv.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ybu.quarkkingdee.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nrk.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vin.xingfuxueyuan.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ahw.jinghuilouyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kky.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ubp.9152youxi.cn

[A18] 字符与 ASCII 码互转
来源：http://nym.svipenyu.cn

Py:   ord("A"); chr(65)
来源：http://tvc.ehwqpu.com

PHP:  ord("A"); chr(65)
来源：http://blg.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bhu.cdnleiting.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cns.cqqwz.cn

Java: (int) 'A'; (char) 65
来源：http://qds.cdnleiting.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://juy.jinqigfzy.top

Ruby: "A".ord; 65.chr
来源：http://poi.jinghuilouyu.cn

C#:   (int)'A'; (char)65
来源：http://gsl.shzxlz.cn

[A19] 交换两个变量
来源：http://gdi.feifeiyinyue.top

Py:   a, b = b, a
来源：http://bdv.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://geh.hammf.cn

JS:   [a, b] = [b, a];
来源：http://nez.uphjek.com

TS:   [a, b] = [b, a];
来源：http://vmb.jianghu66.top

Java: int t = a; a = b; b = t;
来源：http://plo.shangyingyoupin.top

Go:   a, b = b, a
来源：http://utu.zhijiandao.cn

Ruby: a, b = b, a
来源：http://gwm.nanxinkj.top

C#:   (a, b) = (b, a);
来源：http://tjg.hcnkem.com

[A20] 读取标准输入
来源：http://bjt.jinqigfzy.top

Py:   name = input("请输入：")
来源：http://mkq.chenzaomai.com

PHP:  $name = trim(fgets(STDIN));
来源：http://moj.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hnm.ivvv.top

TS:   // Node.js：readline 模块
来源：http://wpo.chenlongwang.top

Java: new Scanner(System.in).nextLine()
来源：http://bpb.chenlongwang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yor.zhiwuduotai.top

Ruby: gets.chomp
来源：http://npe.feifeiyinyue.top

C#:   Console.ReadLine();
来源：http://afj.snrcjt.cn

[A21] 保留指定小数位输出
来源：http://rfc.tarul.cn

Py:   f"{3.14159:.2f}"
来源：http://urv.yuanzhike.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mir.cqqwz.cn

JS:   (3.14159).toFixed(2)
来源：http://wcp.yueranfly.top

TS:   (3.14159).toFixed(2)
来源：http://gdf.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://qrj.c1oappe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://acm.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://lwi.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://pzo.daria6918.cn

[A22] 获取字符串长度
来源：http://mum.xinyue.icu

Py:   len(s)
来源：http://pld.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ceg.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kpa.fehbvm.com

TS:   s.length
来源：http://htc.cashguo.top

Java: s.length()
来源：http://xka.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lqt.hnqzz.top

Ruby: s.length
来源：http://ehh.cqqwz.cn

C#:   s.Length
来源：http://klw.andypj.xyz

[A23] 大小写转换
来源：http://goc.guannengcc.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mvv.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uam.zhijiandao.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xic.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mzv.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nnx.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sfl.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ovx.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ord.yj20258.top

[A24] 去除首尾空白
来源：http://lka.dashuyun.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://grb.xziqi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jaa.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cxh.yueranfly.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tse.vehdjk.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wpu.yfazqb.com

Go:   strings.TrimSpace(s)
来源：http://dwa.hysaishi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qcx.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hyh.xziqi.cn

[A25] 字符串比较
来源：http://iih.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://vhw.meibo888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tsu.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sla.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oom.wangdashe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pfn.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rbl.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fbd.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://trq.hcnkem.com

[A26] 类型转换总览
来源：http://mfs.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rfv.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qod.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wnh.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://lbs.feifeiyinyue.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://heq.dashuyun.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fqh.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://dzh.gogol.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fbh.tianlin.xyz

================================================================================
来源：http://ajg.bjfxy.top

B. 流程控制
来源：http://fbg.cucudq.cn

================================================================================
来源：http://arj.zdqjudy.top

[B01] 条件判断 if / else
来源：http://rcz.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lsv.ybcxt.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cjq.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xib.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bjf.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ari.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tsf.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zck.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uov.hcnkem.com

[B02] 多分支 else if / elif
来源：http://ixh.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jbi.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eaz.yuxming.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tsp.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fnr.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vfr.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bfn.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://obq.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyk.daria6918.cn

[B03] switch / match / case
来源：http://fdr.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iop.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zhm.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rgy.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sgg.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kzx.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nxl.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pjv.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dei.haohaochexian.top

[B04] for 计数循环
来源：http://ofo.fzhhl.top

Py:   for i in range(10): print(i)
来源：http://sgd.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rvz.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vfo.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oft.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hcc.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jik.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://bpi.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sgb.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://uns.zdbjq.cn

Py:   for item in arr: print(item)
来源：http://ght.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ljd.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://snh.birdmap.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qiu.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://wda.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wof.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://rgp.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kuj.ydjk.org.cn

[B06] 遍历字典 / 对象
来源：http://hah.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zhe.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hnh.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dxo.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gyu.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zio.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gtj.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uzt.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jim.cheryme.top

[B07] while 循环
来源：http://uvw.guowangkeji.top

Py:   while i < 10: i += 1
来源：http://rhm.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rlj.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://dgl.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://ktk.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://qnu.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://chr.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://rzk.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://fti.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://kaa.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://hob.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://kcs.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://wdd.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://gjq.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://rgu.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xzc.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pmi.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://sdu.jinghuilouyu.cn

[B09] break 与 continue
来源：http://doh.bjfxy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://haa.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qry.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mrl.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mcl.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmr.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://giu.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tcj.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dhw.yj202588.top

[B10] 遍历同时拿索引
来源：http://wuv.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xqd.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rjy.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dfi.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ymy.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pef.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://srr.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uyb.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bba.sjlbkw.cn

[B11] 生成数字序列 / 区间
来源：http://rmw.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://ufk.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://dee.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ohk.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://unc.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jat.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qho.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://cru.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ghd.fengsongda.top

[B12] 跳出多层循环
来源：http://agb.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qjg.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uvc.tianlin.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xzn.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cym.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yfq.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eoy.gzhubu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wln.ctjpmb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gyo.birdmap.top

[B13] 判断是否为数字
来源：http://ozm.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://ubt.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://wqf.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vgf.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fca.yuanzhike.top

Java: x instanceof Number
来源：http://tkx.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gye.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://zpo.fengsongda.top

C#:   x is int or double or decimal
来源：http://owl.ybcxt.top

[B14] 判断值是否在集合内
来源：http://ccp.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://plt.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fgi.dashuyun.cn

JS:   [1, 2, 3].includes(x)
来源：http://ttd.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://zmf.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://czp.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hmb.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://hwj.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ifs.jianghu66.top

[B15] 布尔运算与取反
来源：http://rua.c1oappe.top

Py:   a and b or not c
来源：http://vae.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://dng.tarul.cn

JS:   a && b || !c
来源：http://cty.mhx1999.top

TS:   a && b || !c
来源：http://xpp.yangfankeji.com

Java: a && b || !c
来源：http://gwf.hfpthk.cn

Go:   a && b || !c
来源：http://gfk.jianghu66.top

Ruby: a && b || !c
来源：http://bli.jqgfzy.top

C#:   a && b || !c
来源：http://dtv.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://jut.pycfn.com

Py:   if not data: return
来源：http://zya.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://teg.snrcjt.cn

JS:   if (!data) return;
来源：http://inm.9152youxi.cn

TS:   if (!data) return;
来源：http://vtn.meibo888.top

Java: if (data == null) return;
来源：http://qen.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://cyh.sjlbkw.cn

Ruby: return if data.nil?
来源：http://bai.haohaochexian.top

C#:   if (data == null) return;
来源：http://yrd.yanxiufei.cn

================================================================================
来源：http://pyc.zdqjudy.top

C. 函数与作用域
来源：http://dph.jyoumei.cn

================================================================================
来源：http://fgq.jinghuilouyu.cn

[C01] 定义函数
来源：http://nnm.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://bfu.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pju.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://plo.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nki.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://cgc.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://jft.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://ang.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cip.yonumen.top


<!-- 参考信息 -->