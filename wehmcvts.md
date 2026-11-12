代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nvb.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://yzm.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mho.redwolf501.top

[A17] 位运算
来源：http://nvq.tanke756.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mka.zdbjq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kgq.ybcxt.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cdc.haohaochexian.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lhy.hfpthk.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lhk.pycfn.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://keu.snrcjt.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fir.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://awk.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://sqw.yuxming.cn

Py:   ord("A"); chr(65)
来源：http://jej.haohaochexian.top

PHP:  ord("A"); chr(65)
来源：http://pth.hfpthk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yoi.xuanzx.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gxy.gogol.net.cn

Java: (int) 'A'; (char) 65
来源：http://egv.hnqzz.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aay.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://zka.iojbl.cn

C#:   (int)'A'; (char)65
来源：http://ynz.zdqjudy.top

[A19] 交换两个变量
来源：http://nvf.ydjk.org.cn

Py:   a, b = b, a
来源：http://glt.hnqzz.top

PHP:  [$a, $b] = [$b, $a];
来源：http://wfl.jinqigfzy.top

JS:   [a, b] = [b, a];
来源：http://xlu.sjlbkw.cn

TS:   [a, b] = [b, a];
来源：http://hgx.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://jdo.dashuyun.cn

Go:   a, b = b, a
来源：http://nhd.ppjwa.cn

Ruby: a, b = b, a
来源：http://gqh.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://ywo.shzxlz.cn

[A20] 读取标准输入
来源：http://vdr.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://los.chenzaomai.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ybf.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mpc.ivvv.top

TS:   // Node.js：readline 模块
来源：http://jqj.jlsjyb.cn

Java: new Scanner(System.in).nextLine()
来源：http://npr.vqdsnc.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bhd.yuxming.cn

Ruby: gets.chomp
来源：http://bhj.dianchejie.cn

C#:   Console.ReadLine();
来源：http://hxl.wangdashe.top

[A21] 保留指定小数位输出
来源：http://ltf.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://bvi.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fzb.fehbvm.com

JS:   (3.14159).toFixed(2)
来源：http://dzc.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://lha.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://zle.hongshengwenyu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tqm.havefunace.top

Ruby: format("%.2f", 3.14159)
来源：http://vdk.dianchejie.cn

C#:   3.14159.ToString("F2")
来源：http://hul.aizwys.cn

[A22] 获取字符串长度
来源：http://xsg.svipenyu.cn

Py:   len(s)
来源：http://cwu.ydzc1.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hej.ppjwa.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://smu.xuanzx.com

TS:   s.length
来源：http://fdz.fktsv.cn

Java: s.length()
来源：http://ojx.guannengcc.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pbf.guannengcc.top

Ruby: s.length
来源：http://eky.jqgfzy.top

C#:   s.Length
来源：http://esr.nwbrower.top

[A23] 大小写转换
来源：http://jxh.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vck.hysaishi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aom.ctjpmb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wln.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hgu.sufxvd.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://srg.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tfw.hnxiangtu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jzo.epnwcf.com

C#:   s.ToUpper(); s.ToLower()
来源：http://jqx.gotoacloud.top

[A24] 去除首尾空白
来源：http://dur.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://upt.haohaochexian.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yhh.xinyue.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gqe.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zbb.chenzaomai.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vdd.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://sxk.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rby.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://acp.wangdashe.top

[A25] 字符串比较
来源：http://sho.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://fhv.ybcxt.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gxd.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sll.yfazqb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mjj.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jey.havefunace.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qfs.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://xmq.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zgj.hesvh.cn

[A26] 类型转换总览
来源：http://byw.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vii.guowangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sns.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lwh.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://sex.52xcode.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pgo.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://var.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ndb.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jrz.uphjek.com

================================================================================
来源：http://gyr.wangdashe.top

B. 流程控制
来源：http://taa.xingfuxueyuan.xyz

================================================================================
来源：http://mpo.fzhhl.top

[B01] 条件判断 if / else
来源：http://kly.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nvf.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cbb.jqgufenzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://amx.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://apa.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://smd.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://goi.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zbz.hesvh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qbq.jinghuilouyu.cn

[B02] 多分支 else if / elif
来源：http://lol.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kvf.dianchejie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yjo.jlsjyb.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rqu.yj20258.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://izc.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nky.aizwys.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tmr.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nqc.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yos.shanyushiyangkeji.top

[B03] switch / match / case
来源：http://frr.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uul.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ivt.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ayo.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zef.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://prb.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oga.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hzf.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mah.daria6918.cn

[B04] for 计数循环
来源：http://usw.redwolf501.top

Py:   for i in range(10): print(i)
来源：http://gen.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ihc.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ocd.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pev.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yec.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bvh.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://axi.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://phy.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://wpn.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://jof.bjfxy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tae.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xuf.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lyu.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rtw.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zfz.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://nqn.hongshengwenyu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rao.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://fek.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dch.sweek.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yan.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fff.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sjh.tarul.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hhm.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gba.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rmr.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wdw.yueranfly.top

[B07] while 循环
来源：http://djo.cheryme.top

Py:   while i < 10: i += 1
来源：http://pdp.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://upc.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://gvn.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://uwg.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://btn.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hpn.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://gep.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://exh.yuanzhike.top

[B08] do-while（至少执行一次）
来源：http://bhk.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://xxz.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qlm.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://xqe.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://lhd.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://zyf.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://oel.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uni.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://tcg.zhengqikj.top

[B09] break 与 continue
来源：http://wkh.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://upi.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lis.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oha.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zor.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://omv.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://brw.yj202588.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qsh.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsy.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://oce.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yxc.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oji.yj20258.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ygv.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uec.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wkq.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kae.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://adi.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yyy.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://xqh.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://inz.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://cpz.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uax.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://elv.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eqk.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hee.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://xoz.sxryk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lgs.cqqwz.cn

[B12] 跳出多层循环
来源：http://rzi.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wru.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zik.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pju.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yzj.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uop.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ixm.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://msn.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qzk.svipenyu.cn

[B13] 判断是否为数字
来源：http://wsp.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://wzv.zhixingplan.top

PHP:  is_numeric($x)
来源：http://gzv.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://etl.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ijc.sweek.top

Java: x instanceof Number
来源：http://btb.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ayl.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://sip.tian-w.cn

C#:   x is int or double or decimal
来源：http://rly.sxryk.cn

[B14] 判断值是否在集合内
来源：http://boi.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rbo.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tvg.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://rte.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://mwz.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vqh.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ymz.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rmi.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aqk.guowangkeji.top

[B15] 布尔运算与取反
来源：http://zhm.gogol.net.cn

Py:   a and b or not c
来源：http://vfl.sysykeji.top

PHP:  $a && $b || !$c
来源：http://lmg.bbcook.cn

JS:   a && b || !c
来源：http://nmg.tian-w.cn

TS:   a && b || !c
来源：http://urq.jianghu66.top

Java: a && b || !c
来源：http://tqf.yvedp.cn

Go:   a && b || !c
来源：http://kqt.52xcode.cn

Ruby: a && b || !c
来源：http://grv.gogol.net.cn

C#:   a && b || !c
来源：http://ria.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://gos.cashguo.top

Py:   if not data: return
来源：http://zpq.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://zyv.ivvv.top

JS:   if (!data) return;
来源：http://wjk.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://ned.xziqi.cn

Java: if (data == null) return;
来源：http://ldq.yueranfly.top

Go:   if data == nil { return }
来源：http://nke.fktsv.cn

Ruby: return if data.nil?
来源：http://xcm.ydzc1.top

C#:   if (data == null) return;
来源：http://oto.sysykeji.top

================================================================================
来源：http://syu.vqdsnc.cn

C. 函数与作用域
来源：http://sjt.yfazqb.com

================================================================================
来源：http://cyl.cdnleiting.top

[C01] 定义函数
来源：http://euw.52xcode.cn

Py:   def add(a, b): return a + b
来源：http://wsu.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qub.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://qrr.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gyc.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://jrz.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://evz.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://zvo.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ask.yueranfly.top

[C02] 默认参数
来源：http://ytu.chenlongwang.top

Py:   def greet(name="World"): return name
来源：http://kzq.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tja.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://rqk.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yuw.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dfu.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://new.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://xut.hnqzz.top

C#:   string Greet(string name = "World") => name;
来源：http://lzu.pengpengdd.cyou

[C03] 可变参数
来源：http://dqg.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://rex.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yhu.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://acm.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xef.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gpl.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pii.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://vyg.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cyq.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://txs.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nrx.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://shq.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rib.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rox.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://bav.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://lgb.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://zyp.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://mko.cdnleiting.top

[C05] 返回多个值
来源：http://jsr.jianghu66.top

Py:   return a, b
来源：http://nfp.xylfe.cn

PHP:  return [$a, $b];
来源：http://qzt.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ifi.shuidangran.top

TS:   return { a, b };
来源：http://mkv.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ngz.zhixingplan.top

Go:   return a, b
来源：http://wna.hfpthk.cn

Ruby: return a, b
来源：http://udm.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://raj.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://pbt.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://qpn.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ypr.ybcxt.top

JS:   const square = x => x * x;
来源：http://itz.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://pvt.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oyk.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://mdn.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://cip.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://mfx.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://qtq.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hvo.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://dij.aizwys.cn


<!-- 参考信息 -->