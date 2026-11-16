代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://inh.daxiang520.top

Ruby: "Hello, #{name}!"
来源：http://hsi.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://hrf.jinqigfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fca.zdbjq.cn

Py:   "第一行\n第二行"
来源：http://gdi.yj20258.top

PHP:  "第一行\n第二行"
来源：http://sba.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://dll.aizwys.cn

TS:   "第一行\n第二行"
来源：http://bhv.sysykeji.top

Java: "第一行\n第二行"
来源：http://bya.xuetiantiany.cn

Go:   "第一行\n第二行"
来源：http://jhp.316326.xyz

Ruby: "第一行\n第二行"
来源：http://jji.zhoulong.xyz

C#:   "第一行\n第二行"
来源：http://lwm.hysaishi.cn

[A14] 注释写法
来源：http://hvx.yvedp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uxl.xuanzx.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://olt.havefunace.top

JS:   // 单行；/* 多行 */
来源：http://yio.ydjk.org.cn

TS:   // 单行；/* 多行 */
来源：http://lso.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fgn.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://nsu.havefunace.top

Ruby: # 单行；=begin 多行 =end
来源：http://klf.jinqigufen.top

C#:   // 单行；/* 多行 */
来源：http://fbo.yanxiufei.cn

[A15] 空值判断与默认值
来源：http://jpt.yangfankeji.com

Py:   value = data or "默认值"
来源：http://hoa.jiagoushi.top

PHP:  $value = $data ?? "默认值";
来源：http://yar.yj202588.top

JS:   const value = data ?? "默认值";
来源：http://lrd.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://xtm.zhaomingkeji.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mck.svipenyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://iic.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://mmv.tarul.cn

C#:   var value = data ?? "默认值";
来源：http://wor.c1oappe.top

[A16] 真假值判断规则
来源：http://fnl.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mmj.ctjpmb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ssw.yongpay.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hbx.yangfankeji.com

TS:   if (!x) {}
来源：http://ard.zycfv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lfs.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lia.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rsp.aizwys.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lej.yj20258888.top

[A17] 位运算
来源：http://rbf.jyoumei.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pee.quarkkingdee.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wlj.xziqi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hrx.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://juo.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uyx.xingfuxueyuan.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lhu.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dgj.gotoacloud.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vay.c1oappe.top

[A18] 字符与 ASCII 码互转
来源：http://nad.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://qfw.xingfuxueyuan.xyz

PHP:  ord("A"); chr(65)
来源：http://sly.yvedp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fsm.hcnkem.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lsu.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://zez.zhongyouzk.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mes.sufxvd.cn

Ruby: "A".ord; 65.chr
来源：http://zql.aibaodan.cn

C#:   (int)'A'; (char)65
来源：http://vzp.zdbjq.cn

[A19] 交换两个变量
来源：http://vpg.wangshuangyany.cn

Py:   a, b = b, a
来源：http://lad.jinghuilouyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://igl.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://egd.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://kpz.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://scw.zhengqikj.top

Go:   a, b = b, a
来源：http://prp.c1oappe.top

Ruby: a, b = b, a
来源：http://kyo.yonumen.top

C#:   (a, b) = (b, a);
来源：http://ntq.xylfe.cn

[A20] 读取标准输入
来源：http://rza.gogol.net.cn

Py:   name = input("请输入：")
来源：http://gbp.sweek.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mkz.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gly.sweek.top

TS:   // Node.js：readline 模块
来源：http://hmi.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://gzj.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jgh.dashuyun.cn

Ruby: gets.chomp
来源：http://bin.xinyue.icu

C#:   Console.ReadLine();
来源：http://jch.hesvh.cn

[A21] 保留指定小数位输出
来源：http://mdk.jinqigfzy.top

Py:   f"{3.14159:.2f}"
来源：http://vsc.ydjk.org.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cpb.chenzaomai.com

JS:   (3.14159).toFixed(2)
来源：http://xwy.ppjwa.cn

TS:   (3.14159).toFixed(2)
来源：http://vsy.ydzc1.top

Java: String.format("%.2f", 3.14159)
来源：http://kcy.fzhhl.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hwo.0kj1m.cn

Ruby: format("%.2f", 3.14159)
来源：http://iqq.tarul.cn

C#:   3.14159.ToString("F2")
来源：http://wnm.yfazqb.com

[A22] 获取字符串长度
来源：http://umd.dianchejie.cn

Py:   len(s)
来源：http://kyc.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wbm.smart0.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dvr.bjfxy.top

TS:   s.length
来源：http://uac.svipenyu.cn

Java: s.length()
来源：http://dcc.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ebe.bbcook.cn

Ruby: s.length
来源：http://voo.yj20258888.top

C#:   s.Length
来源：http://mbo.sufxvd.cn

[A23] 大小写转换
来源：http://lfv.yuanzhike.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kkp.vqdsnc.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pxu.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dhb.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dyd.andypj.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vmz.9152youxi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gsv.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pvg.tarul.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://icp.gotoacloud.top

[A24] 去除首尾空白
来源：http://lol.shangyingyoupin.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lff.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zvw.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://smi.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vvb.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ibm.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://vvk.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uuo.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hgb.mhx1999.top

[A25] 字符串比较
来源：http://vdb.feifeiyinyue.top

Py:   s1 == s2; s1 != s2
来源：http://kay.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kri.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://csg.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zvk.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lmk.nanxinkj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sbc.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nen.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://scv.hcnkem.com

[A26] 类型转换总览
来源：http://opq.dashuyun.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://moa.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sts.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rkx.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://vbp.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qbp.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wbz.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dea.zhongyouzk.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gwe.zhixingplan.top

================================================================================
来源：http://chc.yj202588.top

B. 流程控制
来源：http://kru.shzxlz.cn

================================================================================
来源：http://uea.yj202588.top

[B01] 条件判断 if / else
来源：http://aao.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jey.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jjv.sufxvd.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jih.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nre.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://nfm.svipenyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fik.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ota.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lbi.316326.xyz

[B02] 多分支 else if / elif
来源：http://rsz.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://okb.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ysx.jlsjyb.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zcd.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hyk.redwolf501.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dmi.yanxiufei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mlx.jinqigufen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vlr.pycfn.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oym.cashguo.top

[B03] switch / match / case
来源：http://obv.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ibv.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://due.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gmo.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pnh.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lqd.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fcq.316326.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wmd.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yvd.yj20258888.top

[B04] for 计数循环
来源：http://vrx.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://rwi.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xnc.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yjd.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iut.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ini.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://byn.jqgufenzy.top

Ruby: 10.times { |i| puts i }
来源：http://aut.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qaa.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://njm.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://qba.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hcy.jqgufenzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://oik.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ibq.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://sco.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pkm.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://zdk.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fdv.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://wbo.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hew.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fqj.xingfuxueyuan.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://biv.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mqa.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ldc.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://osz.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wbd.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wvt.ppjwa.cn

[B07] while 循环
来源：http://hhh.fengsongda.top

Py:   while i < 10: i += 1
来源：http://bbh.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://ulm.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://lsv.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://zpk.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://xfv.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://awj.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://whz.tianlin.xyz

C#:   while (i < 10) { i++; }
来源：http://akp.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://igh.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://pbu.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://vem.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://jld.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://lmo.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://hgz.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ygw.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vlk.yj20258.top

C#:   do { i++; } while (i < 10);
来源：http://jni.zhengqikj.top

[B09] break 与 continue
来源：http://yyl.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kkg.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zmo.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmk.daxiang520.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lau.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://htk.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kni.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yby.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vnz.epnwcf.com

[B10] 遍历同时拿索引
来源：http://frq.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tin.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xwv.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://twm.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qeg.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fhv.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://deg.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qld.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dxu.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://oyi.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://leb.hammf.cn

PHP:  range(0, 10, 2);
来源：http://tit.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vqx.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hur.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rfc.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tzr.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://znx.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vwk.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://lps.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wey.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://thc.316326.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://crd.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ayj.vqdsnc.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://svq.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wgj.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qca.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ffa.gotoacloud.top

[B13] 判断是否为数字
来源：http://kag.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://ueo.yuanzhike.top

PHP:  is_numeric($x)
来源：http://mtr.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gpd.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kps.ctjpmb.com

Java: x instanceof Number
来源：http://kwd.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qay.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://xmk.yj202588.top

C#:   x is int or double or decimal
来源：http://rme.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://dcn.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hvn.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://esg.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://nrx.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://aci.shangyingyoupin.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xjl.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sxv.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://wny.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pcw.daxiang520.top

[B15] 布尔运算与取反
来源：http://ocd.sxryk.cn

Py:   a and b or not c
来源：http://fpa.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://lxt.0kj1m.cn

JS:   a && b || !c
来源：http://qag.jqgufenzy.top

TS:   a && b || !c
来源：http://tlz.aibaodan.cn

Java: a && b || !c
来源：http://bux.ppjwa.cn

Go:   a && b || !c
来源：http://nbq.hesvh.cn

Ruby: a && b || !c
来源：http://zmb.vehdjk.com

C#:   a && b || !c
来源：http://oks.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://qvx.fengsongda.top

Py:   if not data: return
来源：http://lsk.pycfn.com

PHP:  if (!$data) { return; }
来源：http://wsj.xuanzx.com

JS:   if (!data) return;
来源：http://xfq.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://dio.quarkkingdee.top

Java: if (data == null) return;
来源：http://rrj.52xcode.cn

Go:   if data == nil { return }
来源：http://rvv.birdmap.top

Ruby: return if data.nil?
来源：http://dsz.yongpay.top

C#:   if (data == null) return;
来源：http://sgu.yuxming.cn

================================================================================
来源：http://tdd.yueranfly.top

C. 函数与作用域
来源：http://oik.andypj.xyz

================================================================================
来源：http://kan.nanxinkj.top

[C01] 定义函数
来源：http://aoc.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://ixg.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wov.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://bvq.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://urn.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vkg.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://zqk.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://pso.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wpz.chenzaomai.com

[C02] 默认参数
来源：http://wzk.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://qcx.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://grl.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://ctf.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kdl.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ijj.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ecz.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://fzz.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://mfi.aizwys.cn

[C03] 可变参数
来源：http://dqe.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://sxe.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xbc.sxryk.cn


<!-- 参考信息 -->