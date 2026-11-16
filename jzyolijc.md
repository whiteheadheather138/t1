代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pfx.hywenlv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zdr.ctjpmb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ufh.shanyushiyangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ayi.xinyue.icu

[A18] 字符与 ASCII 码互转
来源：http://vrp.jqgfzy.top

Py:   ord("A"); chr(65)
来源：http://xcs.mhx1999.top

PHP:  ord("A"); chr(65)
来源：http://xuc.daria6918.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xaq.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://myq.yangfankeji.com

Java: (int) 'A'; (char) 65
来源：http://scj.c1oappe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ltw.zhixingplan.top

Ruby: "A".ord; 65.chr
来源：http://mcw.hnqzz.top

C#:   (int)'A'; (char)65
来源：http://rgg.hnqzz.top

[A19] 交换两个变量
来源：http://ibf.zhengqikj.top

Py:   a, b = b, a
来源：http://xxd.guowangkeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://apo.yj202588.top

JS:   [a, b] = [b, a];
来源：http://mqx.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://buj.andypj.xyz

Java: int t = a; a = b; b = t;
来源：http://xil.jyoumei.cn

Go:   a, b = b, a
来源：http://opq.gotoacloud.top

Ruby: a, b = b, a
来源：http://mzv.svipenyu.cn

C#:   (a, b) = (b, a);
来源：http://pcx.316326.xyz

[A20] 读取标准输入
来源：http://rpm.svipenyu.cn

Py:   name = input("请输入：")
来源：http://grq.shuidangran.top

PHP:  $name = trim(fgets(STDIN));
来源：http://heb.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sra.zycfv.cn

TS:   // Node.js：readline 模块
来源：http://kca.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://sjs.gogol.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://spp.bbcook.cn

Ruby: gets.chomp
来源：http://anz.jianghu66.top

C#:   Console.ReadLine();
来源：http://kwb.fengsongda.top

[A21] 保留指定小数位输出
来源：http://qzw.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://lqi.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ifp.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://vdl.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://egt.ppjwa.cn

Java: String.format("%.2f", 3.14159)
来源：http://zhv.fktsv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://apw.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://fer.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://ckz.mhx1999.top

[A22] 获取字符串长度
来源：http://xhp.hysaishi.cn

Py:   len(s)
来源：http://jnm.yuanzhike.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://knl.jqgfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hcp.zdqjudy.top

TS:   s.length
来源：http://onq.jinqigfzy.top

Java: s.length()
来源：http://whr.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ruh.ybcxt.top

Ruby: s.length
来源：http://kdp.dianchejie.cn

C#:   s.Length
来源：http://bbs.sufxvd.cn

[A23] 大小写转换
来源：http://uid.yonumen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://yap.zhengqikj.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lqi.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sef.wangshuangyany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://smf.smart0.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jhl.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ajv.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mvr.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nhp.jqgfzy.top

[A24] 去除首尾空白
来源：http://oxa.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lwn.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iux.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ner.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ttj.nanxinkj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lgb.xylfe.cn

Go:   strings.TrimSpace(s)
来源：http://avt.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://swt.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kpr.hywenlv.cn

[A25] 字符串比较
来源：http://oxh.tarul.cn

Py:   s1 == s2; s1 != s2
来源：http://cpp.yonumen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://acx.svipenyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wmm.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dus.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://frt.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lor.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tcs.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://muv.hcnkem.com

[A26] 类型转换总览
来源：http://vgm.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mtq.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ate.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gwf.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://ifh.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wmi.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gae.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nyp.ctjpmb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://swu.aibaodan.cn

================================================================================
来源：http://cjr.vehdjk.com

B. 流程控制
来源：http://bij.pengpengdd.cyou

================================================================================
来源：http://hpb.epnwcf.com

[B01] 条件判断 if / else
来源：http://kub.nanxinkj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xal.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ouz.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kdz.gzhubu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lki.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://tuf.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://reo.guannengcc.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hbi.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://glo.pycfn.com

[B02] 多分支 else if / elif
来源：http://ocv.quarkkingdee.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ufq.bbcook.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mna.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ctd.uphjek.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcg.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xhs.chenzaomai.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yok.vqdsnc.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bmz.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ulr.vehdjk.com

[B03] switch / match / case
来源：http://qix.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zcf.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ulc.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://plq.zhixingplan.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tzl.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lew.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zft.yanxiufei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ztx.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://btu.xziqi.cn

[B04] for 计数循环
来源：http://tqh.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://alq.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fiq.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zhy.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://piq.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mdz.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bho.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://lzg.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qed.chenzaomai.com

[B05] 遍历数组 / 列表
来源：http://rpf.guannengcc.top

Py:   for item in arr: print(item)
来源：http://jpv.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ohl.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://iwv.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ook.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dmr.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rzt.zhaomingkeji.xyz

Ruby: arr.each { |item| puts item }
来源：http://zdt.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gcu.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://yxx.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://nxk.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gqc.chenzaomai.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rot.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txf.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fxc.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xvb.jqgfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zbs.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lwm.yanxiufei.cn

[B07] while 循环
来源：http://evq.pengpengdd.cyou

Py:   while i < 10: i += 1
来源：http://fon.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hui.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://nll.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://asc.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://jyc.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wpf.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://gpo.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://hxz.316326.xyz

[B08] do-while（至少执行一次）
来源：http://bvy.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://sec.9152youxi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jnj.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://nyp.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://yuu.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://iuz.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tcb.xingfuxueyuan.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://fyi.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://usx.gaohongyu789.top

[B09] break 与 continue
来源：http://ljk.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ccu.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mmp.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzk.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xfv.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ijn.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yoq.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rwd.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gye.yvedp.cn

[B10] 遍历同时拿索引
来源：http://wkt.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fxx.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cvf.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ety.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ixf.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wtk.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hnh.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://crz.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yqu.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://bhe.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://nvn.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://rmw.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bws.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jnr.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ilg.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hjk.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://seq.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ypb.andypj.xyz

[B12] 跳出多层循环
来源：http://sws.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wmb.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://agp.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ylg.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jqa.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ifg.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cwd.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zuw.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cou.shangyingyoupin.top

[B13] 判断是否为数字
来源：http://hba.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://upg.316326.xyz

PHP:  is_numeric($x)
来源：http://ljp.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://psj.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fet.yueranfly.top

Java: x instanceof Number
来源：http://bbm.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xnk.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://qzf.yj20258.top

C#:   x is int or double or decimal
来源：http://dul.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://bom.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fgf.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fum.yueranfly.top

JS:   [1, 2, 3].includes(x)
来源：http://gja.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://mnm.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wzm.jianghu66.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cyl.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://rpp.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ayr.iojbl.cn

[B15] 布尔运算与取反
来源：http://gkr.yonumen.top

Py:   a and b or not c
来源：http://lwm.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://lyw.nanxinkj.top

JS:   a && b || !c
来源：http://rgn.hnqzz.top

TS:   a && b || !c
来源：http://ezl.hywenlv.cn

Java: a && b || !c
来源：http://lya.gaohongyu789.top

Go:   a && b || !c
来源：http://igr.dianchejie.cn

Ruby: a && b || !c
来源：http://qsa.cqqwz.cn

C#:   a && b || !c
来源：http://lzn.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://eks.cashguo.top

Py:   if not data: return
来源：http://hzn.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://uzr.c1oappe.top

JS:   if (!data) return;
来源：http://lfl.hnqzz.top

TS:   if (!data) return;
来源：http://imx.gaohongyu789.top

Java: if (data == null) return;
来源：http://rbr.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://wrg.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://sed.ybcxt.top

C#:   if (data == null) return;
来源：http://fbx.hywenlv.cn

================================================================================
来源：http://alc.yuxming.cn

C. 函数与作用域
来源：http://ulk.zdqjudy.top

================================================================================
来源：http://tzf.yj20258888.top

[C01] 定义函数
来源：http://vyg.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://enh.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://efh.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://zph.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zxi.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xzj.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://csi.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://fza.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mcj.nanxuanxn.top

[C02] 默认参数
来源：http://qph.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://vpx.daxiang520.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aaq.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://uzv.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iwz.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zsj.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bfs.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://ige.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://iwh.mhx1999.top

[C03] 可变参数
来源：http://uxp.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://vkk.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wyz.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uhr.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nmn.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zsf.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ine.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lbe.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cvv.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://dyq.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://avk.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bcc.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bhl.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://djk.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://ccp.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://wpx.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://ujc.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://gqs.xylfe.cn

[C05] 返回多个值
来源：http://rhz.zycfv.cn

Py:   return a, b
来源：http://sln.dashuyun.cn

PHP:  return [$a, $b];
来源：http://rjh.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://oso.fengsongda.top

TS:   return { a, b };
来源：http://uuk.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://koh.gogol.net.cn

Go:   return a, b
来源：http://sfm.andypj.xyz

Ruby: return a, b
来源：http://dci.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://qdm.birdmap.top

[C06] 匿名函数 / lambda
来源：http://ilq.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://vwn.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hjz.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://smk.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://xeh.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://clc.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://bbh.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://sqs.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://rjl.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://owd.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ujd.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://opq.yj202588.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jda.fengsongda.top

TS:   arr.map(String)
来源：http://sby.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kmt.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tli.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://kog.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eca.nanxinkj.top

[C08] 闭包
来源：http://tqv.birdmap.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iec.ywan-chungtsiang.top


<!-- 参考信息 -->