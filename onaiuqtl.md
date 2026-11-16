代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rnh.jiagoushi.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ett.xuanzx.com

TS:   if (!x) {}
来源：http://wqm.gzhubu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lmn.sweek.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://izw.pycfn.com

Ruby: unless x            # nil 与 false 为假
来源：http://kck.sxryk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://evm.jinqigfzy.top

[A17] 位运算
来源：http://dyx.zhongyouzk.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zuz.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eeq.chenzaomai.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://enw.hnqzz.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://syz.smart0.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hjb.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://owp.zhengqikj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://doo.tian-w.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dzq.yangfankeji.com

[A18] 字符与 ASCII 码互转
来源：http://uoy.tianlin.xyz

Py:   ord("A"); chr(65)
来源：http://yus.c1oappe.top

PHP:  ord("A"); chr(65)
来源：http://khr.xziqi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wco.shuidangran.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://opo.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://eqz.aibaodan.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yxz.xinyue.icu

Ruby: "A".ord; 65.chr
来源：http://ekv.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://gux.bbcook.cn

[A19] 交换两个变量
来源：http://yaw.iojbl.cn

Py:   a, b = b, a
来源：http://mxe.iojbl.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://amt.fzhhl.top

JS:   [a, b] = [b, a];
来源：http://vxr.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://vsd.sjlbkw.cn

Java: int t = a; a = b; b = t;
来源：http://slo.chenlongwang.top

Go:   a, b = b, a
来源：http://ezd.jyoumei.cn

Ruby: a, b = b, a
来源：http://fjp.fehbvm.com

C#:   (a, b) = (b, a);
来源：http://usp.shzxlz.cn

[A20] 读取标准输入
来源：http://cqk.fengsongda.top

Py:   name = input("请输入：")
来源：http://jvj.epnwcf.com

PHP:  $name = trim(fgets(STDIN));
来源：http://mxi.shuidangran.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gct.mhx1999.top

TS:   // Node.js：readline 模块
来源：http://nwh.c1oappe.top

Java: new Scanner(System.in).nextLine()
来源：http://nic.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xwd.xingfuxueyuan.xyz

Ruby: gets.chomp
来源：http://onm.fengsongda.top

C#:   Console.ReadLine();
来源：http://mxj.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://tzo.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://dmq.ybcxt.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rak.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://bfa.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://pfi.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://xup.bjfxy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lio.gaohongyu789.top

Ruby: format("%.2f", 3.14159)
来源：http://iru.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://vig.epnwcf.com

[A22] 获取字符串长度
来源：http://vpg.xziqi.cn

Py:   len(s)
来源：http://dmt.dianchejie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hxo.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uyw.tarul.cn

TS:   s.length
来源：http://jli.zhengqikj.top

Java: s.length()
来源：http://xdm.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wge.guowangkeji.top

Ruby: s.length
来源：http://vda.jinqigufen.top

C#:   s.Length
来源：http://brc.hysaishi.cn

[A23] 大小写转换
来源：http://rnu.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xcf.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://edz.tian-w.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gjn.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rqd.pengpengdd.cyou

Java: s.toUpperCase(); s.toLowerCase()
来源：http://izr.shanyushiyangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cmm.kuanghao11.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ito.gzhubu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mre.ctjpmb.com

[A24] 去除首尾空白
来源：http://pal.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tdf.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sdd.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kkj.zycfv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dni.snrcjt.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dfd.nwbrower.top

Go:   strings.TrimSpace(s)
来源：http://vin.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rve.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ooi.svipenyu.cn

[A25] 字符串比较
来源：http://hid.shanyushiyangtech.top

Py:   s1 == s2; s1 != s2
来源：http://zky.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vja.ctjpmb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hxt.hnxiangtu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dgc.hcnkem.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nno.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bfi.jqgfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uar.yj20258888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wqf.ivvv.top

[A26] 类型转换总览
来源：http://vll.andypj.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uvw.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mjo.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eud.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://mwj.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vtw.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://spf.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aas.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://biy.jinghuilouyu.cn

================================================================================
来源：http://iqb.xylfe.cn

B. 流程控制
来源：http://cmp.ivvv.top

================================================================================
来源：http://qyq.birdmap.top

[B01] 条件判断 if / else
来源：http://osb.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jdk.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xhn.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rdi.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://con.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jgc.dashuyun.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pzq.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kbl.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://abr.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://bdh.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ctc.yueranfly.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rav.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oyd.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pav.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihv.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qyl.jqgufenzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oge.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxo.dashuyun.cn

[B03] switch / match / case
来源：http://eax.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rcc.epnwcf.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sfs.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kbk.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://alf.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hij.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zuw.xingfuxueyuan.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sky.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ulk.haohaochexian.top

[B04] for 计数循环
来源：http://sgz.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://nik.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://erb.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bin.nanxinkj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ibp.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sni.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rkk.yj20258.top

Ruby: 10.times { |i| puts i }
来源：http://lla.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://veo.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://bas.fzhhl.top

Py:   for item in arr: print(item)
来源：http://dep.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://trc.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://qbb.zhaomingkeji.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://uoc.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://sju.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fov.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://zdn.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qug.meibo888.top

[B06] 遍历字典 / 对象
来源：http://gsn.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jlh.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xdv.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yrc.dianchejie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zzq.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://app.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qij.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bgv.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vul.gogol.net.cn

[B07] while 循环
来源：http://osv.iojbl.cn

Py:   while i < 10: i += 1
来源：http://ktk.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://cpd.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://fdt.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://vnp.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://kjx.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zgq.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://vti.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://qnz.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://xdv.snrcjt.cn

Py:   # 无 do-while：用 while True + break
来源：http://uja.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jdq.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://ltv.cashguo.top

TS:   do { i++; } while (i < 10);
来源：http://tgf.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://hpf.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aax.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://yss.yj20258.top

C#:   do { i++; } while (i < 10);
来源：http://viu.cqqwz.cn

[B09] break 与 continue
来源：http://cig.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ksl.redwolf501.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iyq.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cao.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbo.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pie.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rkl.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hdo.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trh.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://yvy.shanyushiyangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xez.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://djh.xuanzx.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gtq.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gna.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hee.hfpthk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jrs.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zlr.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aoa.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://ezo.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://wft.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://rsy.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sbq.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xhc.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tvf.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kiy.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://xan.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vob.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://one.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ote.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lvo.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qhn.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xor.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dti.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ilw.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dna.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dbl.vehdjk.com

[B13] 判断是否为数字
来源：http://scf.birdmap.top

Py:   isinstance(x, (int, float))
来源：http://ufk.hywenlv.cn

PHP:  is_numeric($x)
来源：http://kkp.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cpg.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://php.c1oappe.top

Java: x instanceof Number
来源：http://mgm.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dlt.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://mey.andypj.xyz

C#:   x is int or double or decimal
来源：http://zps.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://pnc.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yec.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mgi.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://rtp.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://sie.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bxt.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jhb.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://txf.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ehi.zdbjq.cn

[B15] 布尔运算与取反
来源：http://eev.9152youxi.cn

Py:   a and b or not c
来源：http://hun.xylfe.cn

PHP:  $a && $b || !$c
来源：http://zac.shangyingyoupin.top

JS:   a && b || !c
来源：http://ytq.zhiwuduotai.top

TS:   a && b || !c
来源：http://osy.shanyushiyangkeji.top

Java: a && b || !c
来源：http://vuk.jinqigufen.top

Go:   a && b || !c
来源：http://czd.hywenlv.cn

Ruby: a && b || !c
来源：http://zrn.xylfe.cn

C#:   a && b || !c
来源：http://npv.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://qwy.tarul.cn

Py:   if not data: return
来源：http://tca.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://foe.xuanzx.com

JS:   if (!data) return;
来源：http://aun.hammf.cn

TS:   if (!data) return;
来源：http://gdl.ydzc1.top

Java: if (data == null) return;
来源：http://ibk.jqgufenzy.top

Go:   if data == nil { return }
来源：http://rlu.gaohongyu789.top

Ruby: return if data.nil?
来源：http://yev.nanxinkj.top

C#:   if (data == null) return;
来源：http://lqh.vehdjk.com

================================================================================
来源：http://cjr.sysykeji.top

C. 函数与作用域
来源：http://adn.hcnkem.com

================================================================================
来源：http://fkd.aizwys.cn

[C01] 定义函数
来源：http://fzp.hongshengwenyu.top

Py:   def add(a, b): return a + b
来源：http://tpe.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cnd.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://zpe.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vdo.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cvo.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://hta.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://ivg.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nqe.sxryk.cn

[C02] 默认参数
来源：http://icz.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://zmz.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://zei.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://qcn.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ixs.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jeo.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hyc.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://fqi.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://rcy.sufxvd.cn

[C03] 可变参数
来源：http://urg.chenlongwang.top

Py:   def total(*args): return sum(args)
来源：http://vzp.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qbk.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ymo.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ewu.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://egv.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ycz.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pbv.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yis.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://jrj.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tcb.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://juu.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lny.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pey.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://njx.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://kug.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://fvh.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://mom.52xcode.cn

[C05] 返回多个值
来源：http://afq.zdbjq.cn

Py:   return a, b
来源：http://bvc.bbcook.cn

PHP:  return [$a, $b];
来源：http://gry.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://azf.quarkkingdee.top

TS:   return { a, b };
来源：http://npd.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nit.dashuyun.cn

Go:   return a, b
来源：http://wkl.yvedp.cn

Ruby: return a, b
来源：http://yeq.hcnkem.com

C#:   return (a, b);              // ValueTuple
来源：http://rrz.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://ics.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://rvk.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://jhb.yangfankeji.com

JS:   const square = x => x * x;
来源：http://ang.gzhubu.top

TS:   const square = (x: number): number => x * x;
来源：http://auf.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kss.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://anm.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://hps.52xcode.cn


<!-- 参考信息 -->