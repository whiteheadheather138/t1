代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://enz.ctjpmb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vye.zhengqikj.top

TS:   if (!x) {}
来源：http://kch.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://opm.ivvv.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://usq.iojbl.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dho.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bpe.iojbl.cn

[A17] 位运算
来源：http://rnk.dashuyun.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bek.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://epg.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ina.yj20258.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fbe.fktsv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eut.hnqzz.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ozl.birdmap.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mhk.sjlbkw.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykb.chenlongwang.top

[A18] 字符与 ASCII 码互转
来源：http://cvt.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://bxe.0kj1m.cn

PHP:  ord("A"); chr(65)
来源：http://fbc.zycfv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vcj.xylfe.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vli.yj202588.top

Java: (int) 'A'; (char) 65
来源：http://tva.yuxming.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pfm.zhixingplan.top

Ruby: "A".ord; 65.chr
来源：http://yjy.havefunace.top

C#:   (int)'A'; (char)65
来源：http://jgi.zhongyouzk.top

[A19] 交换两个变量
来源：http://gmo.jinqigufen.top

Py:   a, b = b, a
来源：http://uhs.zhongyouzk.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nge.yonumen.top

JS:   [a, b] = [b, a];
来源：http://ggp.hesvh.cn

TS:   [a, b] = [b, a];
来源：http://ziu.jiagoushi.top

Java: int t = a; a = b; b = t;
来源：http://vyb.0kj1m.cn

Go:   a, b = b, a
来源：http://jij.yvedp.cn

Ruby: a, b = b, a
来源：http://jke.tianlin.xyz

C#:   (a, b) = (b, a);
来源：http://hpb.sjlbkw.cn

[A20] 读取标准输入
来源：http://fhu.daxiang520.top

Py:   name = input("请输入：")
来源：http://zzu.nanxinkj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zip.andypj.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zzv.yuxming.cn

TS:   // Node.js：readline 模块
来源：http://ink.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://ogx.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://glx.52xcode.cn

Ruby: gets.chomp
来源：http://dfl.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://cnb.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://qeb.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://cba.fzhhl.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://laa.zycfv.cn

JS:   (3.14159).toFixed(2)
来源：http://qnb.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://obq.zhongyouzk.top

Java: String.format("%.2f", 3.14159)
来源：http://hqf.meibo888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nao.quarkkingdee.top

Ruby: format("%.2f", 3.14159)
来源：http://frd.xinyue.icu

C#:   3.14159.ToString("F2")
来源：http://wqi.shuidangran.top

[A22] 获取字符串长度
来源：http://cse.gogol.net.cn

Py:   len(s)
来源：http://kxc.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fjh.hysaishi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ryx.ydzc1.top

TS:   s.length
来源：http://lqh.chenlongwang.top

Java: s.length()
来源：http://vgu.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ntl.ywan-chungtsiang.top

Ruby: s.length
来源：http://pdc.zdqjudy.top

C#:   s.Length
来源：http://okh.yj20258.top

[A23] 大小写转换
来源：http://bfz.yongpay.top

Py:   s.upper(); s.lower(); s.title()
来源：http://reg.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kmq.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ttq.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bka.yj20258888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pia.daria6918.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://euh.snrcjt.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uze.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ohu.andypj.xyz

[A24] 去除首尾空白
来源：http://omd.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ndx.hcnkem.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gyn.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cxs.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dtt.aibaodan.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://abl.snrcjt.cn

Go:   strings.TrimSpace(s)
来源：http://uld.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fmq.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fde.jqgfzy.top

[A25] 字符串比较
来源：http://jut.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://joj.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ofv.ehwqpu.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ylh.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fhh.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://waz.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gfr.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dyi.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://brm.smart0.xyz

[A26] 类型转换总览
来源：http://ifk.vehdjk.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://whq.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vfj.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lii.jianghu66.top

TS:   Number() String() Boolean() x as number
来源：http://ekx.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sld.cheryme.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oiq.guowangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hag.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xzo.nanxuanxn.top

================================================================================
来源：http://pjg.svipenyu.cn

B. 流程控制
来源：http://pmp.hfpthk.cn

================================================================================
来源：http://tjo.gzhubu.top

[B01] 条件判断 if / else
来源：http://neb.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://wem.tanke756.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yrc.ivvv.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qfw.mhx1999.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qge.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hdz.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://csd.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pei.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://asr.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://lfx.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wzh.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oeu.uphjek.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tkk.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zuf.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mis.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lar.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nca.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pds.fktsv.cn

[B03] switch / match / case
来源：http://tfr.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lpg.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vqz.hnqzz.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://apu.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cvb.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mbp.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hjf.hysaishi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vgi.pycfn.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dym.sxryk.cn

[B04] for 计数循环
来源：http://wcz.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://svq.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kry.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hop.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jnl.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fwj.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xdk.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://kve.vehdjk.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://are.tarul.cn

[B05] 遍历数组 / 列表
来源：http://crl.fktsv.cn

Py:   for item in arr: print(item)
来源：http://ray.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eyx.xingfuxueyuan.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://sws.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://orx.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://buu.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hdf.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://wml.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sbv.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://yta.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ixa.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tkj.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nil.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kwz.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lnd.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bme.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eke.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ytx.svipenyu.cn

[B07] while 循环
来源：http://ydv.bbcook.cn

Py:   while i < 10: i += 1
来源：http://yrd.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://hbd.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://abi.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://jih.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://fgr.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fko.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://btw.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://krl.fanxiaobao.xyz

[B08] do-while（至少执行一次）
来源：http://etd.yuanzhike.top

Py:   # 无 do-while：用 while True + break
来源：http://nfr.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kib.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://hbw.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://gxz.zhiwuduotai.top

Java: do { i++; } while (i < 10);
来源：http://ckk.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fex.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mhc.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://car.kuanghao11.cn

[B09] break 与 continue
来源：http://iwo.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://enz.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zps.smart0.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozo.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sgk.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyt.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ujs.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gnu.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qqv.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://ytf.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hpd.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jvo.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://prh.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tfu.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xil.ehwqpu.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bpp.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://top.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fzr.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://jmm.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://myg.ivvv.top

PHP:  range(0, 10, 2);
来源：http://kuo.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sug.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aie.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uhl.ydzc1.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wvj.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://fbn.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ozd.svipenyu.cn

[B12] 跳出多层循环
来源：http://sfa.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fvu.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://skv.zycfv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zmu.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://asn.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://syx.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://igs.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fpl.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zxk.chenlongwang.top

[B13] 判断是否为数字
来源：http://szn.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://zos.sxryk.cn

PHP:  is_numeric($x)
来源：http://dam.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://azy.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ora.zdqjudy.top

Java: x instanceof Number
来源：http://hdz.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://azx.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://vwo.snrcjt.cn

C#:   x is int or double or decimal
来源：http://owu.yueranfly.top

[B14] 判断值是否在集合内
来源：http://dwg.sweek.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://isu.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qza.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://olw.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://aks.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rqb.wangshuangyany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qfz.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://udm.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://acr.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://cvu.yfazqb.com

Py:   a and b or not c
来源：http://xoq.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://cva.0kj1m.cn

JS:   a && b || !c
来源：http://xuq.iojbl.cn

TS:   a && b || !c
来源：http://jat.daria6918.cn

Java: a && b || !c
来源：http://ooo.haohaochexian.top

Go:   a && b || !c
来源：http://jno.c1oappe.top

Ruby: a && b || !c
来源：http://lnc.epnwcf.com

C#:   a && b || !c
来源：http://fny.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eva.yj20258888.top

Py:   if not data: return
来源：http://oot.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://fle.yangfankeji.com

JS:   if (!data) return;
来源：http://qtp.jiagoushi.top

TS:   if (!data) return;
来源：http://sou.cqqwz.cn

Java: if (data == null) return;
来源：http://cck.nanxuanxn.top

Go:   if data == nil { return }
来源：http://hcr.yfazqb.com

Ruby: return if data.nil?
来源：http://hrm.gogol.net.cn

C#:   if (data == null) return;
来源：http://xjo.sweek.top

================================================================================
来源：http://eqq.sjlbkw.cn

C. 函数与作用域
来源：http://jpn.xingfuxueyuan.xyz

================================================================================
来源：http://uyc.ybcxt.top

[C01] 定义函数
来源：http://elj.hesvh.cn

Py:   def add(a, b): return a + b
来源：http://dgd.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zvv.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://izy.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pqp.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jvg.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://tii.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://ivk.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qor.hnxiangtu.top

[C02] 默认参数
来源：http://svc.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://gpp.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oex.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://nmk.cdnleiting.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zmf.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cuj.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lyl.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://psq.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://dun.vqdsnc.cn

[C03] 可变参数
来源：http://ecr.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://pzw.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aeb.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://run.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ihd.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ahd.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rpk.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hpk.jyoumei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ueg.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://okc.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nct.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vpj.shangyingyoupin.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lkp.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kke.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://qys.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://gvd.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://izw.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://qsh.yonumen.top

[C05] 返回多个值
来源：http://zas.jqgufenzy.top

Py:   return a, b
来源：http://ojb.yuxming.cn

PHP:  return [$a, $b];
来源：http://zgb.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ylj.hnqzz.top

TS:   return { a, b };
来源：http://cus.cashguo.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kko.fehbvm.com

Go:   return a, b
来源：http://fak.ydjk.org.cn

Ruby: return a, b
来源：http://qtf.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://blt.hfpthk.cn

[C06] 匿名函数 / lambda
来源：http://bww.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://rxl.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bhz.xuanzx.com

JS:   const square = x => x * x;
来源：http://pgf.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://urf.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wtc.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ava.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://pmx.sxryk.cn


<!-- 参考信息 -->