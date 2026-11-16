代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzy.ppjwa.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xxo.sweek.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dyj.sweek.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bbc.hongshengwenyu.top

[A18] 字符与 ASCII 码互转
来源：http://zow.gogol.net.cn

Py:   ord("A"); chr(65)
来源：http://mdl.vqdsnc.cn

PHP:  ord("A"); chr(65)
来源：http://tjz.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nef.havefunace.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wkj.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://ity.jiagoushi.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kyb.jiagoushi.top

Ruby: "A".ord; 65.chr
来源：http://wsm.hnxiangtu.top

C#:   (int)'A'; (char)65
来源：http://gxu.fktsv.cn

[A19] 交换两个变量
来源：http://ifn.epnwcf.com

Py:   a, b = b, a
来源：http://inu.hnqzz.top

PHP:  [$a, $b] = [$b, $a];
来源：http://cgo.tian-w.cn

JS:   [a, b] = [b, a];
来源：http://xka.cashguo.top

TS:   [a, b] = [b, a];
来源：http://csc.andypj.xyz

Java: int t = a; a = b; b = t;
来源：http://kko.chenzaomai.com

Go:   a, b = b, a
来源：http://msh.316326.xyz

Ruby: a, b = b, a
来源：http://yvw.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://tbb.ydzc1.top

[A20] 读取标准输入
来源：http://upa.xziqi.cn

Py:   name = input("请输入：")
来源：http://dpp.zhijiandao.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ael.jyoumei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://img.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://nfw.ywan-chungtsiang.top

Java: new Scanner(System.in).nextLine()
来源：http://fzh.gaohongyu789.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tok.nanxinkj.top

Ruby: gets.chomp
来源：http://etu.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://hcr.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://jyo.birdmap.top

Py:   f"{3.14159:.2f}"
来源：http://zhl.wangdashe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kyt.jinghuilouyu.cn

JS:   (3.14159).toFixed(2)
来源：http://gwy.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://uae.zhengqikj.top

Java: String.format("%.2f", 3.14159)
来源：http://ayo.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ixu.jlsjyb.cn

Ruby: format("%.2f", 3.14159)
来源：http://gsg.ydjk.org.cn

C#:   3.14159.ToString("F2")
来源：http://orl.52xcode.cn

[A22] 获取字符串长度
来源：http://nee.gotoacloud.top

Py:   len(s)
来源：http://pxj.svipenyu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nle.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wpz.jqgufenzy.top

TS:   s.length
来源：http://dsp.nwbrower.top

Java: s.length()
来源：http://yvm.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zqw.dianchejie.cn

Ruby: s.length
来源：http://itg.yj202588.top

C#:   s.Length
来源：http://sko.jqgfzy.top

[A23] 大小写转换
来源：http://nxk.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hdq.bbcook.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ukc.haohaochexian.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sjo.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gug.yfazqb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xkk.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qot.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ttf.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xbn.redwolf501.top

[A24] 去除首尾空白
来源：http://hly.dianchejie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oqa.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tfj.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nne.feifeiyinyue.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jns.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jsa.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://bik.tianlin.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wtz.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://obu.ctjpmb.com

[A25] 字符串比较
来源：http://rdz.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://wsp.jiagoushi.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cup.gaohongyu789.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hzc.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aac.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bll.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kej.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://svz.52xcode.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://exw.yanxiufei.cn

[A26] 类型转换总览
来源：http://zwt.kuanghao11.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hpa.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tbb.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yqq.tian-w.cn

TS:   Number() String() Boolean() x as number
来源：http://apk.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hkv.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fbz.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ocd.pengpengdd.cyou

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xbe.tanke756.top

================================================================================
来源：http://zku.sysykeji.top

B. 流程控制
来源：http://teo.wangshuangyany.cn

================================================================================
来源：http://yzq.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://rvp.kuanghao11.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://akq.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qjd.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ptm.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rbk.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dvz.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gqc.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fow.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wpl.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://iay.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://usr.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vmq.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uvd.c1oappe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yek.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzm.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://epz.hywenlv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mpm.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vif.chenzaomai.com

[B03] switch / match / case
来源：http://tlq.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ubb.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://geh.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://abi.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hxc.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wfm.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wqt.aibaodan.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lmc.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kkm.yj20258888.top

[B04] for 计数循环
来源：http://rda.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://cqx.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ewr.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qja.yvedp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vdk.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xzu.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vnx.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://hzq.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uhb.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://auw.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://wxo.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tbv.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oov.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rbd.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jze.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tor.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://ahr.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gfy.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://vqv.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yve.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ykv.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sld.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oxk.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dhs.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lvm.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jhm.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ogp.chenzaomai.com

[B07] while 循环
来源：http://uia.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://bwt.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ody.shangyingyoupin.top

JS:   while (i < 10) { i++; }
来源：http://qxc.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://jvk.yj202588.top

Java: while (i < 10) { i++; }
来源：http://kdn.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gob.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://rpq.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://vgj.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://xla.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://pnz.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jys.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://csv.daxiang520.top

TS:   do { i++; } while (i < 10);
来源：http://hcb.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://cpp.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://urq.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://hve.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://bbd.haohaochexian.top

[B09] break 与 continue
来源：http://bwb.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uns.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tuv.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nbq.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zrw.yangfankeji.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eat.shangyingyoupin.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xoy.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://crh.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vao.nwbrower.top

[B10] 遍历同时拿索引
来源：http://gwu.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nfq.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lca.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kdm.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fsd.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lyz.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://umm.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sng.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ffh.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://kve.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://eaj.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://ypu.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://suk.gotoacloud.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dnx.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://erx.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kck.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://kch.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qmj.jinqigufen.top

[B12] 跳出多层循环
来源：http://pkg.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mda.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cdy.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://umu.hywenlv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ejf.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gwi.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hzg.zhoulong.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://udl.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://atg.316326.xyz

[B13] 判断是否为数字
来源：http://hwb.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://yth.ivvv.top

PHP:  is_numeric($x)
来源：http://ate.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://acb.zhoulong.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alu.fktsv.cn

Java: x instanceof Number
来源：http://tsw.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://smm.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://wue.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://jbj.yueranfly.top

[B14] 判断值是否在集合内
来源：http://gqk.guowangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fyt.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qnl.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://juj.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://kit.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qur.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ouc.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tcl.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://adc.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://zsq.jianghu66.top

Py:   a and b or not c
来源：http://bsg.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://qua.hfpthk.cn

JS:   a && b || !c
来源：http://mps.tarul.cn

TS:   a && b || !c
来源：http://unw.iojbl.cn

Java: a && b || !c
来源：http://ott.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://ger.hesvh.cn

Ruby: a && b || !c
来源：http://mjs.havefunace.top

C#:   a && b || !c
来源：http://ysr.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://gfx.gotoacloud.top

Py:   if not data: return
来源：http://jgj.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://lor.hammf.cn

JS:   if (!data) return;
来源：http://cdq.ctjpmb.com

TS:   if (!data) return;
来源：http://dmh.zdbjq.cn

Java: if (data == null) return;
来源：http://sjb.ydzc1.top

Go:   if data == nil { return }
来源：http://hqr.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://usd.uphjek.com

C#:   if (data == null) return;
来源：http://ebk.shangyingyoupin.top

================================================================================
来源：http://rui.jinyuanbaomall.cn

C. 函数与作用域
来源：http://gyw.zhiwuduotai.top

================================================================================
来源：http://mci.wangshuangyany.cn

[C01] 定义函数
来源：http://twn.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://zzc.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kht.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://cbx.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://apk.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gqe.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://oay.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://dra.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vsx.cheryme.top

[C02] 默认参数
来源：http://kkv.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://bfx.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://arg.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://haj.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xed.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://idu.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vpx.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://wgj.bbcook.cn

C#:   string Greet(string name = "World") => name;
来源：http://xkr.gzhubu.top

[C03] 可变参数
来源：http://tqp.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://krm.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://osa.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jdn.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tcr.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tek.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lqe.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://brz.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tpu.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://sml.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xyb.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rlv.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oku.52xcode.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://omq.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://fsl.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://pdc.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://phn.yuanzhike.top

C#:   f(a: 1, b: 2)
来源：http://fth.kuanghao11.cn

[C05] 返回多个值
来源：http://llo.gaohongyu789.top

Py:   return a, b
来源：http://iwa.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://owh.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://psd.gotoacloud.top

TS:   return { a, b };
来源：http://ljh.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wie.zhoulong.xyz

Go:   return a, b
来源：http://kzf.ctjpmb.com

Ruby: return a, b
来源：http://ivo.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://pdl.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://fzp.ivvv.top

Py:   square = lambda x: x * x
来源：http://apu.snrcjt.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zkh.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://kfh.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://nnl.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://chp.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://zqn.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://vel.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ojs.fktsv.cn

[C07] 把函数作为参数传入
来源：http://voh.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://smp.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://xdy.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nya.cqqwz.cn

TS:   arr.map(String)
来源：http://jos.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ynb.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oau.hcnkem.com

Ruby: arr.map(&:upcase)
来源：http://eqb.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://glr.nanxuanxn.top

[C08] 闭包
来源：http://bom.hysaishi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jvn.yangfankeji.com


<!-- 参考信息 -->