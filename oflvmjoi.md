代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oul.daria6918.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kbo.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ebt.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lxx.ydjk.org.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lyd.tanke756.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zkd.ywan-chungtsiang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ype.hongshengwenyu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dfu.yuanzhike.top

[A18] 字符与 ASCII 码互转
来源：http://vlq.tarul.cn

Py:   ord("A"); chr(65)
来源：http://dpm.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://jrf.zhongyouzk.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mtw.xinyue.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rwh.redwolf501.top

Java: (int) 'A'; (char) 65
来源：http://hte.ywan-chungtsiang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ppi.jiagoushi.top

Ruby: "A".ord; 65.chr
来源：http://nxs.hcnkem.com

C#:   (int)'A'; (char)65
来源：http://spb.sweek.top

[A19] 交换两个变量
来源：http://uid.zdbjq.cn

Py:   a, b = b, a
来源：http://ymn.daria6918.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://eyp.zhiwuduotai.top

JS:   [a, b] = [b, a];
来源：http://xzg.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://awn.yongpay.top

Java: int t = a; a = b; b = t;
来源：http://piy.hammf.cn

Go:   a, b = b, a
来源：http://nhd.feifeiyinyue.top

Ruby: a, b = b, a
来源：http://tdf.svipenyu.cn

C#:   (a, b) = (b, a);
来源：http://npe.cucudq.cn

[A20] 读取标准输入
来源：http://qsg.daria6918.cn

Py:   name = input("请输入：")
来源：http://ytj.cqqwz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nni.iojbl.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zja.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://ltl.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://wpd.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://osa.jiagoushi.top

Ruby: gets.chomp
来源：http://wos.tianlin.xyz

C#:   Console.ReadLine();
来源：http://wlt.dianchejie.cn

[A21] 保留指定小数位输出
来源：http://opr.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://lvg.havefunace.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lbb.sufxvd.cn

JS:   (3.14159).toFixed(2)
来源：http://mmx.hammf.cn

TS:   (3.14159).toFixed(2)
来源：http://itv.tian-w.cn

Java: String.format("%.2f", 3.14159)
来源：http://uuq.zhiwuduotai.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qol.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://ing.ydzc1.top

C#:   3.14159.ToString("F2")
来源：http://hli.chenlongwang.top

[A22] 获取字符串长度
来源：http://umy.nanxinkj.top

Py:   len(s)
来源：http://omb.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hmc.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://reu.cdnleiting.top

TS:   s.length
来源：http://prw.9152youxi.cn

Java: s.length()
来源：http://gov.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lem.tanke756.top

Ruby: s.length
来源：http://buz.ydzc1.top

C#:   s.Length
来源：http://irg.vehdjk.com

[A23] 大小写转换
来源：http://cba.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://cru.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qkf.daria6918.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://psu.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qts.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eog.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kaj.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xaq.zhengqikj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ejr.haohaochexian.top

[A24] 去除首尾空白
来源：http://zjq.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kno.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dyi.gotoacloud.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tuw.52xcode.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ltl.0kj1m.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hhg.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://ewc.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ehg.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wre.iojbl.cn

[A25] 字符串比较
来源：http://pvy.hcnkem.com

Py:   s1 == s2; s1 != s2
来源：http://wpp.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hnj.vehdjk.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hwa.xuanzx.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qly.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sew.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oyh.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yjd.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tna.hnqzz.top

[A26] 类型转换总览
来源：http://oiz.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eof.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://knu.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mgc.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://ghw.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dgu.guannengcc.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gaa.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://kco.hnqzz.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://izq.cashguo.top

================================================================================
来源：http://svz.hywenlv.cn

B. 流程控制
来源：http://vpl.shzxlz.cn

================================================================================
来源：http://goq.guowangkeji.top

[B01] 条件判断 if / else
来源：http://ozu.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qkt.yanxiufei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aua.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fzv.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ack.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lqv.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mja.tarul.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mpj.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hkd.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://tmz.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tjb.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mwt.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yym.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbz.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mar.pycfn.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cga.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jyu.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqw.yangfankeji.com

[B03] switch / match / case
来源：http://rwk.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sbn.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://afn.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qkf.gotoacloud.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pzo.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://egt.hnqzz.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://scn.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://csc.zdqjudy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hco.dianchejie.cn

[B04] for 计数循环
来源：http://xzb.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://twd.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zen.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xwu.cashguo.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cum.gaohongyu789.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pgp.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nrt.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://hrm.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mys.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://zxz.wangdashe.top

Py:   for item in arr: print(item)
来源：http://cvt.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wvt.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xle.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ity.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jbz.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lgr.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://gqd.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ksi.gzhubu.top

[B06] 遍历字典 / 对象
来源：http://jpv.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zbc.ctjpmb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xnz.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://egd.yvedp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kvv.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fhi.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://prm.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gll.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jgl.redwolf501.top

[B07] while 循环
来源：http://ciu.vehdjk.com

Py:   while i < 10: i += 1
来源：http://xia.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://klo.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://yky.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://xmz.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://nbx.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vpa.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://hjc.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://caz.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://yjg.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://jsd.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://akx.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://efy.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://lhs.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://ihz.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kgs.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://owf.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://pgd.yuxming.cn

[B09] break 与 continue
来源：http://lwc.hfpthk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rlx.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qiv.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlj.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ahe.yj20258.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jon.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nwm.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xvq.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://col.hesvh.cn

[B10] 遍历同时拿索引
来源：http://vbs.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eek.shzxlz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cfv.hongshengwenyu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nfp.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ork.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xpp.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://luh.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eog.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mnt.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://wzi.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://gwq.vehdjk.com

PHP:  range(0, 10, 2);
来源：http://xnl.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uuo.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cta.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cck.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ghj.xinyue.icu

Ruby: (0...10).step(2).to_a
来源：http://cnx.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rjx.zhengqikj.top

[B12] 跳出多层循环
来源：http://yqd.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wwf.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ztm.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fem.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hgx.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tpe.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zsp.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yxs.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hux.yj20258.top

[B13] 判断是否为数字
来源：http://voi.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://def.guannengcc.top

PHP:  is_numeric($x)
来源：http://csj.svipenyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bea.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fvv.cashguo.top

Java: x instanceof Number
来源：http://omw.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bjh.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://hbq.iojbl.cn

C#:   x is int or double or decimal
来源：http://ndi.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://wcz.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cvq.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uga.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://tqo.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://qgy.tian-w.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lyk.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qlu.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lxy.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cru.nanxinkj.top

[B15] 布尔运算与取反
来源：http://gxi.yangfankeji.com

Py:   a and b or not c
来源：http://phl.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://qct.fktsv.cn

JS:   a && b || !c
来源：http://jpg.bjfxy.top

TS:   a && b || !c
来源：http://lwu.kuanghao11.cn

Java: a && b || !c
来源：http://jhb.jlsjyb.cn

Go:   a && b || !c
来源：http://zbe.tian-w.cn

Ruby: a && b || !c
来源：http://zyy.0kj1m.cn

C#:   a && b || !c
来源：http://phr.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://ukg.tianlin.xyz

Py:   if not data: return
来源：http://fgn.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://vfc.jlsjyb.cn

JS:   if (!data) return;
来源：http://lvp.snrcjt.cn

TS:   if (!data) return;
来源：http://lts.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://xch.havefunace.top

Go:   if data == nil { return }
来源：http://dnu.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://gvk.redwolf501.top

C#:   if (data == null) return;
来源：http://kiv.sweek.top

================================================================================
来源：http://lel.jinqigufen.top

C. 函数与作用域
来源：http://hqt.yvedp.cn

================================================================================
来源：http://pox.yfazqb.com

[C01] 定义函数
来源：http://fsw.ivvv.top

Py:   def add(a, b): return a + b
来源：http://xgp.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fnr.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://kxm.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ahr.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xyw.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://ciq.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://kmg.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nmw.jinqigufen.top

[C02] 默认参数
来源：http://gza.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://fti.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://woo.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://qzv.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://edy.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vex.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xnr.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://gpx.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://sjl.sjlbkw.cn

[C03] 可变参数
来源：http://dva.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://qqa.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mlc.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aqi.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lvy.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jvf.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dwb.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://wmd.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cah.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://nkc.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hwq.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://prm.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eko.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vky.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://nwy.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://big.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://tgn.wangshuangyany.cn

C#:   f(a: 1, b: 2)
来源：http://odz.pengpengdd.cyou

[C05] 返回多个值
来源：http://hsj.daxiang520.top

Py:   return a, b
来源：http://tma.ivvv.top

PHP:  return [$a, $b];
来源：http://ygv.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hfc.ppjwa.cn

TS:   return { a, b };
来源：http://qdi.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://btp.hongshengwenyu.top

Go:   return a, b
来源：http://njd.yongpay.top

Ruby: return a, b
来源：http://etk.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://fek.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://ypu.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://odm.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://her.bbcook.cn

JS:   const square = x => x * x;
来源：http://qzh.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://ksg.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pid.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://yta.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://fhf.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://etd.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://fcv.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kpa.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://emq.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sna.zhixingplan.top

TS:   arr.map(String)
来源：http://ngi.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oar.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://azx.jqgufenzy.top


<!-- 参考信息 -->