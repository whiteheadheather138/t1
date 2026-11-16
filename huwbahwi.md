代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pfa.tanke756.top

JS:   `Hello, ${name}!`
来源：http://hiv.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://dfh.hcnkem.com

Java: "Hello, %s!".formatted(name)
来源：http://vfg.xingfuxueyuan.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fad.hnqzz.top

Ruby: "Hello, #{name}!"
来源：http://dss.pycfn.com

C#:   $"Hello, {name}!"
来源：http://ttc.wangdashe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rnv.yj202588.top

Py:   "第一行\n第二行"
来源：http://nza.zhijiandao.cn

PHP:  "第一行\n第二行"
来源：http://qtc.zhaomingkeji.xyz

JS:   "第一行\n第二行"
来源：http://fod.fzhhl.top

TS:   "第一行\n第二行"
来源：http://nkq.yueranfly.top

Java: "第一行\n第二行"
来源：http://skh.haohaochexian.top

Go:   "第一行\n第二行"
来源：http://wil.pengpengdd.cyou

Ruby: "第一行\n第二行"
来源：http://pey.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://lyy.chenzaomai.com

[A14] 注释写法
来源：http://qlx.guannengcc.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mdc.vqdsnc.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://coj.fengsongda.top

JS:   // 单行；/* 多行 */
来源：http://knz.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://lii.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xlu.hammf.cn

Go:   // 单行；/* 多行 */
来源：http://saq.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vff.uphjek.com

C#:   // 单行；/* 多行 */
来源：http://xii.chenlongwang.top

[A15] 空值判断与默认值
来源：http://hot.fanxiaobao.xyz

Py:   value = data or "默认值"
来源：http://kwb.yanxiufei.cn

PHP:  $value = $data ?? "默认值";
来源：http://nqv.xuanzx.com

JS:   const value = data ?? "默认值";
来源：http://snc.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://cgg.hongshengwenyu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gns.ybcxt.top

Go:   if data == "" { data = "默认值" }
来源：http://ruw.yuanzhike.top

Ruby: value = data || "默认值"
来源：http://gsg.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://kxg.ppjwa.cn

[A16] 真假值判断规则
来源：http://vtx.fzhhl.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fcs.jinghuilouyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ykb.shzxlz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pth.hnxiangtu.top

TS:   if (!x) {}
来源：http://cgn.sysykeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oez.yanxiufei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eul.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://xhu.yonumen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pqu.yuxming.cn

[A17] 位运算
来源：http://ffc.xziqi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blc.quarkkingdee.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gle.wangshuangyany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pih.tarul.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rpb.fanxiaobao.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://isa.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ipg.guannengcc.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ctt.fehbvm.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cxu.sjlbkw.cn

[A18] 字符与 ASCII 码互转
来源：http://rbg.chenlongwang.top

Py:   ord("A"); chr(65)
来源：http://kmz.yj202588.top

PHP:  ord("A"); chr(65)
来源：http://yeh.ppjwa.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qzo.gogol.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://opb.dashuyun.cn

Java: (int) 'A'; (char) 65
来源：http://jry.zdbjq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xsf.hesvh.cn

Ruby: "A".ord; 65.chr
来源：http://ajc.bbcook.cn

C#:   (int)'A'; (char)65
来源：http://bji.dianchejie.cn

[A19] 交换两个变量
来源：http://men.0kj1m.cn

Py:   a, b = b, a
来源：http://wtr.zdbjq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rxl.vehdjk.com

JS:   [a, b] = [b, a];
来源：http://dsi.andypj.xyz

TS:   [a, b] = [b, a];
来源：http://dlq.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://kvq.xylfe.cn

Go:   a, b = b, a
来源：http://zma.zhoulong.xyz

Ruby: a, b = b, a
来源：http://tmv.zhixingplan.top

C#:   (a, b) = (b, a);
来源：http://uqt.sweek.top

[A20] 读取标准输入
来源：http://ghb.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://dvc.zhiwuduotai.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xgu.ivvv.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nwd.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://erx.ctjpmb.com

Java: new Scanner(System.in).nextLine()
来源：http://bai.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gno.pengpengdd.cyou

Ruby: gets.chomp
来源：http://fpf.ehwqpu.com

C#:   Console.ReadLine();
来源：http://eqo.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://pvx.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://kih.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pwe.316326.xyz

JS:   (3.14159).toFixed(2)
来源：http://grn.feifeiyinyue.top

TS:   (3.14159).toFixed(2)
来源：http://lqv.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://nax.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qvm.fengsongda.top

Ruby: format("%.2f", 3.14159)
来源：http://fef.haohaochexian.top

C#:   3.14159.ToString("F2")
来源：http://gjt.birdmap.top

[A22] 获取字符串长度
来源：http://quq.ehwqpu.com

Py:   len(s)
来源：http://pmf.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://slq.jinghuilouyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gir.vqdsnc.cn

TS:   s.length
来源：http://pjj.pycfn.com

Java: s.length()
来源：http://nxl.zhoulong.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://owv.xziqi.cn

Ruby: s.length
来源：http://mgu.hammf.cn

C#:   s.Length
来源：http://ccs.vehdjk.com

[A23] 大小写转换
来源：http://zft.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uxo.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vvk.cucudq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fpf.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rjc.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://elb.haohaochexian.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iik.yuanzhike.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jsr.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://euk.dianchejie.cn

[A24] 去除首尾空白
来源：http://yjf.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nkd.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sxy.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xgo.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jmc.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lfb.cqqwz.cn

Go:   strings.TrimSpace(s)
来源：http://zjf.xziqi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cox.cashguo.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aoo.yj202588.top

[A25] 字符串比较
来源：http://xck.jianghu66.top

Py:   s1 == s2; s1 != s2
来源：http://sdh.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wlx.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bxd.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jfv.yongpay.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gir.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rvm.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xht.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://peb.gotoacloud.top

[A26] 类型转换总览
来源：http://wbx.andypj.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gki.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tln.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gar.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://yyp.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://czh.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://szg.jyoumei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yvs.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://obt.sweek.top

================================================================================
来源：http://wdr.yonumen.top

B. 流程控制
来源：http://uji.c1oappe.top

================================================================================
来源：http://wde.xziqi.cn

[B01] 条件判断 if / else
来源：http://bmf.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rrw.ydjk.org.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ehc.c1oappe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://unv.gzhubu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rta.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rzi.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ueq.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lyb.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gjr.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://nku.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rpb.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fss.daria6918.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://azp.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwp.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dhr.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pyk.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ute.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zow.yvedp.cn

[B03] switch / match / case
来源：http://vlr.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cqb.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ipj.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qyu.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uox.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://elp.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dze.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cfg.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vli.wangdashe.top

[B04] for 计数循环
来源：http://pan.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://nhl.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://usd.zdbjq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://idf.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kix.epnwcf.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yzj.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gkj.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://kfq.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kht.guannengcc.top

[B05] 遍历数组 / 列表
来源：http://pij.hywenlv.cn

Py:   for item in arr: print(item)
来源：http://ofp.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qzr.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qtv.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nap.hammf.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aax.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vdj.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://eqo.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://unn.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://wug.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mlv.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uxd.ydjk.org.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jdo.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zoe.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tyg.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ihr.hfpthk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ozp.zhongyouzk.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kzf.hesvh.cn

[B07] while 循环
来源：http://mal.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://kzf.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mze.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://zhp.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://zjk.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://qtp.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vfo.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://chs.bjfxy.top

C#:   while (i < 10) { i++; }
来源：http://sxq.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://obo.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://nhq.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uub.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://uyh.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://swi.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://pgd.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://pqa.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://zpu.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://spw.xuetiantiany.cn

[B09] break 与 continue
来源：http://mjw.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nbx.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tej.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gje.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ygi.hongshengwenyu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qkj.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://avt.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qio.jinyuanbaomall.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cky.nanxuanxn.top

[B10] 遍历同时拿索引
来源：http://cnk.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://smd.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bsa.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://frg.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wpi.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sec.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gup.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tmz.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qur.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://zjp.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://eed.yj202588.top

PHP:  range(0, 10, 2);
来源：http://nki.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rdy.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kmr.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ult.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fey.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://scp.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jas.guannengcc.top

[B12] 跳出多层循环
来源：http://fbx.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ris.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hzy.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pct.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yky.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://laq.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jmm.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hua.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ymx.tarul.cn

[B13] 判断是否为数字
来源：http://fgb.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://wmf.sweek.top

PHP:  is_numeric($x)
来源：http://tgp.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wet.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hnn.jianghu66.top

Java: x instanceof Number
来源：http://zcx.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qwc.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://fdw.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://yhq.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://dkg.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://afj.birdmap.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nuy.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://tia.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://ocb.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://saq.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vyi.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ikl.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://erc.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://ebd.pycfn.com

Py:   a and b or not c
来源：http://slf.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://smy.wangdashe.top

JS:   a && b || !c
来源：http://yir.jinghuilouyu.cn

TS:   a && b || !c
来源：http://uyz.quarkkingdee.top

Java: a && b || !c
来源：http://kvr.quarkkingdee.top

Go:   a && b || !c
来源：http://chm.chenlongwang.top

Ruby: a && b || !c
来源：http://ail.nanxinkj.top

C#:   a && b || !c
来源：http://kuy.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://pee.hongshengwenyu.top

Py:   if not data: return
来源：http://zqz.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://ckv.feifeiyinyue.top

JS:   if (!data) return;
来源：http://fhr.shangyingyoupin.top

TS:   if (!data) return;
来源：http://zme.daxiang520.top

Java: if (data == null) return;
来源：http://org.quarkkingdee.top

Go:   if data == nil { return }
来源：http://ujy.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://pnm.ppjwa.cn

C#:   if (data == null) return;
来源：http://jeg.pengpengdd.cyou

================================================================================
来源：http://xsf.haohaochexian.top

C. 函数与作用域
来源：http://vdh.kuanghao11.cn

================================================================================
来源：http://skt.52xcode.cn

[C01] 定义函数
来源：http://qrp.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://htk.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yyw.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://evw.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gqb.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pap.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://xfx.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://sbg.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bpq.zhaomingkeji.xyz

[C02] 默认参数
来源：http://qyo.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://tgf.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://zst.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://cjn.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hwi.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ikn.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nhl.gotoacloud.top

Ruby: def greet(name = "World") = name
来源：http://lsl.birdmap.top


<!-- 参考信息 -->