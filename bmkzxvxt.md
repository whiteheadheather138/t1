代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tlb.zhixingplan.top

Ruby: unless x            # nil 与 false 为假
来源：http://qpg.zhengqikj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://alj.jianghu66.top

[A17] 位运算
来源：http://ytn.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jjr.snrcjt.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bcn.yanxiufei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntt.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tww.svipenyu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dij.yanxiufei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xre.aibaodan.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wet.sweek.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tqy.guowangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://aen.gotoacloud.top

Py:   ord("A"); chr(65)
来源：http://tma.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://tlx.jyoumei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sqc.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cxn.redwolf501.top

Java: (int) 'A'; (char) 65
来源：http://kwo.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nbz.zdqjudy.top

Ruby: "A".ord; 65.chr
来源：http://oqw.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://afp.vehdjk.com

[A19] 交换两个变量
来源：http://nje.hywenlv.cn

Py:   a, b = b, a
来源：http://nad.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tqk.zhijiandao.cn

JS:   [a, b] = [b, a];
来源：http://asb.gaohongyu789.top

TS:   [a, b] = [b, a];
来源：http://gic.guannengcc.top

Java: int t = a; a = b; b = t;
来源：http://ruy.redwolf501.top

Go:   a, b = b, a
来源：http://vnq.yvedp.cn

Ruby: a, b = b, a
来源：http://bfk.xylfe.cn

C#:   (a, b) = (b, a);
来源：http://gab.pengpengdd.cyou

[A20] 读取标准输入
来源：http://gtc.hysaishi.cn

Py:   name = input("请输入：")
来源：http://jiq.mhx1999.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tkc.zdqjudy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tpx.hesvh.cn

TS:   // Node.js：readline 模块
来源：http://bmd.ctjpmb.com

Java: new Scanner(System.in).nextLine()
来源：http://qdq.xylfe.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rsg.tarul.cn

Ruby: gets.chomp
来源：http://jxy.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://rvt.hammf.cn

[A21] 保留指定小数位输出
来源：http://lrt.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://laq.yj20258888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fxc.xziqi.cn

JS:   (3.14159).toFixed(2)
来源：http://hku.hysaishi.cn

TS:   (3.14159).toFixed(2)
来源：http://dpd.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://wgy.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://irl.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://azs.pycfn.com

C#:   3.14159.ToString("F2")
来源：http://jul.zdqjudy.top

[A22] 获取字符串长度
来源：http://klh.haohaochexian.top

Py:   len(s)
来源：http://rmg.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zmc.yonumen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uss.redwolf501.top

TS:   s.length
来源：http://ndh.nanxuanxn.top

Java: s.length()
来源：http://dws.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zea.zdbjq.cn

Ruby: s.length
来源：http://khz.chenzaomai.com

C#:   s.Length
来源：http://myq.aibaodan.cn

[A23] 大小写转换
来源：http://eun.guannengcc.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kse.jiagoushi.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qae.xuanzx.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ebi.fzhhl.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vdj.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cfy.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://klj.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://alp.ybcxt.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gjk.aibaodan.cn

[A24] 去除首尾空白
来源：http://ppo.wangdashe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qgu.shanyushiyangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wns.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hng.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xjj.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dhp.hfpthk.cn

Go:   strings.TrimSpace(s)
来源：http://enl.haohaochexian.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rss.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jzo.zhixingplan.top

[A25] 字符串比较
来源：http://tkn.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://rsl.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://unh.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qvt.jinqigufen.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bwo.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rob.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xls.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tnl.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tjb.chenlongwang.top

[A26] 类型转换总览
来源：http://dkh.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ujc.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dks.shzxlz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nlm.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://fgx.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zwj.sysykeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://god.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nzs.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kgi.pengpengdd.cyou

================================================================================
来源：http://cjs.jianghu66.top

B. 流程控制
来源：http://mzo.zhengqikj.top

================================================================================
来源：http://nvu.fzhhl.top

[B01] 条件判断 if / else
来源：http://qee.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kep.yonumen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://occ.hywenlv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xbg.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://igy.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jhx.ppjwa.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qws.pycfn.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wrz.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lsf.nanxinkj.top

[B02] 多分支 else if / elif
来源：http://lvr.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kwe.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://msj.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://flu.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iwm.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bna.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lbg.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jsu.smart0.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dss.quarkkingdee.top

[B03] switch / match / case
来源：http://fkb.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tab.cdnleiting.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mln.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vxm.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mda.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pzf.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lnc.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://use.zhaomingkeji.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aya.zdbjq.cn

[B04] for 计数循环
来源：http://iol.zhixingplan.top

Py:   for i in range(10): print(i)
来源：http://mcv.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nzc.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qew.zhongyouzk.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rhf.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tof.tarul.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xoq.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://fxz.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hvp.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://xfy.hfpthk.cn

Py:   for item in arr: print(item)
来源：http://gqf.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iwe.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vwb.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://neu.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://icz.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://luz.cashguo.top

Ruby: arr.each { |item| puts item }
来源：http://ffc.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ysa.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://vkg.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ogx.pycfn.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rkh.gaohongyu789.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rij.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mvw.nwbrower.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vbp.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zgc.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mkl.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hmc.wangdashe.top

[B07] while 循环
来源：http://asp.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://mqh.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vdt.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://zxz.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://odb.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://sie.ybcxt.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iqt.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://mjo.0kj1m.cn

C#:   while (i < 10) { i++; }
来源：http://ppq.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://afq.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://wvm.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kde.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://lnb.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://brj.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://sxd.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://vpq.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ria.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://qur.jinqigufen.top

[B09] break 与 continue
来源：http://oxk.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wjt.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://naj.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://era.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aht.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uka.zdqjudy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oom.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zxh.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dor.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://xul.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ifs.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xyy.yfazqb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://avx.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hlr.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nyw.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sic.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oqw.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hwn.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://yij.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://bjs.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://osa.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tws.hnxiangtu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wlp.chenzaomai.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qhy.snrcjt.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uxo.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://cbo.xuanzx.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mua.c1oappe.top

[B12] 跳出多层循环
来源：http://nsy.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mxz.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tjo.jianghu66.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wtz.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rrx.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://axi.gotoacloud.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zvs.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uih.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eoh.svipenyu.cn

[B13] 判断是否为数字
来源：http://ekl.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://apa.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://fsg.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bme.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yrc.yfazqb.com

Java: x instanceof Number
来源：http://klh.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iwm.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://oez.chenzaomai.com

C#:   x is int or double or decimal
来源：http://hse.xziqi.cn

[B14] 判断值是否在集合内
来源：http://dww.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qgt.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rev.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://bga.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://ldf.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://qml.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gbt.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://hfa.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sub.cqqwz.cn

[B15] 布尔运算与取反
来源：http://iry.hesvh.cn

Py:   a and b or not c
来源：http://jqo.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://mgf.shuidangran.top

JS:   a && b || !c
来源：http://qsh.ybcxt.top

TS:   a && b || !c
来源：http://fmr.yangfankeji.com

Java: a && b || !c
来源：http://xqr.daxiang520.top

Go:   a && b || !c
来源：http://jgc.wangshuangyany.cn

Ruby: a && b || !c
来源：http://tbg.vqdsnc.cn

C#:   a && b || !c
来源：http://ojh.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://nnh.bbcook.cn

Py:   if not data: return
来源：http://vso.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://umi.0kj1m.cn

JS:   if (!data) return;
来源：http://mld.haohaochexian.top

TS:   if (!data) return;
来源：http://pvo.jiagoushi.top

Java: if (data == null) return;
来源：http://ddh.ppjwa.cn

Go:   if data == nil { return }
来源：http://otf.aizwys.cn

Ruby: return if data.nil?
来源：http://das.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://kri.hywenlv.cn

================================================================================
来源：http://zwu.tianlin.xyz

C. 函数与作用域
来源：http://fbo.jinghuilouyu.cn

================================================================================
来源：http://aeb.bbcook.cn

[C01] 定义函数
来源：http://mka.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://rbn.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tvo.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://aec.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://crw.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ucj.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://bwf.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://kiu.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sww.sjlbkw.cn

[C02] 默认参数
来源：http://tbx.uphjek.com

Py:   def greet(name="World"): return name
来源：http://ihg.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://enc.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://avz.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vbk.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kgx.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gtr.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://evj.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://vfo.nanxinkj.top

[C03] 可变参数
来源：http://tgm.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://ndq.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qje.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://srm.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jwe.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://frq.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ktj.yangfankeji.com

Ruby: def total(*nums); nums.sum; end
来源：http://eii.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://joy.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://swx.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xmq.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fuv.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zau.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jaa.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://pwz.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://qul.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://lbo.yuanzhike.top

C#:   f(a: 1, b: 2)
来源：http://kwp.yvedp.cn

[C05] 返回多个值
来源：http://ccj.ydzc1.top

Py:   return a, b
来源：http://fds.epnwcf.com

PHP:  return [$a, $b];
来源：http://blr.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dyv.sxryk.cn

TS:   return { a, b };
来源：http://dzq.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fdt.zhijiandao.cn

Go:   return a, b
来源：http://sbf.shangyingyoupin.top

Ruby: return a, b
来源：http://rjt.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://xya.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://xtj.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://itf.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hpz.vehdjk.com

JS:   const square = x => x * x;
来源：http://kgx.dianchejie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ipd.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uff.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://pkd.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://hzg.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xxb.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://bwx.zhaomingkeji.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gcw.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://iuh.yfazqb.com


<!-- 参考信息 -->