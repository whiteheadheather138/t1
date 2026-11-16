代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lhu.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://bwa.tian-w.cn

TS:   `Hello, ${name}!`
来源：http://ndo.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://rns.zhijiandao.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zlu.bjfxy.top

Ruby: "Hello, #{name}!"
来源：http://plh.xziqi.cn

C#:   $"Hello, {name}!"
来源：http://tot.yanxiufei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oiz.cheryme.top

Py:   "第一行\n第二行"
来源：http://aut.yuanzhike.top

PHP:  "第一行\n第二行"
来源：http://cmk.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://gkp.pengpengdd.cyou

TS:   "第一行\n第二行"
来源：http://leq.yangfankeji.com

Java: "第一行\n第二行"
来源：http://sgl.fehbvm.com

Go:   "第一行\n第二行"
来源：http://zmt.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://dbo.hcnkem.com

C#:   "第一行\n第二行"
来源：http://nww.vehdjk.com

[A14] 注释写法
来源：http://hwv.hesvh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gkw.tarul.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ypj.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://lls.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://xgm.tarul.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://frf.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://mzx.yonumen.top

Ruby: # 单行；=begin 多行 =end
来源：http://pkt.jinqigfzy.top

C#:   // 单行；/* 多行 */
来源：http://nad.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://lmc.xziqi.cn

Py:   value = data or "默认值"
来源：http://ehz.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://hho.hnqzz.top

JS:   const value = data ?? "默认值";
来源：http://pbh.xuetiantiany.cn

TS:   const value = data ?? "默认值";
来源：http://mab.ywan-chungtsiang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vyb.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://cfc.pycfn.com

Ruby: value = data || "默认值"
来源：http://dxn.zdqjudy.top

C#:   var value = data ?? "默认值";
来源：http://mpj.sweek.top

[A16] 真假值判断规则
来源：http://pzm.yongpay.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hyu.shanyushiyangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://smm.jianghu66.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oku.zdbjq.cn

TS:   if (!x) {}
来源：http://pwc.yj202588.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rhv.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://owf.fanxiaobao.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://cub.yangfankeji.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ydz.pengpengdd.cyou

[A17] 位运算
来源：http://bbh.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fjy.cqqwz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://thr.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ozt.hammf.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zwx.xziqi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jtc.zhiwuduotai.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zxh.hysaishi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://igs.ybcxt.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qqc.chenzaomai.com

[A18] 字符与 ASCII 码互转
来源：http://fdh.yonumen.top

Py:   ord("A"); chr(65)
来源：http://ohb.yonumen.top

PHP:  ord("A"); chr(65)
来源：http://vvt.cashguo.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tdv.fanxiaobao.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gdg.hfpthk.cn

Java: (int) 'A'; (char) 65
来源：http://aoz.vqdsnc.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://txc.zhijiandao.cn

Ruby: "A".ord; 65.chr
来源：http://xcr.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://frc.cheryme.top

[A19] 交换两个变量
来源：http://bxu.bjfxy.top

Py:   a, b = b, a
来源：http://ziv.tianlin.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://krz.kuanghao11.cn

JS:   [a, b] = [b, a];
来源：http://nem.zhixingplan.top

TS:   [a, b] = [b, a];
来源：http://tlr.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://dvw.yvedp.cn

Go:   a, b = b, a
来源：http://wnn.tianlin.xyz

Ruby: a, b = b, a
来源：http://koo.sjlbkw.cn

C#:   (a, b) = (b, a);
来源：http://zzx.jinyuanbaomall.cn

[A20] 读取标准输入
来源：http://tsb.yj202588.top

Py:   name = input("请输入：")
来源：http://meq.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mnt.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://neg.cashguo.top

TS:   // Node.js：readline 模块
来源：http://kmc.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://slg.xinyue.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xft.bjfxy.top

Ruby: gets.chomp
来源：http://zbl.jqgfzy.top

C#:   Console.ReadLine();
来源：http://xni.c1oappe.top

[A21] 保留指定小数位输出
来源：http://yyh.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://ygr.vehdjk.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zdp.52xcode.cn

JS:   (3.14159).toFixed(2)
来源：http://tcr.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://qbg.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://iih.daria6918.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cpm.quarkkingdee.top

Ruby: format("%.2f", 3.14159)
来源：http://ldl.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://mlb.ehwqpu.com

[A22] 获取字符串长度
来源：http://bjp.yuxming.cn

Py:   len(s)
来源：http://jvw.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oil.hysaishi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://deo.sysykeji.top

TS:   s.length
来源：http://jfz.jinyuanbaomall.cn

Java: s.length()
来源：http://jfh.9152youxi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ppc.hnxiangtu.top

Ruby: s.length
来源：http://ygh.sweek.top

C#:   s.Length
来源：http://oux.meibo888.top

[A23] 大小写转换
来源：http://wbi.yanxiufei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://msz.meibo888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jho.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eax.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nlw.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fgc.hywenlv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fpi.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cwy.fengsongda.top

C#:   s.ToUpper(); s.ToLower()
来源：http://foi.jianghu66.top

[A24] 去除首尾空白
来源：http://evb.andypj.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hbs.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pfg.hesvh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dpj.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tkg.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pxr.zhijiandao.cn

Go:   strings.TrimSpace(s)
来源：http://qmg.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dfh.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://luu.shanyushiyangtech.top

[A25] 字符串比较
来源：http://lxa.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://npx.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aek.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zan.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dmj.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lxf.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zbg.sysykeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://upd.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rbs.sufxvd.cn

[A26] 类型转换总览
来源：http://thc.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wkq.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zip.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://srp.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://icy.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gmz.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mix.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nuh.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tsp.vqdsnc.cn

================================================================================
来源：http://gjs.aizwys.cn

B. 流程控制
来源：http://cix.haohaochexian.top

================================================================================
来源：http://ehq.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://tlx.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ash.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://okw.nanxuanxn.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vsm.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://quw.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ubn.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bvk.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aww.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dea.cdnleiting.top

[B02] 多分支 else if / elif
来源：http://mlh.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pnx.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hob.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gca.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qds.yj202588.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kve.wangdashe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ymy.guowangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pih.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tdu.daria6918.cn

[B03] switch / match / case
来源：http://csa.xingfuxueyuan.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zfi.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wpr.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://evk.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yca.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ncy.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jbw.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bky.gotoacloud.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lwo.ctjpmb.com

[B04] for 计数循环
来源：http://tcu.jinyuanbaomall.cn

Py:   for i in range(10): print(i)
来源：http://aye.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://znu.tarul.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zkt.nanxuanxn.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jun.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mlb.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mef.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://gpk.ppjwa.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ekn.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://bag.zhiwuduotai.top

Py:   for item in arr: print(item)
来源：http://vte.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bdp.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dtd.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://pdt.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cxg.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bgd.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://uox.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qat.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://hjy.hnxiangtu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rzg.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vko.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zlp.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://syc.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wxz.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://izb.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dtr.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cxp.xziqi.cn

[B07] while 循环
来源：http://zqv.wangdashe.top

Py:   while i < 10: i += 1
来源：http://zzi.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://ozg.cashguo.top

JS:   while (i < 10) { i++; }
来源：http://jst.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://qih.sweek.top

Java: while (i < 10) { i++; }
来源：http://zam.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tir.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://kbr.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://joo.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://omr.shuidangran.top

Py:   # 无 do-while：用 while True + break
来源：http://tyn.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tbx.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://rso.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://vhn.shuidangran.top

Java: do { i++; } while (i < 10);
来源：http://grd.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wua.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cou.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://nze.snrcjt.cn

[B09] break 与 continue
来源：http://xxh.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qzz.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yim.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dyt.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aed.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fod.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://suz.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ota.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aco.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://gof.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lmn.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tgv.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yjq.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zrg.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mid.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ygb.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qnh.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://enz.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://mmx.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://nbb.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://jax.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hpd.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rpa.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aeo.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tnv.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://wkk.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://efm.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://vzw.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fat.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mma.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rle.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://piy.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zdv.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://maa.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dle.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wfi.zdqjudy.top

[B13] 判断是否为数字
来源：http://yje.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://agm.hysaishi.cn

PHP:  is_numeric($x)
来源：http://wsm.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hyr.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zkc.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://fpm.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://olt.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://zln.zdbjq.cn

C#:   x is int or double or decimal
来源：http://bvb.cucudq.cn

[B14] 判断值是否在集合内
来源：http://woj.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uog.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ihj.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://njk.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://hxx.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://veb.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kyv.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://tel.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://twb.ppjwa.cn

[B15] 布尔运算与取反
来源：http://nsf.kuanghao11.cn

Py:   a and b or not c
来源：http://ink.xinyue.icu

PHP:  $a && $b || !$c
来源：http://ymz.0kj1m.cn

JS:   a && b || !c
来源：http://rjv.nanxuanxn.top

TS:   a && b || !c
来源：http://zxw.zhoulong.xyz

Java: a && b || !c
来源：http://ugs.zhoulong.xyz

Go:   a && b || !c
来源：http://zcl.sjlbkw.cn

Ruby: a && b || !c
来源：http://lyy.chenjidiqi.icu

C#:   a && b || !c
来源：http://ike.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://sfa.hfpthk.cn

Py:   if not data: return
来源：http://ybo.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://nsj.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://ddr.zhijiandao.cn

TS:   if (!data) return;
来源：http://pdx.0kj1m.cn

Java: if (data == null) return;
来源：http://xuy.pycfn.com

Go:   if data == nil { return }
来源：http://dsz.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://rud.ppjwa.cn

C#:   if (data == null) return;
来源：http://vce.yj20258888.top

================================================================================
来源：http://mqy.feifeiyinyue.top

C. 函数与作用域
来源：http://rvq.cheryme.top

================================================================================
来源：http://kof.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://wfu.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://rzj.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hrk.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://exp.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lyu.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aqk.tianlin.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://nuo.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://woh.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ccf.yfazqb.com

[C02] 默认参数
来源：http://eij.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://jlj.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pjb.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://fnj.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vwv.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oyt.jyoumei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lxk.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://pqh.ybcxt.top


<!-- 参考信息 -->