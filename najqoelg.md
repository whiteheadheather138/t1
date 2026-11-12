代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bjh.tarul.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pll.hfpthk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fst.haohaochexian.top

[A17] 位运算
来源：http://hht.vqdsnc.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://utr.ehwqpu.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eqg.smart0.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iai.smart0.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xpi.yj20258888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrd.bjfxy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://igs.tian-w.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pez.hnqzz.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kfu.guannengcc.top

[A18] 字符与 ASCII 码互转
来源：http://dvp.epnwcf.com

Py:   ord("A"); chr(65)
来源：http://hud.shanyushiyangtech.top

PHP:  ord("A"); chr(65)
来源：http://vyy.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vql.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xxz.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://hfi.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mmt.snrcjt.cn

Ruby: "A".ord; 65.chr
来源：http://tvy.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://tfj.shzxlz.cn

[A19] 交换两个变量
来源：http://omn.daria6918.cn

Py:   a, b = b, a
来源：http://xqo.bjfxy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nhn.jlsjyb.cn

JS:   [a, b] = [b, a];
来源：http://nqs.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://bvy.pengpengdd.cyou

Java: int t = a; a = b; b = t;
来源：http://aqq.fktsv.cn

Go:   a, b = b, a
来源：http://tqf.zhixingplan.top

Ruby: a, b = b, a
来源：http://vsp.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://viy.yueranfly.top

[A20] 读取标准输入
来源：http://vhz.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://tlr.sweek.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xut.smart0.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ldt.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://cim.tanke756.top

Java: new Scanner(System.in).nextLine()
来源：http://bax.c1oappe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tny.tanke756.top

Ruby: gets.chomp
来源：http://qfb.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://fex.birdmap.top

[A21] 保留指定小数位输出
来源：http://xsj.hfpthk.cn

Py:   f"{3.14159:.2f}"
来源：http://bnp.316326.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jjy.xziqi.cn

JS:   (3.14159).toFixed(2)
来源：http://pji.yj202588.top

TS:   (3.14159).toFixed(2)
来源：http://zdy.wangdashe.top

Java: String.format("%.2f", 3.14159)
来源：http://ijq.zhaomingkeji.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uyf.redwolf501.top

Ruby: format("%.2f", 3.14159)
来源：http://ekx.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://kka.gzhubu.top

[A22] 获取字符串长度
来源：http://pqj.zdbjq.cn

Py:   len(s)
来源：http://rjw.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ciz.guowangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pip.nanxinkj.top

TS:   s.length
来源：http://tcl.yvedp.cn

Java: s.length()
来源：http://wln.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lux.jinqigufen.top

Ruby: s.length
来源：http://rlr.pycfn.com

C#:   s.Length
来源：http://xnl.gzhubu.top

[A23] 大小写转换
来源：http://nms.fehbvm.com

Py:   s.upper(); s.lower(); s.title()
来源：http://aeg.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yxu.jianghu66.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vnc.hcnkem.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zxu.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ksl.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oxg.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sxo.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://dst.uphjek.com

[A24] 去除首尾空白
来源：http://ere.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fnd.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mii.fanxiaobao.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cda.yonumen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ico.0kj1m.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xyh.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://vsg.gaohongyu789.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uyd.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vjz.shangyingyoupin.top

[A25] 字符串比较
来源：http://eda.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://lzz.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://imw.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dtk.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kug.andypj.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vxk.sufxvd.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ska.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kzh.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rba.guowangkeji.top

[A26] 类型转换总览
来源：http://ixr.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yny.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pjk.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pht.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://bzr.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://klv.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kwt.yuxming.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nhz.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dik.ydjk.org.cn

================================================================================
来源：http://bzr.ehwqpu.com

B. 流程控制
来源：http://nfq.wangdashe.top

================================================================================
来源：http://whe.ehwqpu.com

[B01] 条件判断 if / else
来源：http://mvn.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dzl.meibo888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gsd.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qct.yj202588.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mss.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lin.9152youxi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pfk.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gss.cdnleiting.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qmf.yongpay.top

[B02] 多分支 else if / elif
来源：http://xiu.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tgh.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nia.xziqi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://adj.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://liv.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxk.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ygl.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://odx.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dok.gotoacloud.top

[B03] switch / match / case
来源：http://cqs.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gux.hysaishi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dav.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lcg.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kpg.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jhz.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mac.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hmv.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jen.vqdsnc.cn

[B04] for 计数循环
来源：http://hwu.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://imw.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bud.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wzl.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ylk.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tka.wangshuangyany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wjq.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://sco.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mtx.bbcook.cn

[B05] 遍历数组 / 列表
来源：http://rah.chenzaomai.com

Py:   for item in arr: print(item)
来源：http://mhu.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qei.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kjx.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yev.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fmx.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nbz.gzhubu.top

Ruby: arr.each { |item| puts item }
来源：http://uxl.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://snl.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://vvk.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ohi.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ubx.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hge.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bdj.wangshuangyany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fqi.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yfz.gzhubu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qnb.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ajr.c1oappe.top

[B07] while 循环
来源：http://zac.cashguo.top

Py:   while i < 10: i += 1
来源：http://gqa.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ama.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://mpm.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://qis.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://nju.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bnb.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://ygg.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://cck.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://krc.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://kcv.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://uhn.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://oua.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://slc.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://zlb.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ggu.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://pha.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://fst.fanxiaobao.xyz

[B09] break 与 continue
来源：http://zqt.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fsy.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xzu.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ply.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kah.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mag.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tvr.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yxv.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxy.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://mmw.daxiang520.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vlg.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pfk.jinyuanbaomall.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cbo.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zwg.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://due.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://goq.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eyf.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kie.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://yke.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://tsn.yonumen.top

PHP:  range(0, 10, 2);
来源：http://zyd.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jdh.hnxiangtu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocr.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fzw.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gmk.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://tlx.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hrl.zhengqikj.top

[B12] 跳出多层循环
来源：http://fei.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zxf.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lkw.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yjv.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aty.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eqr.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://odq.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zvh.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://owo.jyoumei.cn

[B13] 判断是否为数字
来源：http://ret.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://drg.hesvh.cn

PHP:  is_numeric($x)
来源：http://tfh.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ikk.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dfa.zhiwuduotai.top

Java: x instanceof Number
来源：http://eic.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cvz.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://bfs.tianlin.xyz

C#:   x is int or double or decimal
来源：http://nvh.tian-w.cn

[B14] 判断值是否在集合内
来源：http://ahe.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cxz.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tjy.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://lty.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://zpt.yueranfly.top

Java: List.of(1, 2, 3).contains(x)
来源：http://otq.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lpl.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uyj.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cnw.yongpay.top

[B15] 布尔运算与取反
来源：http://iai.svipenyu.cn

Py:   a and b or not c
来源：http://fdm.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://uzb.gaohongyu789.top

JS:   a && b || !c
来源：http://qmi.nwbrower.top

TS:   a && b || !c
来源：http://gdx.nwbrower.top

Java: a && b || !c
来源：http://egz.fzhhl.top

Go:   a && b || !c
来源：http://tyb.0kj1m.cn

Ruby: a && b || !c
来源：http://bdf.iojbl.cn

C#:   a && b || !c
来源：http://wao.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://oud.xuetiantiany.cn

Py:   if not data: return
来源：http://uxa.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://uyv.yueranfly.top

JS:   if (!data) return;
来源：http://pvl.chenjidiqi.icu

TS:   if (!data) return;
来源：http://tec.shzxlz.cn

Java: if (data == null) return;
来源：http://ltj.bbcook.cn

Go:   if data == nil { return }
来源：http://twr.smart0.xyz

Ruby: return if data.nil?
来源：http://wor.hammf.cn

C#:   if (data == null) return;
来源：http://iks.ybcxt.top

================================================================================
来源：http://fun.bjfxy.top

C. 函数与作用域
来源：http://weg.yanxiufei.cn

================================================================================
来源：http://bqz.52xcode.cn

[C01] 定义函数
来源：http://llj.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://hkb.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kfm.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://knq.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://psk.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://boy.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://kxs.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://zqr.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qlr.tianlin.xyz

[C02] 默认参数
来源：http://zsm.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://ote.zhongyouzk.top

PHP:  function greet($name = "World") { return $name; }
来源：http://exz.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://tlu.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://drw.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pql.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hms.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://tya.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://qtu.zdqjudy.top

[C03] 可变参数
来源：http://seb.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://pfg.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qou.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://isq.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://and.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fuw.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kbh.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://cqt.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hla.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://vkg.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vyk.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kwc.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jrh.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vaw.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://rxc.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://vpq.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://hqy.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://iyb.hongshengwenyu.top

[C05] 返回多个值
来源：http://udb.wangshuangyany.cn

Py:   return a, b
来源：http://ltc.svipenyu.cn

PHP:  return [$a, $b];
来源：http://okn.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://luk.birdmap.top

TS:   return { a, b };
来源：http://jqo.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kti.shanyushiyangtech.top

Go:   return a, b
来源：http://ggb.hfpthk.cn

Ruby: return a, b
来源：http://oah.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://rsl.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://lyn.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://ryg.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://zjd.chenlongwang.top

JS:   const square = x => x * x;
来源：http://kwk.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://hbx.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://csb.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ako.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://gtz.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ddo.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://tnv.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mch.ydzc1.top

PHP:  array_map("strtoupper", $arr);
来源：http://cdf.ppjwa.cn


<!-- 参考信息 -->