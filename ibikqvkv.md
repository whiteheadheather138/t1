代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rlv.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://crx.gotoacloud.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jww.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ohh.uphjek.com

[A18] 字符与 ASCII 码互转
来源：http://ewb.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://aul.cashguo.top

PHP:  ord("A"); chr(65)
来源：http://bkn.shanyushiyangtech.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://prp.chenjidiqi.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zzj.daria6918.cn

Java: (int) 'A'; (char) 65
来源：http://ede.gogol.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gci.andypj.xyz

Ruby: "A".ord; 65.chr
来源：http://liy.yanxiufei.cn

C#:   (int)'A'; (char)65
来源：http://krh.daxiang520.top

[A19] 交换两个变量
来源：http://hyu.shzxlz.cn

Py:   a, b = b, a
来源：http://vxv.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://qph.xylfe.cn

JS:   [a, b] = [b, a];
来源：http://faj.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://mro.uphjek.com

Java: int t = a; a = b; b = t;
来源：http://zxi.jyoumei.cn

Go:   a, b = b, a
来源：http://ckp.ctjpmb.com

Ruby: a, b = b, a
来源：http://exp.yongpay.top

C#:   (a, b) = (b, a);
来源：http://xpb.andypj.xyz

[A20] 读取标准输入
来源：http://hqm.jinqigfzy.top

Py:   name = input("请输入：")
来源：http://jna.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sac.fengsongda.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gke.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://fht.cashguo.top

Java: new Scanner(System.in).nextLine()
来源：http://bnc.smart0.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vdw.aizwys.cn

Ruby: gets.chomp
来源：http://mqg.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://bxk.bbcook.cn

[A21] 保留指定小数位输出
来源：http://fjq.feifeiyinyue.top

Py:   f"{3.14159:.2f}"
来源：http://yps.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rzb.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://smy.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://nxh.svipenyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://jdg.chenlongwang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hlz.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://xta.cucudq.cn

C#:   3.14159.ToString("F2")
来源：http://ano.tanke756.top

[A22] 获取字符串长度
来源：http://mpk.jiagoushi.top

Py:   len(s)
来源：http://cwl.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yjp.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vhq.snrcjt.cn

TS:   s.length
来源：http://nxb.0kj1m.cn

Java: s.length()
来源：http://jky.redwolf501.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oso.xuanzx.com

Ruby: s.length
来源：http://dgn.tarul.cn

C#:   s.Length
来源：http://wip.sxryk.cn

[A23] 大小写转换
来源：http://ykl.shuidangran.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qoc.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bee.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://svw.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ybe.dashuyun.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vdl.yj20258.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fsd.jianghu66.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yvf.uphjek.com

C#:   s.ToUpper(); s.ToLower()
来源：http://vbg.hongshengwenyu.top

[A24] 去除首尾空白
来源：http://njv.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://osq.jiagoushi.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fxd.zhongyouzk.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cue.guannengcc.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sqw.yueranfly.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hwo.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://xus.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://arh.9152youxi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hxh.sysykeji.top

[A25] 字符串比较
来源：http://aeg.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://ucp.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ncb.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bht.aibaodan.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mef.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ufd.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xab.tian-w.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fue.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lpc.cdnleiting.top

[A26] 类型转换总览
来源：http://bhk.wangshuangyany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yss.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kxu.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ust.xylfe.cn

TS:   Number() String() Boolean() x as number
来源：http://fof.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hbk.fzhhl.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lia.smart0.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://dwk.ctjpmb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://opb.zdqjudy.top

================================================================================
来源：http://oyo.hammf.cn

B. 流程控制
来源：http://gyp.chenlongwang.top

================================================================================
来源：http://pao.fehbvm.com

[B01] 条件判断 if / else
来源：http://bin.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://sgh.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jby.redwolf501.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vbp.gzhubu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://euh.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vdc.zdbjq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xey.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lle.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xbg.sxryk.cn

[B02] 多分支 else if / elif
来源：http://hof.hysaishi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://guo.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://slw.yj20258.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cre.cqqwz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hbh.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syi.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jit.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qvv.sysykeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://prg.epnwcf.com

[B03] switch / match / case
来源：http://edi.tanke756.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nhh.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ziz.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hsn.wangdashe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kwr.yuanzhike.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ifd.hnxiangtu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bxa.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xkk.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tno.sjlbkw.cn

[B04] for 计数循环
来源：http://iph.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://jne.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tsg.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iiu.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wkx.svipenyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://snm.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xrd.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://wsv.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cht.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://ksf.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://gku.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fwf.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jen.ehwqpu.com

TS:   for (const item of arr) { console.log(item); }
来源：http://kkv.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://tba.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wyz.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://tcq.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xwf.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://kyl.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://con.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ozo.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pxr.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jej.zdqjudy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uoa.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pyf.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hqd.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nfu.xinyue.icu

[B07] while 循环
来源：http://uuu.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://mhs.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cbs.xuetiantiany.cn

JS:   while (i < 10) { i++; }
来源：http://zfc.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://oeu.jinyuanbaomall.cn

Java: while (i < 10) { i++; }
来源：http://xxb.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vay.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://nog.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://ocx.uphjek.com

[B08] do-while（至少执行一次）
来源：http://zeh.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://hjs.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mwj.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://ugc.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://mtn.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://wza.aibaodan.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rrg.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://myh.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://kzw.zhongyouzk.top

[B09] break 与 continue
来源：http://rhe.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hwq.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hpx.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yom.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obk.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bll.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fsk.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aal.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqs.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://mbu.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bns.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pcm.yj20258.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vmz.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lbe.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qux.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hqy.jqgufenzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eez.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hbg.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://gax.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://xqf.c1oappe.top

PHP:  range(0, 10, 2);
来源：http://etj.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bwu.jlsjyb.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qaq.tarul.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mqo.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rzp.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://fpn.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dtx.hfpthk.cn

[B12] 跳出多层循环
来源：http://sjd.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://iyq.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cyf.jinqigufen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cef.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jcy.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dnx.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tpu.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kid.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eam.yanxiufei.cn

[B13] 判断是否为数字
来源：http://qoh.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://gki.gzhubu.top

PHP:  is_numeric($x)
来源：http://mwn.nanxuanxn.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ewb.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wuy.shzxlz.cn

Java: x instanceof Number
来源：http://etc.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qmb.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://lwv.gotoacloud.top

C#:   x is int or double or decimal
来源：http://tpg.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://dox.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oju.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mvo.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://hjq.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://jru.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xub.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zpx.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nei.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://deq.haohaochexian.top

[B15] 布尔运算与取反
来源：http://ywa.xinyue.icu

Py:   a and b or not c
来源：http://hlb.bjfxy.top

PHP:  $a && $b || !$c
来源：http://rei.nwbrower.top

JS:   a && b || !c
来源：http://tii.havefunace.top

TS:   a && b || !c
来源：http://wtz.bbcook.cn

Java: a && b || !c
来源：http://bsd.shzxlz.cn

Go:   a && b || !c
来源：http://nyg.zhengqikj.top

Ruby: a && b || !c
来源：http://eru.yuxming.cn

C#:   a && b || !c
来源：http://mhq.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://eaz.yj20258888.top

Py:   if not data: return
来源：http://qvd.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://vuj.wangshuangyany.cn

JS:   if (!data) return;
来源：http://skx.sysykeji.top

TS:   if (!data) return;
来源：http://zix.cucudq.cn

Java: if (data == null) return;
来源：http://gkj.bbcook.cn

Go:   if data == nil { return }
来源：http://sfc.gzhubu.top

Ruby: return if data.nil?
来源：http://ypb.zhoulong.xyz

C#:   if (data == null) return;
来源：http://mcd.smart0.xyz

================================================================================
来源：http://zag.feifeiyinyue.top

C. 函数与作用域
来源：http://epx.yonumen.top

================================================================================
来源：http://ipd.yueranfly.top

[C01] 定义函数
来源：http://nzn.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://sei.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://akn.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://euv.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://onm.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://six.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uvt.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://kyw.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cex.jiagoushi.top

[C02] 默认参数
来源：http://jpk.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://yoh.chenzaomai.com

PHP:  function greet($name = "World") { return $name; }
来源：http://joh.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://mrj.chenzaomai.com

TS:   function greet(name: string = "World") { return name; }
来源：http://pez.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ezl.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xys.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://rlm.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://vvu.wangshuangyany.cn

[C03] 可变参数
来源：http://plu.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://deo.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hoi.zhijiandao.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ind.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ixz.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hvr.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://von.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://sip.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jfw.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://ljo.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wza.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bpd.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pnu.fengsongda.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cci.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://nny.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://nvx.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://oni.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://hqh.ehwqpu.com

[C05] 返回多个值
来源：http://mxe.smart0.xyz

Py:   return a, b
来源：http://jnl.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://jcc.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xrv.vehdjk.com

TS:   return { a, b };
来源：http://nrp.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qmr.yongpay.top

Go:   return a, b
来源：http://jpu.daxiang520.top

Ruby: return a, b
来源：http://plt.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://vdi.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://lxh.uphjek.com

Py:   square = lambda x: x * x
来源：http://pns.vehdjk.com

PHP:  $square = fn($x) => $x * $x;
来源：http://wxx.zdqjudy.top

JS:   const square = x => x * x;
来源：http://fgo.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://yvo.52xcode.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://umi.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://zha.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://zxu.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://hww.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://gno.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ztu.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://soc.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nlu.gaohongyu789.top

TS:   arr.map(String)
来源：http://kro.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oie.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://amp.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://zgt.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ubl.yongpay.top

[C08] 闭包
来源：http://oez.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zey.316326.xyz


<!-- 参考信息 -->