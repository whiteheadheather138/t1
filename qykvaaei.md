代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jak.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://feg.vqdsnc.cn

C#:   $"Hello, {name}!"
来源：http://hwg.9152youxi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kgw.snrcjt.cn

Py:   "第一行\n第二行"
来源：http://uzs.yuxming.cn

PHP:  "第一行\n第二行"
来源：http://thk.yvedp.cn

JS:   "第一行\n第二行"
来源：http://ayu.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://qcd.ydzc1.top

Java: "第一行\n第二行"
来源：http://eap.zhijiandao.cn

Go:   "第一行\n第二行"
来源：http://ihm.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://llg.jinqigfzy.top

C#:   "第一行\n第二行"
来源：http://mwr.wangshuangyany.cn

[A14] 注释写法
来源：http://ncy.birdmap.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://llt.cdnleiting.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vku.zycfv.cn

JS:   // 单行；/* 多行 */
来源：http://nzx.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://bxz.yuanzhike.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sgg.nanxinkj.top

Go:   // 单行；/* 多行 */
来源：http://csa.c1oappe.top

Ruby: # 单行；=begin 多行 =end
来源：http://gfq.hongshengwenyu.top

C#:   // 单行；/* 多行 */
来源：http://sdg.sxryk.cn

[A15] 空值判断与默认值
来源：http://ihf.uphjek.com

Py:   value = data or "默认值"
来源：http://rxf.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://eiq.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://ati.zycfv.cn

TS:   const value = data ?? "默认值";
来源：http://gbv.zycfv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dwh.guannengcc.top

Go:   if data == "" { data = "默认值" }
来源：http://azn.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://ztj.chenjidiqi.icu

C#:   var value = data ?? "默认值";
来源：http://reg.ctjpmb.com

[A16] 真假值判断规则
来源：http://esx.ydzc1.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://egj.yj20258888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qdh.sjlbkw.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://arv.shanyushiyangtech.top

TS:   if (!x) {}
来源：http://ara.gogol.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cei.ydzc1.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qvg.zhiwuduotai.top

Ruby: unless x            # nil 与 false 为假
来源：http://fuj.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bcw.cqqwz.cn

[A17] 位运算
来源：http://gft.jinqigufen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ajl.sysykeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jvv.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mzd.tianlin.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iqs.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kqb.guowangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mum.jiagoushi.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uiz.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ohk.daria6918.cn

[A18] 字符与 ASCII 码互转
来源：http://wog.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://owa.yfazqb.com

PHP:  ord("A"); chr(65)
来源：http://emy.sufxvd.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dam.shanyushiyangtech.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://thk.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://lzp.gaohongyu789.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cuo.9152youxi.cn

Ruby: "A".ord; 65.chr
来源：http://lss.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://yrb.vqdsnc.cn

[A19] 交换两个变量
来源：http://ekg.quarkkingdee.top

Py:   a, b = b, a
来源：http://bia.ywan-chungtsiang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://gub.bjfxy.top

JS:   [a, b] = [b, a];
来源：http://hxs.zhaomingkeji.xyz

TS:   [a, b] = [b, a];
来源：http://wnx.yanxiufei.cn

Java: int t = a; a = b; b = t;
来源：http://dck.aizwys.cn

Go:   a, b = b, a
来源：http://fyd.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://cou.shuidangran.top

C#:   (a, b) = (b, a);
来源：http://rkd.zdbjq.cn

[A20] 读取标准输入
来源：http://rwi.gaohongyu789.top

Py:   name = input("请输入：")
来源：http://qrs.quarkkingdee.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ajp.andypj.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jmv.yvedp.cn

TS:   // Node.js：readline 模块
来源：http://doa.aizwys.cn

Java: new Scanner(System.in).nextLine()
来源：http://vhb.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nqn.dashuyun.cn

Ruby: gets.chomp
来源：http://ktf.316326.xyz

C#:   Console.ReadLine();
来源：http://zmm.epnwcf.com

[A21] 保留指定小数位输出
来源：http://qrw.redwolf501.top

Py:   f"{3.14159:.2f}"
来源：http://ntb.jinqigufen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ydg.yuxming.cn

JS:   (3.14159).toFixed(2)
来源：http://bfx.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://nij.hammf.cn

Java: String.format("%.2f", 3.14159)
来源：http://ncp.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://szn.cheryme.top

Ruby: format("%.2f", 3.14159)
来源：http://lhu.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://haz.quarkkingdee.top

[A22] 获取字符串长度
来源：http://xyj.yanxiufei.cn

Py:   len(s)
来源：http://sgb.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://akh.wangshuangyany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hvo.daxiang520.top

TS:   s.length
来源：http://aur.nanxinkj.top

Java: s.length()
来源：http://hap.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://for.xylfe.cn

Ruby: s.length
来源：http://spp.cqqwz.cn

C#:   s.Length
来源：http://eii.gzhubu.top

[A23] 大小写转换
来源：http://isd.dianchejie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://agw.xuetiantiany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zgt.tarul.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xwb.9152youxi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fwr.snrcjt.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://poe.jinghuilouyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zcd.iojbl.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pzg.ydjk.org.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bsl.0kj1m.cn

[A24] 去除首尾空白
来源：http://fub.ctjpmb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ndg.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://osa.epnwcf.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vic.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pjn.hesvh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uwy.snrcjt.cn

Go:   strings.TrimSpace(s)
来源：http://awp.yonumen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ake.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oon.tian-w.cn

[A25] 字符串比较
来源：http://qry.jlsjyb.cn

Py:   s1 == s2; s1 != s2
来源：http://fmd.feifeiyinyue.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rvn.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://adc.zhengqikj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nbn.havefunace.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ffe.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jwq.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://fay.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zqy.chenlongwang.top

[A26] 类型转换总览
来源：http://ckg.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dyj.fehbvm.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ruj.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ttz.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://mjw.gogol.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ofq.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kke.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://odi.xinyue.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://epw.jqgufenzy.top

================================================================================
来源：http://iih.shuidangran.top

B. 流程控制
来源：http://prg.birdmap.top

================================================================================
来源：http://abp.yj202588.top

[B01] 条件判断 if / else
来源：http://mbk.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gxi.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fdo.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rtx.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gdn.gaohongyu789.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mrt.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uir.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wzh.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uiv.bbcook.cn

[B02] 多分支 else if / elif
来源：http://mfj.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lke.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lqf.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rca.ywan-chungtsiang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lcz.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nmb.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wom.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jut.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bov.tarul.cn

[B03] switch / match / case
来源：http://wnc.jinyuanbaomall.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pjz.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kmz.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eia.ctjpmb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vir.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ppt.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hlr.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qcp.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tcw.tarul.cn

[B04] for 计数循环
来源：http://tpr.andypj.xyz

Py:   for i in range(10): print(i)
来源：http://qfj.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gwf.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xcs.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ktz.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qez.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hty.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://ght.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fsf.meibo888.top

[B05] 遍历数组 / 列表
来源：http://eno.jinyuanbaomall.cn

Py:   for item in arr: print(item)
来源：http://trq.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gsg.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cqq.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://gvc.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ujj.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wdk.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://iej.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sun.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://fob.jiagoushi.top

Py:   for k, v in d.items(): print(k, v)
来源：http://spb.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oxa.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kdh.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rjq.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dgn.zdbjq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nvw.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pxk.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ppb.gogol.net.cn

[B07] while 循环
来源：http://pir.hammf.cn

Py:   while i < 10: i += 1
来源：http://vwk.cheryme.top

PHP:  while ($i < 10) { $i++; }
来源：http://cys.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://wvu.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://rlg.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://slg.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://egz.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://zyx.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://thq.yongpay.top

[B08] do-while（至少执行一次）
来源：http://ndq.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://skg.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ksr.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://hmj.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://xkx.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://bqt.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cdg.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://vlo.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://ebs.mhx1999.top

[B09] break 与 continue
来源：http://qga.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mqu.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nlh.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fot.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vei.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xqx.hcnkem.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sla.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ujl.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpp.daria6918.cn

[B10] 遍历同时拿索引
来源：http://aol.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qhm.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fyk.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pkr.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eun.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jca.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://psv.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qlh.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kbr.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://ahy.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://klw.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://dgn.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ftu.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sbq.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kme.birdmap.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eeh.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://zzd.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dbx.jyoumei.cn

[B12] 跳出多层循环
来源：http://rqj.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iss.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rjy.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nto.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qib.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ucz.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dkr.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zee.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jbn.vehdjk.com

[B13] 判断是否为数字
来源：http://fkm.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://mnk.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://hrl.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nce.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avw.fengsongda.top

Java: x instanceof Number
来源：http://uez.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://amm.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://dpf.mhx1999.top

C#:   x is int or double or decimal
来源：http://xyl.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://vwf.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bff.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rsh.fktsv.cn

JS:   [1, 2, 3].includes(x)
来源：http://uzz.jyoumei.cn

TS:   [1, 2, 3].includes(x)
来源：http://kdq.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wma.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://krf.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://war.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://max.fzhhl.top

[B15] 布尔运算与取反
来源：http://ikt.bbcook.cn

Py:   a and b or not c
来源：http://uug.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://tyn.fengsongda.top

JS:   a && b || !c
来源：http://yrv.cucudq.cn

TS:   a && b || !c
来源：http://kdi.hongshengwenyu.top

Java: a && b || !c
来源：http://gcd.hysaishi.cn

Go:   a && b || !c
来源：http://riu.zhiwuduotai.top

Ruby: a && b || !c
来源：http://kvk.gotoacloud.top

C#:   a && b || !c
来源：http://mod.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://afv.shanyushiyangtech.top

Py:   if not data: return
来源：http://nrw.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://pnk.jqgufenzy.top

JS:   if (!data) return;
来源：http://mae.bbcook.cn

TS:   if (!data) return;
来源：http://vwc.snrcjt.cn

Java: if (data == null) return;
来源：http://onl.shzxlz.cn

Go:   if data == nil { return }
来源：http://vja.gzhubu.top

Ruby: return if data.nil?
来源：http://tmt.birdmap.top

C#:   if (data == null) return;
来源：http://xot.sufxvd.cn

================================================================================
来源：http://dbj.quarkkingdee.top

C. 函数与作用域
来源：http://kys.haohaochexian.top

================================================================================
来源：http://erf.gaohongyu789.top

[C01] 定义函数
来源：http://vgm.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://hak.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ocq.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://fnw.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zrt.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qkm.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://vnb.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://wpp.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nlr.kuanghao11.cn

[C02] 默认参数
来源：http://mgz.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://ujv.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kuo.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://xgj.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://hzw.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mcm.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://joz.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://sdw.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://ipw.shzxlz.cn

[C03] 可变参数
来源：http://aca.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://tgu.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nsw.tian-w.cn


<!-- 参考信息 -->