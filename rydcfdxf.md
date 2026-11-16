代发 wailian999

Ruby: value = data || "默认值"
来源：http://ooc.fanxiaobao.xyz

C#:   var value = data ?? "默认值";
来源：http://kbg.snrcjt.cn

[A16] 真假值判断规则
来源：http://mlb.sufxvd.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wks.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hma.kuanghao11.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fox.jiagoushi.top

TS:   if (!x) {}
来源：http://loj.gogol.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lej.hcnkem.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bdt.havefunace.top

Ruby: unless x            # nil 与 false 为假
来源：http://bqu.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zsw.yangfankeji.com

[A17] 位运算
来源：http://bri.pycfn.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lei.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://oen.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nvu.kuanghao11.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wlu.jianghu66.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mjm.sysykeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rqr.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://afs.hfpthk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zrj.fengsongda.top

[A18] 字符与 ASCII 码互转
来源：http://ppx.zhengqikj.top

Py:   ord("A"); chr(65)
来源：http://imw.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://ptw.ppjwa.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vbm.yonumen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nst.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://wlf.haohaochexian.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://owy.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://wft.shzxlz.cn

C#:   (int)'A'; (char)65
来源：http://zwo.iojbl.cn

[A19] 交换两个变量
来源：http://vyc.tanke756.top

Py:   a, b = b, a
来源：http://bun.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qyh.hcnkem.com

JS:   [a, b] = [b, a];
来源：http://nml.vqdsnc.cn

TS:   [a, b] = [b, a];
来源：http://klb.fehbvm.com

Java: int t = a; a = b; b = t;
来源：http://gma.jinghuilouyu.cn

Go:   a, b = b, a
来源：http://oac.hesvh.cn

Ruby: a, b = b, a
来源：http://yuo.c1oappe.top

C#:   (a, b) = (b, a);
来源：http://pqy.sufxvd.cn

[A20] 读取标准输入
来源：http://xmn.nwbrower.top

Py:   name = input("请输入：")
来源：http://eft.shangyingyoupin.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qjz.gzhubu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eju.chenlongwang.top

TS:   // Node.js：readline 模块
来源：http://cne.vehdjk.com

Java: new Scanner(System.in).nextLine()
来源：http://lox.tarul.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gvw.yanxiufei.cn

Ruby: gets.chomp
来源：http://woh.sjlbkw.cn

C#:   Console.ReadLine();
来源：http://dof.jianghu66.top

[A21] 保留指定小数位输出
来源：http://wpn.aizwys.cn

Py:   f"{3.14159:.2f}"
来源：http://rkt.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://btt.zhongyouzk.top

JS:   (3.14159).toFixed(2)
来源：http://yvk.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://mrz.vqdsnc.cn

Java: String.format("%.2f", 3.14159)
来源：http://inz.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gny.0kj1m.cn

Ruby: format("%.2f", 3.14159)
来源：http://yyf.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://dkr.smart0.xyz

[A22] 获取字符串长度
来源：http://vlo.xuanzx.com

Py:   len(s)
来源：http://udx.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://icd.yuxming.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kii.iojbl.cn

TS:   s.length
来源：http://tdk.xuetiantiany.cn

Java: s.length()
来源：http://jiu.nanxinkj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://khq.daxiang520.top

Ruby: s.length
来源：http://zzg.meibo888.top

C#:   s.Length
来源：http://cjb.meibo888.top

[A23] 大小写转换
来源：http://grs.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jty.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pmg.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tmc.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bpb.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vie.fanxiaobao.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lvl.fehbvm.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gbi.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gfj.chenzaomai.com

[A24] 去除首尾空白
来源：http://tnz.quarkkingdee.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fnp.wangdashe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://itm.ydzc1.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cjp.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vae.shanyushiyangtech.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kyc.snrcjt.cn

Go:   strings.TrimSpace(s)
来源：http://byn.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://udn.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xjc.sufxvd.cn

[A25] 字符串比较
来源：http://gqr.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://qhy.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://phy.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wgk.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sni.nanxinkj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bet.chenjidiqi.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tjn.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://hkr.aizwys.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aju.aizwys.cn

[A26] 类型转换总览
来源：http://hsa.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dgq.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zqh.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qpp.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://wfg.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gja.xuetiantiany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hhq.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bxe.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ret.nwbrower.top

================================================================================
来源：http://hpm.yueranfly.top

B. 流程控制
来源：http://vgb.fzhhl.top

================================================================================
来源：http://xwv.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://kuw.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://zyc.gogol.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hok.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wcm.zhixingplan.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dgm.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ygr.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://njn.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zug.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rxl.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://pld.wangshuangyany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iuv.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eff.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eud.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xll.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vit.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sqg.vqdsnc.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://afh.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://roh.smart0.xyz

[B03] switch / match / case
来源：http://bfv.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vki.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tiu.yj20258888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tte.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cms.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iye.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qtc.jinghuilouyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xgm.jqgfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dvh.yfazqb.com

[B04] for 计数循环
来源：http://men.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://ydx.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iyk.zdbjq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vjr.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qkl.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bzn.svipenyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mhd.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://jfi.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jcn.gotoacloud.top

[B05] 遍历数组 / 列表
来源：http://opq.fehbvm.com

Py:   for item in arr: print(item)
来源：http://akl.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fqh.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://esi.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://avo.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hdq.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dij.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://ttt.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://chr.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://ayf.yvedp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gvc.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uui.aibaodan.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jzp.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://loy.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ywe.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iak.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qxg.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jyo.wangdashe.top

[B07] while 循环
来源：http://ivu.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://cad.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://euz.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://ftp.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://ayq.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://eyt.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jcs.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://dgd.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://hyn.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://cca.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://oco.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kqc.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://dep.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://bgf.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://rnu.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://two.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://qfw.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://wyy.guowangkeji.top

[B09] break 与 continue
来源：http://wpc.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lxt.jinqigfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zkk.redwolf501.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rea.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hpx.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mvk.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tdb.sufxvd.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://syw.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eyp.mhx1999.top

[B10] 遍历同时拿索引
来源：http://wtf.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xqz.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rwv.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://egy.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://npq.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aab.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dln.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iit.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://psq.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://wvz.jqgufenzy.top

Py:   list(range(0, 10, 2))
来源：http://cme.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://jba.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oet.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gnp.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lwh.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ytb.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://ejz.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kcw.jqgfzy.top

[B12] 跳出多层循环
来源：http://vtl.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eyz.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://lwc.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ffu.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zqf.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ctx.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://owz.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zsc.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yrf.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://ryl.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://dmf.hfpthk.cn

PHP:  is_numeric($x)
来源：http://qca.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iue.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://abz.yvedp.cn

Java: x instanceof Number
来源：http://zij.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://evn.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://bet.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://vdm.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://tdh.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lkd.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gms.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://kpq.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://zin.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vpd.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://usp.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vmy.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://prf.aibaodan.cn

[B15] 布尔运算与取反
来源：http://zov.epnwcf.com

Py:   a and b or not c
来源：http://dkz.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://iyk.cucudq.cn

JS:   a && b || !c
来源：http://wxn.bbcook.cn

TS:   a && b || !c
来源：http://vjg.gzhubu.top

Java: a && b || !c
来源：http://ckp.ppjwa.cn

Go:   a && b || !c
来源：http://nti.9152youxi.cn

Ruby: a && b || !c
来源：http://hsb.fehbvm.com

C#:   a && b || !c
来源：http://oxl.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://itv.yj202588.top

Py:   if not data: return
来源：http://ekj.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://zkp.havefunace.top

JS:   if (!data) return;
来源：http://zdz.nanxuanxn.top

TS:   if (!data) return;
来源：http://upj.yueranfly.top

Java: if (data == null) return;
来源：http://obw.yonumen.top

Go:   if data == nil { return }
来源：http://yxe.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://fda.pycfn.com

C#:   if (data == null) return;
来源：http://dty.yj20258.top

================================================================================
来源：http://xmx.sysykeji.top

C. 函数与作用域
来源：http://rhe.ydzc1.top

================================================================================
来源：http://sav.hongshengwenyu.top

[C01] 定义函数
来源：http://moy.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://ngn.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nbn.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ric.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://icb.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kdw.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://rkg.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://gak.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bwz.aizwys.cn

[C02] 默认参数
来源：http://fpv.sweek.top

Py:   def greet(name="World"): return name
来源：http://imh.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gys.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://qum.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hgt.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rgv.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zed.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://djs.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://yxa.pengpengdd.cyou

[C03] 可变参数
来源：http://kfl.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://jbj.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hlp.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lpt.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rwj.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zej.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oly.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://lqc.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://agi.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://kak.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wtx.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xks.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ebz.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xzb.iojbl.cn

Java: // 无：用 Builder 模式或 record
来源：http://cbk.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://ock.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://met.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://glt.meibo888.top

[C05] 返回多个值
来源：http://gjw.fehbvm.com

Py:   return a, b
来源：http://crk.yangfankeji.com

PHP:  return [$a, $b];
来源：http://bwn.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aek.zycfv.cn

TS:   return { a, b };
来源：http://flm.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ufi.sysykeji.top

Go:   return a, b
来源：http://jqu.cheryme.top

Ruby: return a, b
来源：http://njp.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://qkx.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://ztg.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://dpy.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://iqq.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://zss.jinqigfzy.top


<!-- 参考信息 -->