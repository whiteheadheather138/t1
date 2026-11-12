代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rpn.yj202588.top

Ruby: unless x            # nil 与 false 为假
来源：http://fdb.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://whj.zhongyouzk.top

[A17] 位运算
来源：http://hup.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xob.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iwq.yj20258888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yzf.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://htq.uphjek.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://etr.hongshengwenyu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zzf.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zim.sjlbkw.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vau.zycfv.cn

[A18] 字符与 ASCII 码互转
来源：http://nde.zhoulong.xyz

Py:   ord("A"); chr(65)
来源：http://hsa.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://yir.yj20258.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pva.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mbm.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://gpo.hammf.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wka.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://hjw.316326.xyz

C#:   (int)'A'; (char)65
来源：http://utg.chenlongwang.top

[A19] 交换两个变量
来源：http://isb.sjlbkw.cn

Py:   a, b = b, a
来源：http://gjd.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://qak.jqgfzy.top

JS:   [a, b] = [b, a];
来源：http://ljr.vehdjk.com

TS:   [a, b] = [b, a];
来源：http://kme.redwolf501.top

Java: int t = a; a = b; b = t;
来源：http://jwa.shangyingyoupin.top

Go:   a, b = b, a
来源：http://wsd.jiagoushi.top

Ruby: a, b = b, a
来源：http://fzt.gotoacloud.top

C#:   (a, b) = (b, a);
来源：http://hia.yvedp.cn

[A20] 读取标准输入
来源：http://xfj.fktsv.cn

Py:   name = input("请输入：")
来源：http://hid.ydzc1.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dle.ivvv.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pac.tanke756.top

TS:   // Node.js：readline 模块
来源：http://jqf.meibo888.top

Java: new Scanner(System.in).nextLine()
来源：http://usl.jlsjyb.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lsb.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://xtn.52xcode.cn

C#:   Console.ReadLine();
来源：http://oso.birdmap.top

[A21] 保留指定小数位输出
来源：http://vmd.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://qll.hysaishi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cyp.316326.xyz

JS:   (3.14159).toFixed(2)
来源：http://wzz.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://hkt.chenlongwang.top

Java: String.format("%.2f", 3.14159)
来源：http://jve.9152youxi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nld.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://vaj.mhx1999.top

C#:   3.14159.ToString("F2")
来源：http://wlx.ppjwa.cn

[A22] 获取字符串长度
来源：http://dnl.vehdjk.com

Py:   len(s)
来源：http://cla.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wls.zhongyouzk.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jgk.hammf.cn

TS:   s.length
来源：http://aik.svipenyu.cn

Java: s.length()
来源：http://lff.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cec.xylfe.cn

Ruby: s.length
来源：http://gqu.tarul.cn

C#:   s.Length
来源：http://uig.jlsjyb.cn

[A23] 大小写转换
来源：http://mmr.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xjs.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aqb.cashguo.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://smr.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zoy.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mmh.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gdc.jinqigufen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lwk.epnwcf.com

C#:   s.ToUpper(); s.ToLower()
来源：http://oqy.aizwys.cn

[A24] 去除首尾空白
来源：http://zsp.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ssm.meibo888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wjr.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qrr.yuxming.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://avp.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aha.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://fby.haohaochexian.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tfl.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bya.ydjk.org.cn

[A25] 字符串比较
来源：http://dpw.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://wbk.xziqi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://swd.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bvs.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://guf.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fuf.ppjwa.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oyb.gzhubu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jju.aizwys.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hmc.vqdsnc.cn

[A26] 类型转换总览
来源：http://dla.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dmi.yfazqb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dbw.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kle.vqdsnc.cn

TS:   Number() String() Boolean() x as number
来源：http://mue.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dxg.chenlongwang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kfe.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mml.fehbvm.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vqz.iojbl.cn

================================================================================
来源：http://mkx.havefunace.top

B. 流程控制
来源：http://lva.dianchejie.cn

================================================================================
来源：http://net.zhengqikj.top

[B01] 条件判断 if / else
来源：http://jjt.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://clo.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://akm.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rto.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jkp.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://atc.chenjidiqi.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bjj.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fca.ydzc1.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hwg.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://dnx.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ouu.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qpn.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rcs.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezk.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbq.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uzb.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kgd.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djk.kuanghao11.cn

[B03] switch / match / case
来源：http://vbo.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ipp.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lyw.hcnkem.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dmz.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tbl.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wbv.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://esj.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dbq.ctjpmb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wdp.xziqi.cn

[B04] for 计数循环
来源：http://pbq.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://bgj.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ppn.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvr.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mvo.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gsr.jinqigufen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wao.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://ywi.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iys.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://obj.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://vqw.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rmy.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cyz.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zpd.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mzr.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vxc.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://dfj.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zmj.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://gte.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fgv.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kwy.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vdf.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hbe.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rqg.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://goq.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ela.zhongyouzk.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lsg.haohaochexian.top

[B07] while 循环
来源：http://ofk.xinyue.icu

Py:   while i < 10: i += 1
来源：http://wmr.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://lir.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://ziv.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://xcz.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://hxm.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xex.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://iid.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://bqj.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://oqv.feifeiyinyue.top

Py:   # 无 do-while：用 while True + break
来源：http://fze.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cox.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://ybu.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://lwg.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://mbu.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uej.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://ywj.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://qdq.kuanghao11.cn

[B09] break 与 continue
来源：http://rzr.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iyk.jinghuilouyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ueg.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://luw.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdw.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://klk.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eza.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xni.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wqw.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://cmt.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://urh.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wdj.andypj.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxc.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xns.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uzl.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oob.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ffs.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://isk.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://eqg.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://zyy.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://nsk.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ikl.xylfe.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ruu.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kcw.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dul.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://rzb.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nlg.quarkkingdee.top

[B12] 跳出多层循环
来源：http://dsp.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rfk.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cuu.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xxl.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sub.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fgz.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bkc.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ivy.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lrz.chenjidiqi.icu

[B13] 判断是否为数字
来源：http://ktl.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://cys.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://yjb.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mjo.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fig.uphjek.com

Java: x instanceof Number
来源：http://alo.hongshengwenyu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dis.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://yuy.ctjpmb.com

C#:   x is int or double or decimal
来源：http://fsf.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://cfj.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pun.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vbz.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://goo.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://lao.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wro.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iha.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sdc.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wpd.ydzc1.top

[B15] 布尔运算与取反
来源：http://jvp.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://qwi.ivvv.top

PHP:  $a && $b || !$c
来源：http://hql.hongshengwenyu.top

JS:   a && b || !c
来源：http://jll.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://cox.yj20258888.top

Java: a && b || !c
来源：http://gfp.fanxiaobao.xyz

Go:   a && b || !c
来源：http://hzy.fktsv.cn

Ruby: a && b || !c
来源：http://egk.jinghuilouyu.cn

C#:   a && b || !c
来源：http://cke.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vej.aizwys.cn

Py:   if not data: return
来源：http://adu.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://edq.yuxming.cn

JS:   if (!data) return;
来源：http://ogn.shuidangran.top

TS:   if (!data) return;
来源：http://oxi.hfpthk.cn

Java: if (data == null) return;
来源：http://kmj.fehbvm.com

Go:   if data == nil { return }
来源：http://edx.yj202588.top

Ruby: return if data.nil?
来源：http://zqv.hywenlv.cn

C#:   if (data == null) return;
来源：http://fxn.ywan-chungtsiang.top

================================================================================
来源：http://zcx.epnwcf.com

C. 函数与作用域
来源：http://emg.ybcxt.top

================================================================================
来源：http://gac.yvedp.cn

[C01] 定义函数
来源：http://qvu.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://ssz.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fxp.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://dlp.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jyk.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qyq.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://pxo.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://ejn.yj20258.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dpm.ctjpmb.com

[C02] 默认参数
来源：http://bpa.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://ndo.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://evz.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://nat.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bxv.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cze.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yef.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://cmg.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://fao.tian-w.cn

[C03] 可变参数
来源：http://ddd.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://chp.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tin.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pcx.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gpf.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://owe.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zpq.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wtw.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lmr.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://rsl.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://guh.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xee.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qbi.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mzy.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://tta.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://ach.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://qpz.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://idm.gzhubu.top

[C05] 返回多个值
来源：http://brm.jinqigfzy.top

Py:   return a, b
来源：http://ubf.yangfankeji.com

PHP:  return [$a, $b];
来源：http://dzd.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vzj.hesvh.cn

TS:   return { a, b };
来源：http://zli.havefunace.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dgf.guannengcc.top

Go:   return a, b
来源：http://egb.jinghuilouyu.cn

Ruby: return a, b
来源：http://kjr.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://yly.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://ihj.wangdashe.top

Py:   square = lambda x: x * x
来源：http://cly.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wtc.epnwcf.com

JS:   const square = x => x * x;
来源：http://fqv.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://gnt.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ueg.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://ecv.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://bcm.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://oxm.jinyuanbaomall.cn

[C07] 把函数作为参数传入
来源：http://ibw.cashguo.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pcq.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://puo.chenjidiqi.icu


<!-- 参考信息 -->