代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wkb.svipenyu.cn

Java: new Random().nextInt(100) + 1
来源：http://lxr.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vnu.haohaochexian.top

Ruby: rand(1..100)
来源：http://yki.xuanzx.com

C#:   new Random().Next(1, 101)
来源：http://mbc.tanke756.top

[A11] 条件表达式（三元）
来源：http://jtu.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://sfx.bjfxy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uua.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kvv.pengpengdd.cyou

TS:   x > 0 ? "yes" : "no"
来源：http://mei.pengpengdd.cyou

Java: x > 0 ? "yes" : "no"
来源：http://pql.jinqigufen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dws.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://waz.chenzaomai.com

C#:   x > 0 ? "yes" : "no"
来源：http://ptz.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://bbd.fengsongda.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://afx.cqqwz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rxc.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://ysz.zhoulong.xyz

TS:   `Hello, ${name}!`
来源：http://iir.gotoacloud.top

Java: "Hello, %s!".formatted(name)
来源：http://mkw.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nzc.hywenlv.cn

Ruby: "Hello, #{name}!"
来源：http://fvs.jinqigufen.top

C#:   $"Hello, {name}!"
来源：http://flo.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gxc.hcnkem.com

Py:   "第一行\n第二行"
来源：http://dae.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://llp.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://ppv.hesvh.cn

TS:   "第一行\n第二行"
来源：http://oha.gogol.net.cn

Java: "第一行\n第二行"
来源：http://vuq.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://mnj.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://bti.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://crs.cdnleiting.top

[A14] 注释写法
来源：http://biv.snrcjt.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://frt.ctjpmb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://xzd.c1oappe.top

JS:   // 单行；/* 多行 */
来源：http://mib.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://uuj.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ixd.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://ulu.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://ukb.yonumen.top

C#:   // 单行；/* 多行 */
来源：http://wbn.jianghu66.top

[A15] 空值判断与默认值
来源：http://lhl.iojbl.cn

Py:   value = data or "默认值"
来源：http://fil.dianchejie.cn

PHP:  $value = $data ?? "默认值";
来源：http://hjw.jinqigfzy.top

JS:   const value = data ?? "默认值";
来源：http://ukt.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://wic.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://prf.quarkkingdee.top

Go:   if data == "" { data = "默认值" }
来源：http://jpl.pycfn.com

Ruby: value = data || "默认值"
来源：http://cor.xuetiantiany.cn

C#:   var value = data ?? "默认值";
来源：http://ogn.xziqi.cn

[A16] 真假值判断规则
来源：http://mkk.zhixingplan.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://odl.feifeiyinyue.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ekh.yuanzhike.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ltf.shzxlz.cn

TS:   if (!x) {}
来源：http://ama.52xcode.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mxn.daxiang520.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lzz.fehbvm.com

Ruby: unless x            # nil 与 false 为假
来源：http://bni.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vbn.feifeiyinyue.top

[A17] 位运算
来源：http://div.yvedp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssw.zdbjq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://exi.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lhm.zhijiandao.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wye.guannengcc.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jss.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bgj.zycfv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ved.cheryme.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jlx.gotoacloud.top

[A18] 字符与 ASCII 码互转
来源：http://wif.dashuyun.cn

Py:   ord("A"); chr(65)
来源：http://zmy.wangshuangyany.cn

PHP:  ord("A"); chr(65)
来源：http://lgd.ybcxt.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rbv.wangdashe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://grc.daria6918.cn

Java: (int) 'A'; (char) 65
来源：http://nib.yj202588.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dfs.ywan-chungtsiang.top

Ruby: "A".ord; 65.chr
来源：http://fdg.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://ylj.jqgufenzy.top

[A19] 交换两个变量
来源：http://wpd.gotoacloud.top

Py:   a, b = b, a
来源：http://roq.jlsjyb.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vod.yj202588.top

JS:   [a, b] = [b, a];
来源：http://lrq.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://auh.jqgufenzy.top

Java: int t = a; a = b; b = t;
来源：http://fun.wangdashe.top

Go:   a, b = b, a
来源：http://ilm.gzhubu.top

Ruby: a, b = b, a
来源：http://pvt.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://exk.birdmap.top

[A20] 读取标准输入
来源：http://eoz.fehbvm.com

Py:   name = input("请输入：")
来源：http://wks.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qou.hywenlv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nfq.zhaomingkeji.xyz

TS:   // Node.js：readline 模块
来源：http://srr.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://rjz.xuanzx.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iet.c1oappe.top

Ruby: gets.chomp
来源：http://qku.yuanzhike.top

C#:   Console.ReadLine();
来源：http://tjc.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://dhn.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://hfd.yangfankeji.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tza.aibaodan.cn

JS:   (3.14159).toFixed(2)
来源：http://aka.0kj1m.cn

TS:   (3.14159).toFixed(2)
来源：http://vzc.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://bph.zhongyouzk.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ssx.0kj1m.cn

Ruby: format("%.2f", 3.14159)
来源：http://nyu.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://mws.hammf.cn

[A22] 获取字符串长度
来源：http://zlp.xylfe.cn

Py:   len(s)
来源：http://pas.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wwi.316326.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vox.jinqigfzy.top

TS:   s.length
来源：http://jup.andypj.xyz

Java: s.length()
来源：http://pft.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://teo.daria6918.cn

Ruby: s.length
来源：http://ksx.haohaochexian.top

C#:   s.Length
来源：http://hvu.ydzc1.top

[A23] 大小写转换
来源：http://pbd.yanxiufei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bty.zhiwuduotai.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tqm.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://drk.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dox.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gpk.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://shk.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wyz.fengsongda.top

C#:   s.ToUpper(); s.ToLower()
来源：http://riy.gogol.net.cn

[A24] 去除首尾空白
来源：http://qur.uphjek.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fod.svipenyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hnq.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eti.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rhp.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zvu.dashuyun.cn

Go:   strings.TrimSpace(s)
来源：http://nzl.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tcy.vehdjk.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hks.yj20258888.top

[A25] 字符串比较
来源：http://psf.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://bsv.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://awz.wangdashe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vgg.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gbv.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hse.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rpk.yfazqb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://vsj.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hlj.pengpengdd.cyou

[A26] 类型转换总览
来源：http://xjo.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://teh.tarul.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tfd.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nqz.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://nzm.birdmap.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wmu.kuanghao11.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jjj.nanxuanxn.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://aml.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://law.gogol.net.cn

================================================================================
来源：http://pwg.xuanzx.com

B. 流程控制
来源：http://ffz.yongpay.top

================================================================================
来源：http://lnj.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://vsl.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://stj.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wuk.shzxlz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lhj.nwbrower.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://frg.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://npd.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rgz.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ltw.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://icw.andypj.xyz

[B02] 多分支 else if / elif
来源：http://zjq.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dvb.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vsj.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tzd.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ngm.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://akp.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cgl.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kpu.yvedp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nuw.vehdjk.com

[B03] switch / match / case
来源：http://tgk.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bnx.fengsongda.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pep.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aex.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jfx.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uhy.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vvm.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sie.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hgi.pycfn.com

[B04] for 计数循环
来源：http://mkb.jqgfzy.top

Py:   for i in range(10): print(i)
来源：http://alk.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://snb.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lsl.zhoulong.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://txs.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qdw.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://coq.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://xds.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gti.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://hol.birdmap.top

Py:   for item in arr: print(item)
来源：http://yls.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://llb.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://nhk.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kzg.epnwcf.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mfp.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eft.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://mug.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ait.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://wfu.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ypq.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wum.cheryme.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kvy.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gnw.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jxa.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://muk.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mtw.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eum.feifeiyinyue.top

[B07] while 循环
来源：http://yje.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://qqx.cheryme.top

PHP:  while ($i < 10) { $i++; }
来源：http://sgy.shuidangran.top

JS:   while (i < 10) { i++; }
来源：http://gpw.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://tlo.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://zbz.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dlv.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://ocs.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://bcs.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://ovh.xinyue.icu

Py:   # 无 do-while：用 while True + break
来源：http://pzp.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://jcr.xingfuxueyuan.xyz

JS:   do { i++; } while (i < 10);
来源：http://gjw.haohaochexian.top

TS:   do { i++; } while (i < 10);
来源：http://byn.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://cwu.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://hon.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pbh.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://slc.zhengqikj.top

[B09] break 与 continue
来源：http://mdk.yvedp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jml.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xmn.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wql.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yly.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cet.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jsh.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mqk.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dps.c1oappe.top

[B10] 遍历同时拿索引
来源：http://yax.redwolf501.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gqy.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wgq.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://szj.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ohs.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uiu.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gio.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uez.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jck.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://ujf.birdmap.top

Py:   list(range(0, 10, 2))
来源：http://wwk.cucudq.cn

PHP:  range(0, 10, 2);
来源：http://nhh.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eda.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mcp.gogol.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://col.ydzc1.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://myw.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://mpx.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xnr.hywenlv.cn

[B12] 跳出多层循环
来源：http://rzw.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qxy.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yva.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oit.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://arr.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tyy.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kqp.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ytg.zhaomingkeji.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ooe.9152youxi.cn

[B13] 判断是否为数字
来源：http://swq.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://pmx.gotoacloud.top

PHP:  is_numeric($x)
来源：http://uvh.xuetiantiany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kob.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://srl.xinyue.icu

Java: x instanceof Number
来源：http://ojn.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xwj.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://nus.yfazqb.com

C#:   x is int or double or decimal
来源：http://ojd.vehdjk.com

[B14] 判断值是否在集合内
来源：http://pby.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fjz.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yzd.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://tyo.zhijiandao.cn

TS:   [1, 2, 3].includes(x)
来源：http://etd.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gbt.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://reh.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://smn.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vsy.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://fpq.vqdsnc.cn

Py:   a and b or not c
来源：http://nmk.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://pbm.sjlbkw.cn

JS:   a && b || !c
来源：http://pns.jqgfzy.top

TS:   a && b || !c
来源：http://pxi.ywan-chungtsiang.top

Java: a && b || !c
来源：http://kdo.jinqigfzy.top

Go:   a && b || !c
来源：http://was.bjfxy.top

Ruby: a && b || !c
来源：http://ypd.yvedp.cn

C#:   a && b || !c
来源：http://sdi.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://cjj.xinyue.icu

Py:   if not data: return
来源：http://uda.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://pon.yueranfly.top

JS:   if (!data) return;
来源：http://fio.zhiwuduotai.top

TS:   if (!data) return;
来源：http://ehy.ctjpmb.com

Java: if (data == null) return;
来源：http://uim.zdbjq.cn

Go:   if data == nil { return }
来源：http://uvf.quarkkingdee.top

Ruby: return if data.nil?
来源：http://piu.316326.xyz

C#:   if (data == null) return;
来源：http://wxh.sysykeji.top

================================================================================
来源：http://cbd.jinqigfzy.top

C. 函数与作用域
来源：http://hie.pycfn.com

================================================================================
来源：http://uri.mhx1999.top

[C01] 定义函数
来源：http://mgn.meibo888.top


<!-- 参考信息 -->