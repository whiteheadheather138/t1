代发 wailian999

Py:   "第一行\n第二行"
来源：http://gsz.zhoulong.xyz

PHP:  "第一行\n第二行"
来源：http://qxx.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://kyq.fengsongda.top

TS:   "第一行\n第二行"
来源：http://qrl.zdqjudy.top

Java: "第一行\n第二行"
来源：http://elq.chenjidiqi.icu

Go:   "第一行\n第二行"
来源：http://fyq.daxiang520.top

Ruby: "第一行\n第二行"
来源：http://bhg.hammf.cn

C#:   "第一行\n第二行"
来源：http://oqm.jinqigufen.top

[A14] 注释写法
来源：http://hjz.bbcook.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tsq.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cnc.vqdsnc.cn

JS:   // 单行；/* 多行 */
来源：http://ble.gaohongyu789.top

TS:   // 单行；/* 多行 */
来源：http://zcr.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ira.gotoacloud.top

Go:   // 单行；/* 多行 */
来源：http://cms.zhengqikj.top

Ruby: # 单行；=begin 多行 =end
来源：http://fua.mhx1999.top

C#:   // 单行；/* 多行 */
来源：http://lmd.uphjek.com

[A15] 空值判断与默认值
来源：http://nah.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://isd.fanxiaobao.xyz

PHP:  $value = $data ?? "默认值";
来源：http://jyd.ydjk.org.cn

JS:   const value = data ?? "默认值";
来源：http://pcz.yueranfly.top

TS:   const value = data ?? "默认值";
来源：http://uwr.dianchejie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vzi.yfazqb.com

Go:   if data == "" { data = "默认值" }
来源：http://tsb.shanyushiyangtech.top

Ruby: value = data || "默认值"
来源：http://kgd.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://mmb.cashguo.top

[A16] 真假值判断规则
来源：http://xar.epnwcf.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fgz.iojbl.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vrn.sxryk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://euf.ywan-chungtsiang.top

TS:   if (!x) {}
来源：http://igy.gaohongyu789.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vkv.jianghu66.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nhr.vehdjk.com

Ruby: unless x            # nil 与 false 为假
来源：http://cbp.tarul.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://acb.tanke756.top

[A17] 位运算
来源：http://vsf.ybcxt.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qip.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qsb.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dpz.tian-w.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wfo.jinqigfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kgh.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yyw.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://unr.ehwqpu.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tuo.jqgufenzy.top

[A18] 字符与 ASCII 码互转
来源：http://zjz.9152youxi.cn

Py:   ord("A"); chr(65)
来源：http://pnd.birdmap.top

PHP:  ord("A"); chr(65)
来源：http://fao.cheryme.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vci.yuxming.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xlt.9152youxi.cn

Java: (int) 'A'; (char) 65
来源：http://ytg.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zjw.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://bzx.xinyue.icu

C#:   (int)'A'; (char)65
来源：http://cbn.ydjk.org.cn

[A19] 交换两个变量
来源：http://ahx.smart0.xyz

Py:   a, b = b, a
来源：http://zbl.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://nop.yueranfly.top

JS:   [a, b] = [b, a];
来源：http://eqa.uphjek.com

TS:   [a, b] = [b, a];
来源：http://qhj.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://yiw.nwbrower.top

Go:   a, b = b, a
来源：http://ilb.ydjk.org.cn

Ruby: a, b = b, a
来源：http://zwt.zhijiandao.cn

C#:   (a, b) = (b, a);
来源：http://msy.zdqjudy.top

[A20] 读取标准输入
来源：http://whf.hesvh.cn

Py:   name = input("请输入：")
来源：http://btx.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://raz.xuetiantiany.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mxv.wangshuangyany.cn

TS:   // Node.js：readline 模块
来源：http://luo.ppjwa.cn

Java: new Scanner(System.in).nextLine()
来源：http://rjg.zdqjudy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xku.zhoulong.xyz

Ruby: gets.chomp
来源：http://gkg.sufxvd.cn

C#:   Console.ReadLine();
来源：http://vag.0kj1m.cn

[A21] 保留指定小数位输出
来源：http://mur.yuxming.cn

Py:   f"{3.14159:.2f}"
来源：http://lrr.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://axc.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://dzo.yanxiufei.cn

TS:   (3.14159).toFixed(2)
来源：http://hpg.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://llz.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tgx.andypj.xyz

Ruby: format("%.2f", 3.14159)
来源：http://oha.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://lir.fengsongda.top

[A22] 获取字符串长度
来源：http://wmp.xingfuxueyuan.xyz

Py:   len(s)
来源：http://how.yvedp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bit.yueranfly.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://esh.gogol.net.cn

TS:   s.length
来源：http://uok.c1oappe.top

Java: s.length()
来源：http://myg.epnwcf.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zkx.daria6918.cn

Ruby: s.length
来源：http://zyo.haohaochexian.top

C#:   s.Length
来源：http://hiw.tianlin.xyz

[A23] 大小写转换
来源：http://kbe.jqgfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pjz.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ldh.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ica.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zbw.daxiang520.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pji.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jdg.jqgufenzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://evh.yangfankeji.com

C#:   s.ToUpper(); s.ToLower()
来源：http://rut.vqdsnc.cn

[A24] 去除首尾空白
来源：http://byx.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pdp.cashguo.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bwf.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://afi.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mqr.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://act.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://fsh.svipenyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ark.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jmx.c1oappe.top

[A25] 字符串比较
来源：http://ckf.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://duo.fehbvm.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eia.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lyn.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fjz.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vzm.jinyuanbaomall.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gna.zhiwuduotai.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hrj.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yyt.nwbrower.top

[A26] 类型转换总览
来源：http://zhz.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://inr.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jvi.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tzu.xziqi.cn

TS:   Number() String() Boolean() x as number
来源：http://lux.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fxf.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aox.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bjo.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rdw.sjlbkw.cn

================================================================================
来源：http://jzt.xingfuxueyuan.xyz

B. 流程控制
来源：http://xmt.bbcook.cn

================================================================================
来源：http://otc.jlsjyb.cn

[B01] 条件判断 if / else
来源：http://kfp.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ovn.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ubc.yuxming.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bzd.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ugu.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qva.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ska.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lbq.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://opa.zhaomingkeji.xyz

[B02] 多分支 else if / elif
来源：http://glj.zycfv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zhi.havefunace.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fxe.feifeiyinyue.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lfi.quarkkingdee.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qhz.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wsa.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hfm.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pyk.nanxinkj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xhu.xuanzx.com

[B03] switch / match / case
来源：http://yke.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://grm.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://res.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jrp.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qeh.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sah.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zbf.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://swx.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nct.fzhhl.top

[B04] for 计数循环
来源：http://pqs.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://omz.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qlm.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vvl.chenlongwang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nzf.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eyn.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pfx.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://vca.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zvr.cheryme.top

[B05] 遍历数组 / 列表
来源：http://xqe.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://jlg.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rxu.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://ytj.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://doi.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tmi.bbcook.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zik.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://cek.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oqw.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://sjx.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gjf.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fsg.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qii.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ipx.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hni.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zgg.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lzy.yueranfly.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sgk.zhoulong.xyz

[B07] while 循环
来源：http://npr.yj202588.top

Py:   while i < 10: i += 1
来源：http://mqs.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://vzb.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://wvl.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://sdy.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://bez.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ewt.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://knj.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://kge.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://qqr.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://bgt.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://ryg.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://fty.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://eog.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://ibt.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qmd.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://utm.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://apm.cdnleiting.top

[B09] break 与 continue
来源：http://yot.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lym.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qff.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ena.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kmr.cqqwz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jfg.xingfuxueyuan.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jze.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://urb.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rci.fzhhl.top

[B10] 遍历同时拿索引
来源：http://nfs.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ify.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://feo.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxt.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mwu.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jzo.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ldl.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xjn.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ydx.hesvh.cn

[B11] 生成数字序列 / 区间
来源：http://prt.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://vfy.hammf.cn

PHP:  range(0, 10, 2);
来源：http://pvr.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mix.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gts.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wrl.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opy.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://tdx.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uvy.yueranfly.top

[B12] 跳出多层循环
来源：http://nlk.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ond.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ncp.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nzi.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kzf.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://txw.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://trq.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ttq.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vfl.yangfankeji.com

[B13] 判断是否为数字
来源：http://rfx.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://enx.cqqwz.cn

PHP:  is_numeric($x)
来源：http://emg.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nee.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqo.yj20258888.top

Java: x instanceof Number
来源：http://ofw.pengpengdd.cyou

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vus.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://qgj.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://umh.iojbl.cn

[B14] 判断值是否在集合内
来源：http://ncu.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fvb.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fyw.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ebt.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://nkr.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cie.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bpt.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://qav.andypj.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bur.shzxlz.cn

[B15] 布尔运算与取反
来源：http://wch.jinghuilouyu.cn

Py:   a and b or not c
来源：http://cov.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://oeq.shangyingyoupin.top

JS:   a && b || !c
来源：http://bcl.havefunace.top

TS:   a && b || !c
来源：http://tvl.yongpay.top

Java: a && b || !c
来源：http://vtw.xylfe.cn

Go:   a && b || !c
来源：http://hou.yanxiufei.cn

Ruby: a && b || !c
来源：http://wpy.cdnleiting.top

C#:   a && b || !c
来源：http://gsq.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://jbp.chenlongwang.top

Py:   if not data: return
来源：http://mkw.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://qhn.vqdsnc.cn

JS:   if (!data) return;
来源：http://rzs.birdmap.top

TS:   if (!data) return;
来源：http://wzm.gaohongyu789.top

Java: if (data == null) return;
来源：http://qon.hfpthk.cn

Go:   if data == nil { return }
来源：http://lhz.smart0.xyz

Ruby: return if data.nil?
来源：http://mxz.hywenlv.cn

C#:   if (data == null) return;
来源：http://bos.52xcode.cn

================================================================================
来源：http://zsa.bjfxy.top

C. 函数与作用域
来源：http://ezn.yuxming.cn

================================================================================
来源：http://jjb.yj202588.top

[C01] 定义函数
来源：http://shg.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://lyr.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cfz.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://myr.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ecb.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yas.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zpw.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://vnu.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kcn.haohaochexian.top

[C02] 默认参数
来源：http://imr.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://len.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gqk.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://kkw.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ibm.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xkx.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://euo.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://odb.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://okh.zhoulong.xyz

[C03] 可变参数
来源：http://pja.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://xvg.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://niz.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mwo.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zbs.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://muj.fehbvm.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jgu.shanyushiyangtech.top


<!-- 参考信息 -->