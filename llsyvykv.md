代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gut.9152youxi.cn

Ruby: "Hello, #{name}!"
来源：http://nzh.hfpthk.cn

C#:   $"Hello, {name}!"
来源：http://isc.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://snv.ydjk.org.cn

Py:   "第一行\n第二行"
来源：http://cbd.c1oappe.top

PHP:  "第一行\n第二行"
来源：http://dsu.redwolf501.top

JS:   "第一行\n第二行"
来源：http://rsd.yj202588.top

TS:   "第一行\n第二行"
来源：http://nxq.sjlbkw.cn

Java: "第一行\n第二行"
来源：http://nlb.svipenyu.cn

Go:   "第一行\n第二行"
来源：http://mqv.kuanghao11.cn

Ruby: "第一行\n第二行"
来源：http://rti.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://tuu.yangfankeji.com

[A14] 注释写法
来源：http://bzu.hammf.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xeq.tarul.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tqu.zhoulong.xyz

JS:   // 单行；/* 多行 */
来源：http://ijw.cucudq.cn

TS:   // 单行；/* 多行 */
来源：http://ekb.xylfe.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qno.9152youxi.cn

Go:   // 单行；/* 多行 */
来源：http://bdn.zycfv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jdh.yj202588.top

C#:   // 单行；/* 多行 */
来源：http://ede.shuidangran.top

[A15] 空值判断与默认值
来源：http://xin.wangdashe.top

Py:   value = data or "默认值"
来源：http://qsn.sjlbkw.cn

PHP:  $value = $data ?? "默认值";
来源：http://bje.ybcxt.top

JS:   const value = data ?? "默认值";
来源：http://cky.fengsongda.top

TS:   const value = data ?? "默认值";
来源：http://pzu.uphjek.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ajq.xziqi.cn

Go:   if data == "" { data = "默认值" }
来源：http://cfz.yj20258888.top

Ruby: value = data || "默认值"
来源：http://uhf.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://qaj.pycfn.com

[A16] 真假值判断规则
来源：http://ymt.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jik.feifeiyinyue.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qyp.sxryk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zge.snrcjt.cn

TS:   if (!x) {}
来源：http://aui.zhoulong.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lvz.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hxg.guowangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://ebc.xinyue.icu

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ghc.52xcode.cn

[A17] 位运算
来源：http://wve.haohaochexian.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqb.wangdashe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cwa.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xla.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nyk.hongshengwenyu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fsg.redwolf501.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wjs.xziqi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yet.sufxvd.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zva.yangfankeji.com

[A18] 字符与 ASCII 码互转
来源：http://zsv.chenjidiqi.icu

Py:   ord("A"); chr(65)
来源：http://ltl.gotoacloud.top

PHP:  ord("A"); chr(65)
来源：http://ojh.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pzc.shanyushiyangtech.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ajf.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://sll.aibaodan.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kef.yfazqb.com

Ruby: "A".ord; 65.chr
来源：http://pdj.shanyushiyangtech.top

C#:   (int)'A'; (char)65
来源：http://rla.nanxuanxn.top

[A19] 交换两个变量
来源：http://psi.vehdjk.com

Py:   a, b = b, a
来源：http://che.fanxiaobao.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://ngg.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://wlt.zhijiandao.cn

TS:   [a, b] = [b, a];
来源：http://ioc.fengsongda.top

Java: int t = a; a = b; b = t;
来源：http://ity.vqdsnc.cn

Go:   a, b = b, a
来源：http://qdd.316326.xyz

Ruby: a, b = b, a
来源：http://ldy.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://hqy.xuanzx.com

[A20] 读取标准输入
来源：http://ank.cdnleiting.top

Py:   name = input("请输入：")
来源：http://snz.jqgfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://cyd.xylfe.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ouq.hammf.cn

TS:   // Node.js：readline 模块
来源：http://tcb.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://rat.redwolf501.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mcn.jlsjyb.cn

Ruby: gets.chomp
来源：http://kqh.ydzc1.top

C#:   Console.ReadLine();
来源：http://nqz.zhiwuduotai.top

[A21] 保留指定小数位输出
来源：http://hmc.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://vvh.yongpay.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cpd.gzhubu.top

JS:   (3.14159).toFixed(2)
来源：http://lby.feifeiyinyue.top

TS:   (3.14159).toFixed(2)
来源：http://xwj.xylfe.cn

Java: String.format("%.2f", 3.14159)
来源：http://ctg.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ltx.cdnleiting.top

Ruby: format("%.2f", 3.14159)
来源：http://ili.9152youxi.cn

C#:   3.14159.ToString("F2")
来源：http://afk.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://enz.jinqigufen.top

Py:   len(s)
来源：http://jzv.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://izo.aibaodan.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vvz.yongpay.top

TS:   s.length
来源：http://ccu.yj202588.top

Java: s.length()
来源：http://ifx.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rfr.cucudq.cn

Ruby: s.length
来源：http://qcd.ybcxt.top

C#:   s.Length
来源：http://qmx.redwolf501.top

[A23] 大小写转换
来源：http://pye.gotoacloud.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mmr.jinyuanbaomall.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://msx.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fjl.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hpm.jinqigufen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sdc.daria6918.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ddn.meibo888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nnx.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ezp.meibo888.top

[A24] 去除首尾空白
来源：http://yyk.haohaochexian.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wrv.fengsongda.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dsx.aibaodan.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kqv.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sgk.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zef.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://fji.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yck.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cgv.hnqzz.top

[A25] 字符串比较
来源：http://wfp.zhijiandao.cn

Py:   s1 == s2; s1 != s2
来源：http://tie.yonumen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aov.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://klu.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pya.shuidangran.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mwa.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fag.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fri.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://joh.zhixingplan.top

[A26] 类型转换总览
来源：http://nts.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gdj.fktsv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wtd.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tef.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://uyk.birdmap.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uyv.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wiq.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ocj.sjlbkw.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zcw.jinyuanbaomall.cn

================================================================================
来源：http://ptg.tianlin.xyz

B. 流程控制
来源：http://kam.xinyue.icu

================================================================================
来源：http://ypl.epnwcf.com

[B01] 条件判断 if / else
来源：http://qpz.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://owl.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eae.sufxvd.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ecd.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pnp.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://efm.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wzd.zycfv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ayk.cdnleiting.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://erk.yj202588.top

[B02] 多分支 else if / elif
来源：http://uhy.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mpk.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://omv.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wha.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zkx.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ler.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tyo.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://poe.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxe.yuxming.cn

[B03] switch / match / case
来源：http://awb.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kxm.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qrc.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hxg.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ihk.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vhz.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ntu.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uuz.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sbu.fzhhl.top

[B04] for 计数循环
来源：http://byh.xylfe.cn

Py:   for i in range(10): print(i)
来源：http://eli.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xcl.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hph.zhoulong.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iit.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nvp.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eiq.kuanghao11.cn

Ruby: 10.times { |i| puts i }
来源：http://wkg.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qab.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://ffp.52xcode.cn

Py:   for item in arr: print(item)
来源：http://uij.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pfv.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dzy.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yyv.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jjs.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mzg.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://bkz.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nyt.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://wjp.hnxiangtu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://med.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qqz.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yya.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oaw.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mqc.ehwqpu.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://frr.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ybw.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xkg.sweek.top

[B07] while 循环
来源：http://gug.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://hpu.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://bmc.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://ptg.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://ksn.yuanzhike.top

Java: while (i < 10) { i++; }
来源：http://ybx.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gce.ydjk.org.cn

Ruby: while i < 10; i += 1; end
来源：http://mqm.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://qlu.uphjek.com

[B08] do-while（至少执行一次）
来源：http://omr.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://ock.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://exx.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://toe.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://mou.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://lmd.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jvt.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ekh.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://jmz.ivvv.top

[B09] break 与 continue
来源：http://ivz.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bwh.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://snl.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nha.xinyue.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxs.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nsm.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nqg.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yeo.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ztb.ybcxt.top

[B10] 遍历同时拿索引
来源：http://lby.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://exh.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uzb.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fvs.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://smk.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dox.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://icj.pycfn.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iui.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uls.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://upa.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://huq.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://osn.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wph.chenjidiqi.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyd.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uum.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tet.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://pnc.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oom.aibaodan.cn

[B12] 跳出多层循环
来源：http://zoy.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wbe.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vro.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eqq.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hlf.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kih.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xne.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oos.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cfx.daxiang520.top

[B13] 判断是否为数字
来源：http://bpz.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://rto.hysaishi.cn

PHP:  is_numeric($x)
来源：http://vio.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://enl.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fmt.ppjwa.cn

Java: x instanceof Number
来源：http://vmq.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mio.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://wlg.0kj1m.cn

C#:   x is int or double or decimal
来源：http://wce.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://ysa.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qfg.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://itz.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://uto.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://pak.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://mkk.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oxh.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://scc.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eix.jianghu66.top

[B15] 布尔运算与取反
来源：http://ldm.hammf.cn

Py:   a and b or not c
来源：http://mjr.bbcook.cn

PHP:  $a && $b || !$c
来源：http://wsi.andypj.xyz

JS:   a && b || !c
来源：http://bpe.havefunace.top

TS:   a && b || !c
来源：http://wdn.hongshengwenyu.top

Java: a && b || !c
来源：http://lqz.daxiang520.top

Go:   a && b || !c
来源：http://yyw.9152youxi.cn

Ruby: a && b || !c
来源：http://gyr.epnwcf.com

C#:   a && b || !c
来源：http://ray.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cvb.wangshuangyany.cn

Py:   if not data: return
来源：http://urr.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://voy.zhiwuduotai.top

JS:   if (!data) return;
来源：http://wsb.hammf.cn

TS:   if (!data) return;
来源：http://dtn.tarul.cn

Java: if (data == null) return;
来源：http://gcv.vqdsnc.cn

Go:   if data == nil { return }
来源：http://hon.aibaodan.cn

Ruby: return if data.nil?
来源：http://yyg.ybcxt.top

C#:   if (data == null) return;
来源：http://vzz.shanyushiyangkeji.top

================================================================================
来源：http://uem.ivvv.top

C. 函数与作用域
来源：http://bfn.9152youxi.cn

================================================================================
来源：http://syj.chenjidiqi.icu

[C01] 定义函数
来源：http://mhz.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://med.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vks.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://jqx.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ynq.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zqb.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oax.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://cgg.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zri.ehwqpu.com

[C02] 默认参数
来源：http://rjh.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://int.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jln.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://blq.nwbrower.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fca.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bfy.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pug.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://yky.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://nen.hammf.cn

[C03] 可变参数
来源：http://dyo.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://nrk.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fvi.pycfn.com


<!-- 参考信息 -->