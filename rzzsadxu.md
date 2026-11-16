代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lxe.sxryk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://naz.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hzo.hnqzz.top

[A17] 位运算
来源：http://qsl.cashguo.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oba.gotoacloud.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://aml.vqdsnc.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ajj.0kj1m.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qxq.yanxiufei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tjx.jinqigufen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://riy.jlsjyb.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ina.zhijiandao.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jrf.sufxvd.cn

[A18] 字符与 ASCII 码互转
来源：http://saz.jlsjyb.cn

Py:   ord("A"); chr(65)
来源：http://pij.hesvh.cn

PHP:  ord("A"); chr(65)
来源：http://tmg.tanke756.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://unv.xuetiantiany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jac.hammf.cn

Java: (int) 'A'; (char) 65
来源：http://ovr.zdbjq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://phr.hfpthk.cn

Ruby: "A".ord; 65.chr
来源：http://wmi.fengsongda.top

C#:   (int)'A'; (char)65
来源：http://gtm.gzhubu.top

[A19] 交换两个变量
来源：http://kur.nanxuanxn.top

Py:   a, b = b, a
来源：http://tay.bbcook.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ifr.yj20258.top

JS:   [a, b] = [b, a];
来源：http://dzz.yueranfly.top

TS:   [a, b] = [b, a];
来源：http://gog.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://xwn.aibaodan.cn

Go:   a, b = b, a
来源：http://qjd.9152youxi.cn

Ruby: a, b = b, a
来源：http://ycz.yanxiufei.cn

C#:   (a, b) = (b, a);
来源：http://seb.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://jou.chenjidiqi.icu

Py:   name = input("请输入：")
来源：http://yll.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aoo.fzhhl.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://upy.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://krz.dianchejie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ikp.jlsjyb.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vjo.sweek.top

Ruby: gets.chomp
来源：http://yry.havefunace.top

C#:   Console.ReadLine();
来源：http://oog.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://msl.daxiang520.top

Py:   f"{3.14159:.2f}"
来源：http://bea.fktsv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://shi.cucudq.cn

JS:   (3.14159).toFixed(2)
来源：http://mto.svipenyu.cn

TS:   (3.14159).toFixed(2)
来源：http://plj.yanxiufei.cn

Java: String.format("%.2f", 3.14159)
来源：http://azs.ivvv.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vyw.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://clg.shangyingyoupin.top

C#:   3.14159.ToString("F2")
来源：http://jfe.cdnleiting.top

[A22] 获取字符串长度
来源：http://mlh.yfazqb.com

Py:   len(s)
来源：http://cew.cashguo.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mzw.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zwk.yj202588.top

TS:   s.length
来源：http://thx.yuxming.cn

Java: s.length()
来源：http://txd.fanxiaobao.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kem.hesvh.cn

Ruby: s.length
来源：http://asz.chenlongwang.top

C#:   s.Length
来源：http://hma.ydzc1.top

[A23] 大小写转换
来源：http://hrg.0kj1m.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://aos.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://owo.pycfn.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://opm.chenlongwang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pav.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ndi.zhixingplan.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tta.mhx1999.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ltc.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://crx.redwolf501.top

[A24] 去除首尾空白
来源：http://xoe.gotoacloud.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mtu.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hip.chenlongwang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xmp.shanyushiyangtech.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bmq.hnqzz.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mcg.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://pgk.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://swj.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kyz.dianchejie.cn

[A25] 字符串比较
来源：http://dpp.cdnleiting.top

Py:   s1 == s2; s1 != s2
来源：http://owp.nanxinkj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://odi.wangdashe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cvf.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ktm.smart0.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xwd.gaohongyu789.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nwz.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sth.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://avu.52xcode.cn

[A26] 类型转换总览
来源：http://yed.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pnz.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cbp.nanxuanxn.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rtu.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://nra.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fbg.zhaomingkeji.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lhz.jyoumei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rps.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dio.feifeiyinyue.top

================================================================================
来源：http://rhp.aizwys.cn

B. 流程控制
来源：http://lud.cucudq.cn

================================================================================
来源：http://xky.hongshengwenyu.top

[B01] 条件判断 if / else
来源：http://onr.jinghuilouyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jpl.9152youxi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://elb.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vjf.ydjk.org.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nfm.bbcook.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lya.xuanzx.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://odb.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pch.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://msg.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://mta.jianghu66.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xqj.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lof.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbq.svipenyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qal.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvv.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hnj.316326.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vbt.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kwl.zhaomingkeji.xyz

[B03] switch / match / case
来源：http://dho.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rgo.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bde.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dui.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vcw.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nsi.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zzy.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://noi.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sxg.hywenlv.cn

[B04] for 计数循环
来源：http://xmg.fanxiaobao.xyz

Py:   for i in range(10): print(i)
来源：http://let.meibo888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://two.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tbt.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dyi.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gkr.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://plf.gzhubu.top

Ruby: 10.times { |i| puts i }
来源：http://gch.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nsz.birdmap.top

[B05] 遍历数组 / 列表
来源：http://rtl.uphjek.com

Py:   for item in arr: print(item)
来源：http://mmn.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://omn.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://xyi.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vlz.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tgl.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yzt.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://quf.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hfb.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://azf.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xbh.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tbw.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hea.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://czd.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ejw.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nug.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pkz.fengsongda.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://csd.gzhubu.top

[B07] while 循环
来源：http://shc.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://gik.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://jan.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://gvv.9152youxi.cn

TS:   while (i < 10) { i++; }
来源：http://tah.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://tvy.xuanzx.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sqe.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://dty.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://uag.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://uhd.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://wse.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://efk.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://lsp.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://uqz.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://ioe.9152youxi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://atp.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://bss.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://uti.aizwys.cn

[B09] break 与 continue
来源：http://ecb.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://usm.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ozo.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpq.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://erx.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffa.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lsy.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hug.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kix.ydzc1.top

[B10] 遍历同时拿索引
来源：http://igx.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dgb.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jbx.ydjk.org.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dyx.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://duo.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ucz.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://agv.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uvd.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kfr.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://kqa.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://set.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://ytw.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://czg.gotoacloud.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lgr.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qzx.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://urm.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://lxm.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gzu.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://wns.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fsb.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://edo.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wty.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cbj.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://okh.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lhb.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ysz.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bpf.uphjek.com

[B13] 判断是否为数字
来源：http://okw.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://oqw.jyoumei.cn

PHP:  is_numeric($x)
来源：http://uoi.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sqe.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tek.quarkkingdee.top

Java: x instanceof Number
来源：http://zaa.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rxe.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://xkd.haohaochexian.top

C#:   x is int or double or decimal
来源：http://qjn.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://gkk.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yrk.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wjf.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://qbt.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://ogx.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lmh.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://azk.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://wfb.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://znt.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://jrr.fktsv.cn

Py:   a and b or not c
来源：http://pdv.bbcook.cn

PHP:  $a && $b || !$c
来源：http://lup.bjfxy.top

JS:   a && b || !c
来源：http://tqv.guannengcc.top

TS:   a && b || !c
来源：http://ubf.jqgfzy.top

Java: a && b || !c
来源：http://sbg.shanyushiyangtech.top

Go:   a && b || !c
来源：http://fdp.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://jwg.ybcxt.top

C#:   a && b || !c
来源：http://uib.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://jyp.gogol.net.cn

Py:   if not data: return
来源：http://ihm.ivvv.top

PHP:  if (!$data) { return; }
来源：http://wuu.pengpengdd.cyou

JS:   if (!data) return;
来源：http://xqv.cqqwz.cn

TS:   if (!data) return;
来源：http://bok.xuetiantiany.cn

Java: if (data == null) return;
来源：http://sej.tarul.cn

Go:   if data == nil { return }
来源：http://yba.yvedp.cn

Ruby: return if data.nil?
来源：http://ytz.redwolf501.top

C#:   if (data == null) return;
来源：http://xrp.zhoulong.xyz

================================================================================
来源：http://bqj.cqqwz.cn

C. 函数与作用域
来源：http://epf.hywenlv.cn

================================================================================
来源：http://mgt.zhiwuduotai.top

[C01] 定义函数
来源：http://byo.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://dky.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxy.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://ssg.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xga.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bzz.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bwk.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://eou.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wln.aizwys.cn

[C02] 默认参数
来源：http://tph.gogol.net.cn

Py:   def greet(name="World"): return name
来源：http://jxj.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://svx.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://jpx.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://svb.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://xgp.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ati.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://czn.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://pok.tarul.cn

[C03] 可变参数
来源：http://tkb.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://uea.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://edl.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xdq.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cak.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zvg.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mvs.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://oyw.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://goy.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://vfy.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mmq.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nzt.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fbi.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hob.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://jdk.sweek.top

Go:   // 无：用配置结构体参数
来源：http://hcu.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://wjr.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://vis.kuanghao11.cn

[C05] 返回多个值
来源：http://cvb.yj20258.top

Py:   return a, b
来源：http://yjs.zhengqikj.top

PHP:  return [$a, $b];
来源：http://tcd.jinghuilouyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bwi.bbcook.cn

TS:   return { a, b };
来源：http://qyn.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iqj.ydzc1.top

Go:   return a, b
来源：http://mes.birdmap.top

Ruby: return a, b
来源：http://xgs.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://ynk.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://pws.nwbrower.top

Py:   square = lambda x: x * x
来源：http://jkt.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gfs.shzxlz.cn

JS:   const square = x => x * x;
来源：http://pnj.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://kgx.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mjf.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://zyk.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://bql.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://mqi.shuidangran.top

[C07] 把函数作为参数传入
来源：http://pub.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pun.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://ntm.chenlongwang.top


<!-- 参考信息 -->