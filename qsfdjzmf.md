代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ubx.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dve.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://buo.ywan-chungtsiang.top

[A17] 位运算
来源：http://izw.chenlongwang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kth.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kjq.cheryme.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wgl.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://haf.zhiwuduotai.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nqd.ppjwa.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bfq.bjfxy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yxm.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axv.tarul.cn

[A18] 字符与 ASCII 码互转
来源：http://ppu.ehwqpu.com

Py:   ord("A"); chr(65)
来源：http://nqu.xingfuxueyuan.xyz

PHP:  ord("A"); chr(65)
来源：http://hhe.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ngm.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bie.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://lhc.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vxg.shuidangran.top

Ruby: "A".ord; 65.chr
来源：http://acp.jqgfzy.top

C#:   (int)'A'; (char)65
来源：http://tip.fktsv.cn

[A19] 交换两个变量
来源：http://noh.ivvv.top

Py:   a, b = b, a
来源：http://bth.zhiwuduotai.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qrl.hnqzz.top

JS:   [a, b] = [b, a];
来源：http://fjt.pycfn.com

TS:   [a, b] = [b, a];
来源：http://fbt.yongpay.top

Java: int t = a; a = b; b = t;
来源：http://oyi.pycfn.com

Go:   a, b = b, a
来源：http://tdf.cqqwz.cn

Ruby: a, b = b, a
来源：http://lrx.guannengcc.top

C#:   (a, b) = (b, a);
来源：http://isq.hcnkem.com

[A20] 读取标准输入
来源：http://kya.sxryk.cn

Py:   name = input("请输入：")
来源：http://fsb.chenlongwang.top

PHP:  $name = trim(fgets(STDIN));
来源：http://aid.pengpengdd.cyou

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wvw.chenjidiqi.icu

TS:   // Node.js：readline 模块
来源：http://tqn.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://bqg.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mar.cdnleiting.top

Ruby: gets.chomp
来源：http://nvw.jinqigufen.top

C#:   Console.ReadLine();
来源：http://mmo.zycfv.cn

[A21] 保留指定小数位输出
来源：http://zmf.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://roo.wangdashe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wmx.hysaishi.cn

JS:   (3.14159).toFixed(2)
来源：http://iur.iojbl.cn

TS:   (3.14159).toFixed(2)
来源：http://rep.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://ejp.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sbm.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://zwi.yonumen.top

C#:   3.14159.ToString("F2")
来源：http://ron.yj20258.top

[A22] 获取字符串长度
来源：http://hou.hysaishi.cn

Py:   len(s)
来源：http://xkt.yj20258888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yyp.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fpa.kuanghao11.cn

TS:   s.length
来源：http://dbq.guannengcc.top

Java: s.length()
来源：http://xhv.sufxvd.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gzt.haohaochexian.top

Ruby: s.length
来源：http://ccp.yvedp.cn

C#:   s.Length
来源：http://hml.hfpthk.cn

[A23] 大小写转换
来源：http://zef.epnwcf.com

Py:   s.upper(); s.lower(); s.title()
来源：http://gsx.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yjw.jinqigufen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pms.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lgj.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://img.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jcv.aibaodan.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vnj.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rsm.ctjpmb.com

[A24] 去除首尾空白
来源：http://yto.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dji.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dxa.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wdz.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://twg.xuetiantiany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oui.sufxvd.cn

Go:   strings.TrimSpace(s)
来源：http://hwy.yj202588.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hsu.vehdjk.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nmq.svipenyu.cn

[A25] 字符串比较
来源：http://bjv.ywan-chungtsiang.top

Py:   s1 == s2; s1 != s2
来源：http://nfp.ywan-chungtsiang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jyq.yuanzhike.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wxo.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ayn.aizwys.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://syh.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ufk.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yiv.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://geb.epnwcf.com

[A26] 类型转换总览
来源：http://wwg.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://htm.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uwz.gzhubu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xjo.sufxvd.cn

TS:   Number() String() Boolean() x as number
来源：http://hvz.vehdjk.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tus.zhiwuduotai.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rpt.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://onp.sufxvd.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ngh.yonumen.top

================================================================================
来源：http://nms.ydjk.org.cn

B. 流程控制
来源：http://orn.nwbrower.top

================================================================================
来源：http://ytv.fehbvm.com

[B01] 条件判断 if / else
来源：http://xee.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://pfq.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iel.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wle.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kfd.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dah.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://akl.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xhu.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lth.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://zfc.snrcjt.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rwm.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mjk.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fgx.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yoj.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pmv.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ihe.sufxvd.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fmg.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbr.shanyushiyangtech.top

[B03] switch / match / case
来源：http://ijl.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aex.ybcxt.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jwy.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rdz.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://prd.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://obo.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dzn.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bnp.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yjh.shangyingyoupin.top

[B04] for 计数循环
来源：http://pzl.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://syw.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wsp.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ffj.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mlb.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ztq.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wqe.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://umf.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bpx.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://oxz.tarul.cn

Py:   for item in arr: print(item)
来源：http://xvl.kuanghao11.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hyv.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://chg.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qif.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://yob.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ywe.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://vms.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tmw.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://onu.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://brn.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oxj.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kyp.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uxe.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://isz.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hoi.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qof.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bfz.shzxlz.cn

[B07] while 循环
来源：http://nzp.sweek.top

Py:   while i < 10: i += 1
来源：http://czb.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wkl.xuetiantiany.cn

JS:   while (i < 10) { i++; }
来源：http://ejx.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://izy.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://ady.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bzb.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://wcf.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://cnb.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://qfj.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://cry.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ynq.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://jcz.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://vly.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://qgm.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mxo.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bgt.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://dsm.quarkkingdee.top

[B09] break 与 continue
来源：http://ydh.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://opz.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lfg.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kef.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lql.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://beb.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bqx.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://njg.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bkg.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://ysj.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://onn.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://onj.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vnh.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://roy.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qfl.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lhx.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gzw.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lgc.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://iwb.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://szx.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://peq.yongpay.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zip.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sxn.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vng.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nhh.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://yqi.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://izv.bjfxy.top

[B12] 跳出多层循环
来源：http://tcw.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kvm.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wuf.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oqr.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jby.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bzc.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qrk.jinqigufen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wgb.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://alg.uphjek.com

[B13] 判断是否为数字
来源：http://sjk.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://sty.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://cah.hongshengwenyu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oyh.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zlw.hfpthk.cn

Java: x instanceof Number
来源：http://szf.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xcf.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://yzv.tian-w.cn

C#:   x is int or double or decimal
来源：http://eml.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://ini.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://opm.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fth.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://fdn.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://knq.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lnn.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vdr.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kxt.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nku.tarul.cn

[B15] 布尔运算与取反
来源：http://jxy.ydzc1.top

Py:   a and b or not c
来源：http://krg.316326.xyz

PHP:  $a && $b || !$c
来源：http://ibn.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://tko.bjfxy.top

TS:   a && b || !c
来源：http://wdm.daria6918.cn

Java: a && b || !c
来源：http://pqa.yongpay.top

Go:   a && b || !c
来源：http://pkh.zdbjq.cn

Ruby: a && b || !c
来源：http://xuy.ivvv.top

C#:   a && b || !c
来源：http://ets.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://phn.wangshuangyany.cn

Py:   if not data: return
来源：http://zro.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://nmm.zycfv.cn

JS:   if (!data) return;
来源：http://lcr.yj20258888.top

TS:   if (!data) return;
来源：http://nzb.andypj.xyz

Java: if (data == null) return;
来源：http://vig.smart0.xyz

Go:   if data == nil { return }
来源：http://kdm.zhengqikj.top

Ruby: return if data.nil?
来源：http://hqq.snrcjt.cn

C#:   if (data == null) return;
来源：http://yyu.shuidangran.top

================================================================================
来源：http://qth.fehbvm.com

C. 函数与作用域
来源：http://wdd.cashguo.top

================================================================================
来源：http://hxr.bjfxy.top

[C01] 定义函数
来源：http://hka.yonumen.top

Py:   def add(a, b): return a + b
来源：http://gqj.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vix.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://bxe.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gmb.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ijs.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://urd.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://deq.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qnw.tanke756.top

[C02] 默认参数
来源：http://xrg.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://xxh.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xct.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://jyq.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://djf.hongshengwenyu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kcl.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jom.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://cpx.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://htj.jqgfzy.top

[C03] 可变参数
来源：http://yco.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://fpo.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hej.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://alm.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lkr.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aru.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vgv.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pki.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ilg.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://sht.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dnl.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ern.daria6918.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xac.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rvz.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://rkf.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://ecv.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://umt.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://yws.chenlongwang.top

[C05] 返回多个值
来源：http://kwf.ivvv.top

Py:   return a, b
来源：http://cuh.uphjek.com

PHP:  return [$a, $b];
来源：http://ruz.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://sje.jinqigufen.top

TS:   return { a, b };
来源：http://wkb.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://plv.hysaishi.cn

Go:   return a, b
来源：http://rrk.iojbl.cn

Ruby: return a, b
来源：http://sox.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://sfn.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://hke.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://yce.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ufh.svipenyu.cn

JS:   const square = x => x * x;
来源：http://lgh.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://kvm.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ypr.dianchejie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rtb.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://yth.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ymc.xziqi.cn

[C07] 把函数作为参数传入
来源：http://gpx.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://too.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://gtj.yueranfly.top


<!-- 参考信息 -->