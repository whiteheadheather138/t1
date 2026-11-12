代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fch.yonumen.top

Ruby: "Hello, #{name}!"
来源：http://gqm.aizwys.cn

C#:   $"Hello, {name}!"
来源：http://xoy.ivvv.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dty.zhongyouzk.top

Py:   "第一行\n第二行"
来源：http://kso.nwbrower.top

PHP:  "第一行\n第二行"
来源：http://wsg.gaohongyu789.top

JS:   "第一行\n第二行"
来源：http://tmm.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://vqw.zhijiandao.cn

Java: "第一行\n第二行"
来源：http://fpy.ivvv.top

Go:   "第一行\n第二行"
来源：http://tjm.chenlongwang.top

Ruby: "第一行\n第二行"
来源：http://qld.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://vct.zhiwuduotai.top

[A14] 注释写法
来源：http://tuh.xuetiantiany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dwm.zhixingplan.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ewk.chenzaomai.com

JS:   // 单行；/* 多行 */
来源：http://inz.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://bcg.vehdjk.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ulu.cashguo.top

Go:   // 单行；/* 多行 */
来源：http://vzz.fzhhl.top

Ruby: # 单行；=begin 多行 =end
来源：http://wai.gogol.net.cn

C#:   // 单行；/* 多行 */
来源：http://act.0kj1m.cn

[A15] 空值判断与默认值
来源：http://wgd.9152youxi.cn

Py:   value = data or "默认值"
来源：http://loe.epnwcf.com

PHP:  $value = $data ?? "默认值";
来源：http://sku.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://yhk.cucudq.cn

TS:   const value = data ?? "默认值";
来源：http://szz.kuanghao11.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vom.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://raa.cashguo.top

Ruby: value = data || "默认值"
来源：http://nyr.shzxlz.cn

C#:   var value = data ?? "默认值";
来源：http://jrx.ctjpmb.com

[A16] 真假值判断规则
来源：http://oqa.ppjwa.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qke.jinqigfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://raw.andypj.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nsl.pengpengdd.cyou

TS:   if (!x) {}
来源：http://ikr.tian-w.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yfx.jqgfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dfr.ehwqpu.com

Ruby: unless x            # nil 与 false 为假
来源：http://gte.tian-w.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ndy.xylfe.cn

[A17] 位运算
来源：http://fzw.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mth.tanke756.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://puk.aibaodan.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://unb.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://men.tanke756.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://upq.jyoumei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ebe.sxryk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ymw.316326.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cni.sysykeji.top

[A18] 字符与 ASCII 码互转
来源：http://gzc.yuxming.cn

Py:   ord("A"); chr(65)
来源：http://ucq.kuanghao11.cn

PHP:  ord("A"); chr(65)
来源：http://csw.cashguo.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wab.hesvh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vqj.chenjidiqi.icu

Java: (int) 'A'; (char) 65
来源：http://nfu.daxiang520.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xig.jyoumei.cn

Ruby: "A".ord; 65.chr
来源：http://crp.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://lkc.svipenyu.cn

[A19] 交换两个变量
来源：http://eus.bjfxy.top

Py:   a, b = b, a
来源：http://jdo.cdnleiting.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mdn.ywan-chungtsiang.top

JS:   [a, b] = [b, a];
来源：http://xjk.guannengcc.top

TS:   [a, b] = [b, a];
来源：http://tyr.yfazqb.com

Java: int t = a; a = b; b = t;
来源：http://epe.chenjidiqi.icu

Go:   a, b = b, a
来源：http://zgj.pengpengdd.cyou

Ruby: a, b = b, a
来源：http://pui.yueranfly.top

C#:   (a, b) = (b, a);
来源：http://mhr.hywenlv.cn

[A20] 读取标准输入
来源：http://ylq.feifeiyinyue.top

Py:   name = input("请输入：")
来源：http://huq.vqdsnc.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cyg.fanxiaobao.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nae.mhx1999.top

TS:   // Node.js：readline 模块
来源：http://glv.uphjek.com

Java: new Scanner(System.in).nextLine()
来源：http://lsq.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iib.jinqigfzy.top

Ruby: gets.chomp
来源：http://xur.cucudq.cn

C#:   Console.ReadLine();
来源：http://drx.sufxvd.cn

[A21] 保留指定小数位输出
来源：http://vbt.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://qum.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vtf.vehdjk.com

JS:   (3.14159).toFixed(2)
来源：http://pgv.nwbrower.top

TS:   (3.14159).toFixed(2)
来源：http://zkv.vqdsnc.cn

Java: String.format("%.2f", 3.14159)
来源：http://mlu.yueranfly.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kwu.ybcxt.top

Ruby: format("%.2f", 3.14159)
来源：http://pua.zycfv.cn

C#:   3.14159.ToString("F2")
来源：http://efd.dashuyun.cn

[A22] 获取字符串长度
来源：http://lcy.epnwcf.com

Py:   len(s)
来源：http://ypc.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ecs.snrcjt.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wuf.shanyushiyangtech.top

TS:   s.length
来源：http://dwe.ywan-chungtsiang.top

Java: s.length()
来源：http://wit.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://juc.cucudq.cn

Ruby: s.length
来源：http://ezv.quarkkingdee.top

C#:   s.Length
来源：http://ukk.jinqigufen.top

[A23] 大小写转换
来源：http://lsx.dashuyun.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://osv.gaohongyu789.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hna.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ztm.xuanzx.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jzc.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ufd.haohaochexian.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dta.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sxl.guowangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://koi.hammf.cn

[A24] 去除首尾空白
来源：http://yvj.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nlb.xuanzx.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dvl.jqgufenzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qsq.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ixs.shangyingyoupin.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pst.yj20258888.top

Go:   strings.TrimSpace(s)
来源：http://dze.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fcl.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mgk.zhoulong.xyz

[A25] 字符串比较
来源：http://yoi.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://cim.hywenlv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hjp.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ihk.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wax.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nyi.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zzo.yuanzhike.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xne.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lkl.xziqi.cn

[A26] 类型转换总览
来源：http://ahb.gogol.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://adp.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kxa.nwbrower.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pmm.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://gee.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fjg.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eae.hnqzz.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fdl.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vzx.shanyushiyangkeji.top

================================================================================
来源：http://rjm.mhx1999.top

B. 流程控制
来源：http://dyy.9152youxi.cn

================================================================================
来源：http://ngi.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://cip.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://deq.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lih.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qlw.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qvq.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://aac.redwolf501.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://unz.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ulk.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zvx.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://amo.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xor.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qwc.daxiang520.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hsl.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://drm.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mjo.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yao.sweek.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iwl.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bqi.guannengcc.top

[B03] switch / match / case
来源：http://qxn.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vsj.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iln.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cmf.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tio.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gsc.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gps.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://orj.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dmp.kuanghao11.cn

[B04] for 计数循环
来源：http://ceg.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://tip.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://igw.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ufw.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zzl.zdbjq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aen.zhixingplan.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rob.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://uig.xylfe.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wno.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://wai.sweek.top

Py:   for item in arr: print(item)
来源：http://ikq.jiagoushi.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tbu.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ujr.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fsc.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://oen.yvedp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bbd.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://kqk.yj20258.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pvf.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://asc.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uog.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qgq.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://geh.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tgz.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qye.0kj1m.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mmc.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ryg.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vft.jiagoushi.top

[B07] while 循环
来源：http://lbs.ivvv.top

Py:   while i < 10: i += 1
来源：http://yil.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zak.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://dxj.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://vqi.jianghu66.top

Java: while (i < 10) { i++; }
来源：http://hua.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aua.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://kah.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://aug.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://kly.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://igd.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xnw.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://ypo.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://nkm.yongpay.top

Java: do { i++; } while (i < 10);
来源：http://ggd.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://mzj.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uap.cdnleiting.top

C#:   do { i++; } while (i < 10);
来源：http://dpr.xziqi.cn

[B09] break 与 continue
来源：http://whf.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vrl.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dzi.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndj.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aol.guannengcc.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nlf.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yel.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wng.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bef.cucudq.cn

[B10] 遍历同时拿索引
来源：http://fsr.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dma.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mrw.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://roj.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ojm.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yfs.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mow.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fiy.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kyt.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://gsb.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://stq.yj202588.top

PHP:  range(0, 10, 2);
来源：http://sac.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sut.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://trm.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vlh.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xeb.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://ces.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mna.zdbjq.cn

[B12] 跳出多层循环
来源：http://wiz.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pev.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tvd.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zyd.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jgc.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fxx.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fso.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://row.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ckh.yueranfly.top

[B13] 判断是否为数字
来源：http://hrd.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://dlx.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://jxa.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uvn.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iuj.jiagoushi.top

Java: x instanceof Number
来源：http://fhq.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://agg.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://kme.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://zss.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://mvn.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ojr.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rqq.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://yot.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://jsv.yueranfly.top

Java: List.of(1, 2, 3).contains(x)
来源：http://myk.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lhl.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zzi.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ols.bbcook.cn

[B15] 布尔运算与取反
来源：http://vfm.epnwcf.com

Py:   a and b or not c
来源：http://dft.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://fdu.ivvv.top

JS:   a && b || !c
来源：http://wiq.sysykeji.top

TS:   a && b || !c
来源：http://xmg.nwbrower.top

Java: a && b || !c
来源：http://yxg.ctjpmb.com

Go:   a && b || !c
来源：http://gem.pycfn.com

Ruby: a && b || !c
来源：http://hoa.cucudq.cn

C#:   a && b || !c
来源：http://uym.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://njz.smart0.xyz

Py:   if not data: return
来源：http://wmh.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://blv.ehwqpu.com

JS:   if (!data) return;
来源：http://rlc.sjlbkw.cn

TS:   if (!data) return;
来源：http://dlo.aibaodan.cn

Java: if (data == null) return;
来源：http://xvy.jiagoushi.top

Go:   if data == nil { return }
来源：http://lfq.ydzc1.top

Ruby: return if data.nil?
来源：http://wgf.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://nel.sysykeji.top

================================================================================
来源：http://mqq.zhongyouzk.top

C. 函数与作用域
来源：http://xwe.gogol.net.cn

================================================================================
来源：http://hpb.fzhhl.top

[C01] 定义函数
来源：http://kdm.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://ylt.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sht.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://zyp.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://exk.kuanghao11.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wke.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hni.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://bei.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://til.zhengqikj.top

[C02] 默认参数
来源：http://gji.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://abm.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ruk.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://xmm.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://djy.yvedp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iei.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://moy.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://nvo.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://njg.ivvv.top

[C03] 可变参数
来源：http://tid.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://ltm.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rie.svipenyu.cn


<!-- 参考信息 -->