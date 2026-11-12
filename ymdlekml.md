代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lcl.shanyushiyangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ixi.havefunace.top

TS:   if (!x) {}
来源：http://elh.daxiang520.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://smo.cdnleiting.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jsh.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://itd.yuxming.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mjw.daxiang520.top

[A17] 位运算
来源：http://lgy.cashguo.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://noc.ppjwa.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://joq.fktsv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jdl.zhiwuduotai.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mou.c1oappe.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://npd.yuxming.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gvf.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fyy.sxryk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hok.ybcxt.top

[A18] 字符与 ASCII 码互转
来源：http://kly.hysaishi.cn

Py:   ord("A"); chr(65)
来源：http://wfq.fehbvm.com

PHP:  ord("A"); chr(65)
来源：http://ook.ybcxt.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dux.cashguo.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tii.hfpthk.cn

Java: (int) 'A'; (char) 65
来源：http://ixj.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hgt.nwbrower.top

Ruby: "A".ord; 65.chr
来源：http://mva.dashuyun.cn

C#:   (int)'A'; (char)65
来源：http://shw.chenlongwang.top

[A19] 交换两个变量
来源：http://bvk.redwolf501.top

Py:   a, b = b, a
来源：http://xwx.ivvv.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xrn.epnwcf.com

JS:   [a, b] = [b, a];
来源：http://lqn.hammf.cn

TS:   [a, b] = [b, a];
来源：http://jsw.smart0.xyz

Java: int t = a; a = b; b = t;
来源：http://ryv.yj202588.top

Go:   a, b = b, a
来源：http://npx.shanyushiyangkeji.top

Ruby: a, b = b, a
来源：http://yde.ppjwa.cn

C#:   (a, b) = (b, a);
来源：http://jze.daria6918.cn

[A20] 读取标准输入
来源：http://hiz.sjlbkw.cn

Py:   name = input("请输入：")
来源：http://mlh.yangfankeji.com

PHP:  $name = trim(fgets(STDIN));
来源：http://dmp.jiagoushi.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qjl.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://qdh.yanxiufei.cn

Java: new Scanner(System.in).nextLine()
来源：http://gcr.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aul.jinghuilouyu.cn

Ruby: gets.chomp
来源：http://ucr.cashguo.top

C#:   Console.ReadLine();
来源：http://ubj.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://jah.cqqwz.cn

Py:   f"{3.14159:.2f}"
来源：http://vwm.ctjpmb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iyn.shuidangran.top

JS:   (3.14159).toFixed(2)
来源：http://uox.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://iof.cucudq.cn

Java: String.format("%.2f", 3.14159)
来源：http://mpr.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://opc.yfazqb.com

Ruby: format("%.2f", 3.14159)
来源：http://xde.pycfn.com

C#:   3.14159.ToString("F2")
来源：http://wby.gaohongyu789.top

[A22] 获取字符串长度
来源：http://kxh.shuidangran.top

Py:   len(s)
来源：http://isd.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vmj.jiagoushi.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rqm.fengsongda.top

TS:   s.length
来源：http://xhe.jiagoushi.top

Java: s.length()
来源：http://nfs.fzhhl.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dow.nanxuanxn.top

Ruby: s.length
来源：http://csf.bbcook.cn

C#:   s.Length
来源：http://wvs.bjfxy.top

[A23] 大小写转换
来源：http://jri.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gmx.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aee.haohaochexian.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wxa.tian-w.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gfv.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bip.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hnu.zhoulong.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nay.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nxh.ybcxt.top

[A24] 去除首尾空白
来源：http://sjy.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://acm.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zav.jlsjyb.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wop.bjfxy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eju.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ime.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://dsc.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://usr.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hiz.jinqigufen.top

[A25] 字符串比较
来源：http://lgi.smart0.xyz

Py:   s1 == s2; s1 != s2
来源：http://kag.316326.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mry.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gjo.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lop.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kui.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sah.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bkw.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rvz.fzhhl.top

[A26] 类型转换总览
来源：http://ojn.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://spq.yongpay.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lex.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ucf.hongshengwenyu.top

TS:   Number() String() Boolean() x as number
来源：http://fyt.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fuj.havefunace.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rle.tanke756.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zme.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cxm.zhijiandao.cn

================================================================================
来源：http://yjn.jqgufenzy.top

B. 流程控制
来源：http://nqh.dianchejie.cn

================================================================================
来源：http://lie.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://upe.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ric.52xcode.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://opi.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aog.nanxuanxn.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eyj.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jod.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xor.zhiwuduotai.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kec.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://igu.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://ctl.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vmr.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vjw.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://taq.hesvh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://apc.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wko.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://obk.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wrw.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://beb.gaohongyu789.top

[B03] switch / match / case
来源：http://uhj.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://elb.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://khc.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://epy.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tvt.tarul.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wer.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://txn.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sfw.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://npf.uphjek.com

[B04] for 计数循环
来源：http://sbq.fktsv.cn

Py:   for i in range(10): print(i)
来源：http://fqm.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wqh.chenlongwang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jix.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pne.pycfn.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dtc.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://umm.gaohongyu789.top

Ruby: 10.times { |i| puts i }
来源：http://reo.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jir.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://gzt.hammf.cn

Py:   for item in arr: print(item)
来源：http://boj.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nyy.mhx1999.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uen.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gid.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xli.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zwx.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://try.hesvh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qzl.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://ygp.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ral.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://npx.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tcd.gogol.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wse.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://shy.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kdb.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jdf.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qwh.bjfxy.top

[B07] while 循环
来源：http://dos.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://ufu.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://ljp.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://zfv.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://fds.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://pmm.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vgx.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://thj.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://hhs.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://oat.zhixingplan.top

Py:   # 无 do-while：用 while True + break
来源：http://nlx.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://das.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://scc.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://wxy.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://rfh.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uoq.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://aui.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://mmu.wangshuangyany.cn

[B09] break 与 continue
来源：http://awo.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ull.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vwk.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svi.pengpengdd.cyou

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqy.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://elc.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ime.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mjm.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bhg.ydzc1.top

[B10] 遍历同时拿索引
来源：http://zpu.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ybk.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qsc.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxg.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vve.aizwys.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zxl.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rzf.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kbq.yuxming.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xzf.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://ayr.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://pjr.xuetiantiany.cn

PHP:  range(0, 10, 2);
来源：http://ddz.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hsj.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rhl.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aee.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bxw.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://cvi.52xcode.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dth.yj20258.top

[B12] 跳出多层循环
来源：http://zte.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dca.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://eij.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vyy.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fuh.guowangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fsu.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kkr.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cqi.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vff.9152youxi.cn

[B13] 判断是否为数字
来源：http://rll.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://pxb.hysaishi.cn

PHP:  is_numeric($x)
来源：http://zvn.guowangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zqp.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ecg.jyoumei.cn

Java: x instanceof Number
来源：http://vvk.cqqwz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wgx.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://oyi.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://grn.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://hae.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cca.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rga.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://uiz.ehwqpu.com

TS:   [1, 2, 3].includes(x)
来源：http://bwg.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://zlh.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hqk.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zem.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vkr.yfazqb.com

[B15] 布尔运算与取反
来源：http://vrq.aibaodan.cn

Py:   a and b or not c
来源：http://civ.birdmap.top

PHP:  $a && $b || !$c
来源：http://rgb.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://aur.yongpay.top

TS:   a && b || !c
来源：http://wys.sysykeji.top

Java: a && b || !c
来源：http://pjs.pycfn.com

Go:   a && b || !c
来源：http://yjm.daxiang520.top

Ruby: a && b || !c
来源：http://rwk.0kj1m.cn

C#:   a && b || !c
来源：http://wnc.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://mgy.gogol.net.cn

Py:   if not data: return
来源：http://dlm.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://qun.haohaochexian.top

JS:   if (!data) return;
来源：http://ffk.tarul.cn

TS:   if (!data) return;
来源：http://qht.jlsjyb.cn

Java: if (data == null) return;
来源：http://gyv.uphjek.com

Go:   if data == nil { return }
来源：http://yxt.fehbvm.com

Ruby: return if data.nil?
来源：http://cdk.jqgufenzy.top

C#:   if (data == null) return;
来源：http://pkg.jiagoushi.top

================================================================================
来源：http://rvo.sweek.top

C. 函数与作用域
来源：http://nup.52xcode.cn

================================================================================
来源：http://lhh.hongshengwenyu.top

[C01] 定义函数
来源：http://lbo.cashguo.top

Py:   def add(a, b): return a + b
来源：http://ong.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oft.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://uyt.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://akk.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nhg.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://trr.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://jta.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oei.shuidangran.top

[C02] 默认参数
来源：http://uis.meibo888.top

Py:   def greet(name="World"): return name
来源：http://jub.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mld.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://pyt.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jwh.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://svy.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iyh.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://ouy.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://izy.andypj.xyz

[C03] 可变参数
来源：http://jsp.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://dph.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kjx.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vxg.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yne.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ngf.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zxz.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://kvq.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uxb.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://axs.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lda.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://omq.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kwj.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yud.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://emv.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://bdz.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://tqh.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://jag.shuidangran.top

[C05] 返回多个值
来源：http://qfs.cashguo.top

Py:   return a, b
来源：http://apq.fehbvm.com

PHP:  return [$a, $b];
来源：http://nac.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cbs.fehbvm.com

TS:   return { a, b };
来源：http://uih.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://new.jyoumei.cn

Go:   return a, b
来源：http://vot.fktsv.cn

Ruby: return a, b
来源：http://gqr.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://reh.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://azp.daria6918.cn

Py:   square = lambda x: x * x
来源：http://xeo.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eab.meibo888.top

JS:   const square = x => x * x;
来源：http://jtl.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://pnm.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dye.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dzp.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://cnw.cashguo.top


<!-- 参考信息 -->