代发 wailian999

Ruby: value = data || "默认值"
来源：http://sxl.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://pol.cheryme.top

[A16] 真假值判断规则
来源：http://fbj.zhiwuduotai.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wbc.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://anc.zdbjq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rgc.fanxiaobao.xyz

TS:   if (!x) {}
来源：http://yae.jinqigufen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yaq.meibo888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bhb.ydzc1.top

Ruby: unless x            # nil 与 false 为假
来源：http://vby.vehdjk.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xky.kuanghao11.cn

[A17] 位运算
来源：http://whf.sxryk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jzj.yuanzhike.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nvz.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://twz.daxiang520.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uje.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://klb.zdbjq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gcv.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uxh.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lkv.fengsongda.top

[A18] 字符与 ASCII 码互转
来源：http://hbx.fktsv.cn

Py:   ord("A"); chr(65)
来源：http://ygu.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://adr.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://elo.chenzaomai.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vmy.shanyushiyangkeji.top

Java: (int) 'A'; (char) 65
来源：http://fah.cashguo.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://trv.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://tjw.ivvv.top

C#:   (int)'A'; (char)65
来源：http://tiy.bjfxy.top

[A19] 交换两个变量
来源：http://zaa.pycfn.com

Py:   a, b = b, a
来源：http://dqd.uphjek.com

PHP:  [$a, $b] = [$b, $a];
来源：http://sqd.yonumen.top

JS:   [a, b] = [b, a];
来源：http://jvk.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://dcr.epnwcf.com

Java: int t = a; a = b; b = t;
来源：http://zur.xingfuxueyuan.xyz

Go:   a, b = b, a
来源：http://lmu.tanke756.top

Ruby: a, b = b, a
来源：http://inf.yuanzhike.top

C#:   (a, b) = (b, a);
来源：http://jmb.fzhhl.top

[A20] 读取标准输入
来源：http://tal.tarul.cn

Py:   name = input("请输入：")
来源：http://nsq.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wmy.jinqigufen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lkf.pycfn.com

TS:   // Node.js：readline 模块
来源：http://ifo.sweek.top

Java: new Scanner(System.in).nextLine()
来源：http://qcj.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xri.tanke756.top

Ruby: gets.chomp
来源：http://guq.fzhhl.top

C#:   Console.ReadLine();
来源：http://mkx.xinyue.icu

[A21] 保留指定小数位输出
来源：http://pdq.shangyingyoupin.top

Py:   f"{3.14159:.2f}"
来源：http://icv.ybcxt.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ibw.birdmap.top

JS:   (3.14159).toFixed(2)
来源：http://awb.sufxvd.cn

TS:   (3.14159).toFixed(2)
来源：http://gyk.fanxiaobao.xyz

Java: String.format("%.2f", 3.14159)
来源：http://get.dianchejie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kwb.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://zpx.guowangkeji.top

C#:   3.14159.ToString("F2")
来源：http://xhl.tanke756.top

[A22] 获取字符串长度
来源：http://bbo.fanxiaobao.xyz

Py:   len(s)
来源：http://vwl.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bby.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cru.yuxming.cn

TS:   s.length
来源：http://isr.ydjk.org.cn

Java: s.length()
来源：http://pzc.redwolf501.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://knn.jqgufenzy.top

Ruby: s.length
来源：http://llo.ctjpmb.com

C#:   s.Length
来源：http://dur.snrcjt.cn

[A23] 大小写转换
来源：http://ekf.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hre.yonumen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iur.zycfv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cep.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dql.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cvu.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gsu.cashguo.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kcu.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://leu.yj20258888.top

[A24] 去除首尾空白
来源：http://usl.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iyr.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tbw.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dra.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ksb.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wdi.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://cuj.zdqjudy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iee.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zxb.hysaishi.cn

[A25] 字符串比较
来源：http://fya.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://gan.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sqm.zhijiandao.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://khj.jianghu66.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dnt.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qzn.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hil.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lbc.chenzaomai.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bxc.fehbvm.com

[A26] 类型转换总览
来源：http://azp.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://izy.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vmf.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fgx.jlsjyb.cn

TS:   Number() String() Boolean() x as number
来源：http://smu.zhoulong.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ytg.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qqf.svipenyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gdo.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bht.sysykeji.top

================================================================================
来源：http://grk.sufxvd.cn

B. 流程控制
来源：http://vpx.cdnleiting.top

================================================================================
来源：http://dft.daria6918.cn

[B01] 条件判断 if / else
来源：http://pob.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cpm.jqgufenzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vgx.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ndz.epnwcf.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://swn.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pkv.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hsc.daria6918.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pqn.jianghu66.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ele.fktsv.cn

[B02] 多分支 else if / elif
来源：http://lhg.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mei.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://apv.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xzu.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gem.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fxl.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kos.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://euc.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wof.havefunace.top

[B03] switch / match / case
来源：http://kgy.hysaishi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hzd.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pik.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rfi.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qhm.ehwqpu.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fen.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gcn.yangfankeji.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xle.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jfd.yj20258.top

[B04] for 计数循环
来源：http://njj.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://eex.aibaodan.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kvt.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wrc.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zyk.gogol.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gew.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eoa.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://xcl.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hvs.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://cqe.guannengcc.top

Py:   for item in arr: print(item)
来源：http://fsi.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iet.yanxiufei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qpp.aizwys.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yis.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fbg.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hxb.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://rkb.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dzk.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://ybg.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dec.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fnl.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zzm.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rda.tarul.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wwx.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://opb.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://juh.fengsongda.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zoi.yangfankeji.com

[B07] while 循环
来源：http://jda.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://jyi.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://znl.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://job.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://kdd.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://wow.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nww.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://ubu.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://dth.yj202588.top

[B08] do-while（至少执行一次）
来源：http://jkb.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://sdl.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jsy.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://dtx.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://gus.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://jbw.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pqr.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://mfz.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://wue.hesvh.cn

[B09] break 与 continue
来源：http://ybe.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cvp.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xfc.sjlbkw.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhc.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://itp.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iky.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ubz.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eiy.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://adw.xuanzx.com

[B10] 遍历同时拿索引
来源：http://rzo.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jgw.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vrz.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://icd.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jpa.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gng.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://stk.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iip.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://suw.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://zzw.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://yym.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://igo.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eta.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lrp.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nrd.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tsc.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://sxm.wangshuangyany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aqr.cdnleiting.top

[B12] 跳出多层循环
来源：http://fxh.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ifr.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zgt.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://npv.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wld.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rhi.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ynw.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cqg.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bny.xylfe.cn

[B13] 判断是否为数字
来源：http://aec.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://ada.yuanzhike.top

PHP:  is_numeric($x)
来源：http://gsv.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zrz.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ghk.haohaochexian.top

Java: x instanceof Number
来源：http://qyn.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oca.shanyushiyangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://cvi.sxryk.cn

C#:   x is int or double or decimal
来源：http://kvv.hcnkem.com

[B14] 判断值是否在集合内
来源：http://etp.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mge.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vqa.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://zvz.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://kam.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://mcn.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ljz.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://rvz.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gun.bjfxy.top

[B15] 布尔运算与取反
来源：http://iok.andypj.xyz

Py:   a and b or not c
来源：http://sep.yj20258.top

PHP:  $a && $b || !$c
来源：http://kwr.bbcook.cn

JS:   a && b || !c
来源：http://sou.fehbvm.com

TS:   a && b || !c
来源：http://pxq.quarkkingdee.top

Java: a && b || !c
来源：http://xgr.hnqzz.top

Go:   a && b || !c
来源：http://vfv.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://djh.shzxlz.cn

C#:   a && b || !c
来源：http://une.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sbi.zycfv.cn

Py:   if not data: return
来源：http://bbi.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://obf.ivvv.top

JS:   if (!data) return;
来源：http://oxq.jqgufenzy.top

TS:   if (!data) return;
来源：http://xuj.pengpengdd.cyou

Java: if (data == null) return;
来源：http://vsd.ydzc1.top

Go:   if data == nil { return }
来源：http://bbk.xylfe.cn

Ruby: return if data.nil?
来源：http://fve.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://rft.hammf.cn

================================================================================
来源：http://mxy.yanxiufei.cn

C. 函数与作用域
来源：http://hpd.zhixingplan.top

================================================================================
来源：http://sdb.yueranfly.top

[C01] 定义函数
来源：http://vfh.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://qxy.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fcy.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://dzl.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uhw.xingfuxueyuan.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://nda.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oeu.ybcxt.top

Ruby: def add(a, b); a + b; end
来源：http://ons.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://shx.gotoacloud.top

[C02] 默认参数
来源：http://jdi.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://ctp.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://cua.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://ayu.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vxo.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pio.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eab.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://vbq.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://kwa.daxiang520.top

[C03] 可变参数
来源：http://fda.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://zqk.hnxiangtu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sjq.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aay.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hkb.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rhx.fehbvm.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rip.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://sbp.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xso.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://fzp.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ept.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://duu.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pkt.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://umi.hnxiangtu.top

Java: // 无：用 Builder 模式或 record
来源：http://tpk.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://yhc.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://gpe.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://ukm.fengsongda.top

[C05] 返回多个值
来源：http://gtd.havefunace.top

Py:   return a, b
来源：http://nsg.aibaodan.cn

PHP:  return [$a, $b];
来源：http://nvv.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cti.cashguo.top

TS:   return { a, b };
来源：http://nui.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zdw.yuxming.cn

Go:   return a, b
来源：http://ybi.hcnkem.com

Ruby: return a, b
来源：http://hde.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://pkr.birdmap.top

[C06] 匿名函数 / lambda
来源：http://rzs.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://iqb.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dhy.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://jdy.guannengcc.top


<!-- 参考信息 -->