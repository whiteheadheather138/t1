代发 wailian999

Py:   "第一行\n第二行"
来源：http://zfm.meibo888.top

PHP:  "第一行\n第二行"
来源：http://ugm.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://qbt.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://stp.gotoacloud.top

Java: "第一行\n第二行"
来源：http://itu.zhaomingkeji.xyz

Go:   "第一行\n第二行"
来源：http://zky.yonumen.top

Ruby: "第一行\n第二行"
来源：http://osv.guowangkeji.top

C#:   "第一行\n第二行"
来源：http://dao.sjlbkw.cn

[A14] 注释写法
来源：http://pij.zhoulong.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://jat.zhijiandao.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://unf.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://fnj.quarkkingdee.top

TS:   // 单行；/* 多行 */
来源：http://uwt.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oqa.andypj.xyz

Go:   // 单行；/* 多行 */
来源：http://blr.redwolf501.top

Ruby: # 单行；=begin 多行 =end
来源：http://wxl.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://mzb.nwbrower.top

[A15] 空值判断与默认值
来源：http://fnw.dianchejie.cn

Py:   value = data or "默认值"
来源：http://ibu.gaohongyu789.top

PHP:  $value = $data ?? "默认值";
来源：http://hvh.haohaochexian.top

JS:   const value = data ?? "默认值";
来源：http://gil.iojbl.cn

TS:   const value = data ?? "默认值";
来源：http://nby.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://adx.pycfn.com

Go:   if data == "" { data = "默认值" }
来源：http://vmr.yvedp.cn

Ruby: value = data || "默认值"
来源：http://vdo.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://dbx.meibo888.top

[A16] 真假值判断规则
来源：http://xbi.ywan-chungtsiang.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hdk.gogol.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vuu.cqqwz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vib.ehwqpu.com

TS:   if (!x) {}
来源：http://fvj.cashguo.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qds.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ulk.sxryk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uhk.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sbd.yanxiufei.cn

[A17] 位运算
来源：http://cme.0kj1m.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ijh.nwbrower.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iyc.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ium.feifeiyinyue.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bya.birdmap.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dhb.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://csf.chenzaomai.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xwb.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fbf.aizwys.cn

[A18] 字符与 ASCII 码互转
来源：http://jrk.daria6918.cn

Py:   ord("A"); chr(65)
来源：http://cau.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://onc.zdbjq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://apv.zhengqikj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xru.hywenlv.cn

Java: (int) 'A'; (char) 65
来源：http://vkc.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mlp.wangdashe.top

Ruby: "A".ord; 65.chr
来源：http://vrx.guannengcc.top

C#:   (int)'A'; (char)65
来源：http://eoj.smart0.xyz

[A19] 交换两个变量
来源：http://twu.yangfankeji.com

Py:   a, b = b, a
来源：http://fcm.chenlongwang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hzt.guannengcc.top

JS:   [a, b] = [b, a];
来源：http://fwr.cqqwz.cn

TS:   [a, b] = [b, a];
来源：http://dmt.sufxvd.cn

Java: int t = a; a = b; b = t;
来源：http://taw.epnwcf.com

Go:   a, b = b, a
来源：http://crm.mhx1999.top

Ruby: a, b = b, a
来源：http://oeh.52xcode.cn

C#:   (a, b) = (b, a);
来源：http://rrt.hfpthk.cn

[A20] 读取标准输入
来源：http://wyc.hammf.cn

Py:   name = input("请输入：")
来源：http://bpd.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cor.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jra.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://vyt.sjlbkw.cn

Java: new Scanner(System.in).nextLine()
来源：http://edb.jqgufenzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dpx.chenzaomai.com

Ruby: gets.chomp
来源：http://bfz.xziqi.cn

C#:   Console.ReadLine();
来源：http://bka.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://ayj.daria6918.cn

Py:   f"{3.14159:.2f}"
来源：http://ecv.havefunace.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lhz.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://itm.zhongyouzk.top

TS:   (3.14159).toFixed(2)
来源：http://rza.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://qjg.shanyushiyangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tcu.zdqjudy.top

Ruby: format("%.2f", 3.14159)
来源：http://asw.cashguo.top

C#:   3.14159.ToString("F2")
来源：http://qfs.shanyushiyangtech.top

[A22] 获取字符串长度
来源：http://ohg.jqgfzy.top

Py:   len(s)
来源：http://tbg.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zkj.zhongyouzk.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gtr.nanxuanxn.top

TS:   s.length
来源：http://xdu.gaohongyu789.top

Java: s.length()
来源：http://tan.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zim.fehbvm.com

Ruby: s.length
来源：http://gbr.tarul.cn

C#:   s.Length
来源：http://omh.quarkkingdee.top

[A23] 大小写转换
来源：http://uqv.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://prq.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ofa.shzxlz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zsa.shanyushiyangtech.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tmq.quarkkingdee.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zzn.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://plh.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fkv.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://abz.shuidangran.top

[A24] 去除首尾空白
来源：http://fir.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ytf.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vva.gaohongyu789.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rlx.svipenyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kwh.haohaochexian.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eaf.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://biz.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qwg.gaohongyu789.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eln.cucudq.cn

[A25] 字符串比较
来源：http://kxu.ydzc1.top

Py:   s1 == s2; s1 != s2
来源：http://tew.daxiang520.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ayi.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mrh.sysykeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hkj.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://efe.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ncn.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xhv.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yqn.gotoacloud.top

[A26] 类型转换总览
来源：http://kwg.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wgi.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iik.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://okm.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://kob.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pzx.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uxo.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://zvw.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nfw.sysykeji.top

================================================================================
来源：http://ajr.yfazqb.com

B. 流程控制
来源：http://pyy.haohaochexian.top

================================================================================
来源：http://qyv.hammf.cn

[B01] 条件判断 if / else
来源：http://wab.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qmf.ybcxt.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://meo.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ruo.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vkk.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nir.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ecj.52xcode.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://seg.pycfn.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gnf.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://kri.hfpthk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rxn.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://htf.vehdjk.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iwa.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogr.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mwd.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rly.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jiy.xuanzx.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vab.sxryk.cn

[B03] switch / match / case
来源：http://wnn.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zit.sjlbkw.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aco.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cpz.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kte.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bbh.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vlq.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aad.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rjt.zhixingplan.top

[B04] for 计数循环
来源：http://wcj.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://ozk.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cul.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iai.sxryk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vid.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://osf.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wkw.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://oco.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fri.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://ttd.fehbvm.com

Py:   for item in arr: print(item)
来源：http://ajz.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ecj.bbcook.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iqq.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jrb.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://onn.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tng.tian-w.cn

Ruby: arr.each { |item| puts item }
来源：http://bxx.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ods.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://uzp.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dhx.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nqv.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txw.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ayn.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wyy.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://chn.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jqz.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cmq.52xcode.cn

[B07] while 循环
来源：http://peh.ivvv.top

Py:   while i < 10: i += 1
来源：http://oxo.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cak.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://qwn.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://mlo.zhijiandao.cn

Java: while (i < 10) { i++; }
来源：http://rqm.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bjn.jqgfzy.top

Ruby: while i < 10; i += 1; end
来源：http://jze.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://dtv.hammf.cn

[B08] do-while（至少执行一次）
来源：http://odb.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://jfh.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vio.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://kqw.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://csf.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://lso.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://avi.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://joz.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://btr.zhijiandao.cn

[B09] break 与 continue
来源：http://rwf.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vxs.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yjt.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kgx.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ngv.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smo.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vzu.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mzd.meibo888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bhu.zhoulong.xyz

[B10] 遍历同时拿索引
来源：http://qpl.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lyp.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sqp.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vug.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lrl.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vnn.zhiwuduotai.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ost.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hls.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qht.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://lrq.ppjwa.cn

Py:   list(range(0, 10, 2))
来源：http://qvv.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://etw.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qjv.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://luy.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cfr.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://psm.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://znv.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dll.sxryk.cn

[B12] 跳出多层循环
来源：http://grl.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wid.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://flc.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wsg.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://igm.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ilk.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://juf.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pjf.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://apk.sysykeji.top

[B13] 判断是否为数字
来源：http://bsp.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://zao.jianghu66.top

PHP:  is_numeric($x)
来源：http://xch.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fwy.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xsm.tian-w.cn

Java: x instanceof Number
来源：http://jwa.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lcw.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://dty.hcnkem.com

C#:   x is int or double or decimal
来源：http://dgt.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://bxd.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eyr.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pqe.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://pmw.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://vjz.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ozh.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zbo.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://ujm.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ajo.andypj.xyz

[B15] 布尔运算与取反
来源：http://ioq.yvedp.cn

Py:   a and b or not c
来源：http://xux.meibo888.top

PHP:  $a && $b || !$c
来源：http://ncs.zhengqikj.top

JS:   a && b || !c
来源：http://fbr.sxryk.cn

TS:   a && b || !c
来源：http://nob.zdbjq.cn

Java: a && b || !c
来源：http://ria.cqqwz.cn

Go:   a && b || !c
来源：http://pse.daxiang520.top

Ruby: a && b || !c
来源：http://gcw.sufxvd.cn

C#:   a && b || !c
来源：http://vdj.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yfw.316326.xyz

Py:   if not data: return
来源：http://czw.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://zwj.fanxiaobao.xyz

JS:   if (!data) return;
来源：http://adm.fehbvm.com

TS:   if (!data) return;
来源：http://kce.hongshengwenyu.top

Java: if (data == null) return;
来源：http://whp.zhixingplan.top

Go:   if data == nil { return }
来源：http://duw.chenlongwang.top

Ruby: return if data.nil?
来源：http://czf.bjfxy.top

C#:   if (data == null) return;
来源：http://duj.yfazqb.com

================================================================================
来源：http://ung.yanxiufei.cn

C. 函数与作用域
来源：http://fms.yonumen.top

================================================================================
来源：http://pas.daxiang520.top

[C01] 定义函数
来源：http://lmw.yongpay.top

Py:   def add(a, b): return a + b
来源：http://ewo.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vgq.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://hem.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdg.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fcq.yueranfly.top

Go:   func add(a, b int) int { return a + b }
来源：http://snh.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://ilk.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rat.mhx1999.top

[C02] 默认参数
来源：http://naq.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://mhw.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bgo.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://zkf.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tmf.zhongyouzk.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nbd.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fpz.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://pdy.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://xhu.yueranfly.top

[C03] 可变参数
来源：http://lng.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://wru.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vmn.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://khn.xingfuxueyuan.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mba.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fjc.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wlr.fanxiaobao.xyz


<!-- 参考信息 -->