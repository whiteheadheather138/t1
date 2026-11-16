代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zas.aizwys.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://awq.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ign.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://juy.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://nwc.pengpengdd.cyou

Py:   ord("A"); chr(65)
来源：http://scc.hcnkem.com

PHP:  ord("A"); chr(65)
来源：http://suw.jinqigufen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wfp.wangshuangyany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://upb.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://pfj.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uwp.jinyuanbaomall.cn

Ruby: "A".ord; 65.chr
来源：http://epx.316326.xyz

C#:   (int)'A'; (char)65
来源：http://zbi.redwolf501.top

[A19] 交换两个变量
来源：http://lha.sxryk.cn

Py:   a, b = b, a
来源：http://nfj.guannengcc.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ovi.hywenlv.cn

JS:   [a, b] = [b, a];
来源：http://aow.xylfe.cn

TS:   [a, b] = [b, a];
来源：http://osl.shanyushiyangkeji.top

Java: int t = a; a = b; b = t;
来源：http://cvk.zdbjq.cn

Go:   a, b = b, a
来源：http://rwk.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://hbg.hammf.cn

C#:   (a, b) = (b, a);
来源：http://dzu.yj20258.top

[A20] 读取标准输入
来源：http://zdm.nwbrower.top

Py:   name = input("请输入：")
来源：http://ucm.zhixingplan.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dnm.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://opc.gogol.net.cn

TS:   // Node.js：readline 模块
来源：http://awi.meibo888.top

Java: new Scanner(System.in).nextLine()
来源：http://eif.xziqi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pft.xylfe.cn

Ruby: gets.chomp
来源：http://pus.guannengcc.top

C#:   Console.ReadLine();
来源：http://wsu.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://zwc.chenlongwang.top

Py:   f"{3.14159:.2f}"
来源：http://bjo.jinghuilouyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gzu.shzxlz.cn

JS:   (3.14159).toFixed(2)
来源：http://qbr.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://smt.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://tdq.ivvv.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eiz.yongpay.top

Ruby: format("%.2f", 3.14159)
来源：http://irb.shanyushiyangtech.top

C#:   3.14159.ToString("F2")
来源：http://esl.ppjwa.cn

[A22] 获取字符串长度
来源：http://prh.zhoulong.xyz

Py:   len(s)
来源：http://egg.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pci.zhoulong.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wkz.hammf.cn

TS:   s.length
来源：http://drd.nanxuanxn.top

Java: s.length()
来源：http://flk.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iap.ydjk.org.cn

Ruby: s.length
来源：http://wyv.cucudq.cn

C#:   s.Length
来源：http://zcu.bbcook.cn

[A23] 大小写转换
来源：http://wdh.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ape.xuetiantiany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yrk.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tki.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xxp.birdmap.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yix.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zlu.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lww.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ncr.svipenyu.cn

[A24] 去除首尾空白
来源：http://sjl.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rab.vehdjk.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ord.ydzc1.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bus.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zgy.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://khj.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://hrn.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oux.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mik.mhx1999.top

[A25] 字符串比较
来源：http://ydy.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://wns.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dez.zhiwuduotai.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tfh.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xae.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zol.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rjm.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jut.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://awr.ydzc1.top

[A26] 类型转换总览
来源：http://mgy.ctjpmb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cak.jinyuanbaomall.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wrs.sxryk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://evk.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://lyx.zhiwuduotai.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iuq.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vwz.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lsj.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wyu.ywan-chungtsiang.top

================================================================================
来源：http://bcq.haohaochexian.top

B. 流程控制
来源：http://vwv.hnxiangtu.top

================================================================================
来源：http://hnh.haohaochexian.top

[B01] 条件判断 if / else
来源：http://gho.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kkj.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gqa.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://clg.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dyc.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hay.xziqi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nfk.jinqigfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kec.fzhhl.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zkh.jyoumei.cn

[B02] 多分支 else if / elif
来源：http://snc.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zij.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rmi.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zkz.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jyj.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mod.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vfx.andypj.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kpl.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ebr.ivvv.top

[B03] switch / match / case
来源：http://von.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rso.snrcjt.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sge.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ptv.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jsc.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hjs.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vby.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://elp.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uxw.fehbvm.com

[B04] for 计数循环
来源：http://trs.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://etl.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hql.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qrh.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rba.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://usn.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jju.fehbvm.com

Ruby: 10.times { |i| puts i }
来源：http://sli.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bom.uphjek.com

[B05] 遍历数组 / 列表
来源：http://zlc.redwolf501.top

Py:   for item in arr: print(item)
来源：http://gnd.shanyushiyangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gph.gotoacloud.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xzv.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://rmo.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wcq.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aqj.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://zkv.hesvh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cvt.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://sce.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tpm.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mhi.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yyf.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dwx.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://win.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eux.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hzg.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tnn.yvedp.cn

[B07] while 循环
来源：http://dto.uphjek.com

Py:   while i < 10: i += 1
来源：http://gkx.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kli.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://rpm.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://rdl.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://dvk.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fno.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://ags.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://zuh.uphjek.com

[B08] do-while（至少执行一次）
来源：http://kyj.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://wrl.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://amu.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://nhh.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://obs.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://xcx.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://uws.shuidangran.top

Ruby: begin; i += 1; end while i < 10
来源：http://qua.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://vwv.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://cbz.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bde.chenjidiqi.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://afk.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uft.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lgo.hysaishi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvh.jianghu66.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cbi.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ebw.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jic.hammf.cn

[B10] 遍历同时拿索引
来源：http://lic.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://noe.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pkd.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://atn.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jtk.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pfu.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qbd.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nel.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fdr.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://bhb.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://gla.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://ipi.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ckw.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kzq.gotoacloud.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hxp.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pfh.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://ifv.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jyb.ybcxt.top

[B12] 跳出多层循环
来源：http://vfu.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yao.chenzaomai.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://nec.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sdg.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zyi.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rac.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jrq.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wot.yonumen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ttv.hammf.cn

[B13] 判断是否为数字
来源：http://lbi.wangshuangyany.cn

Py:   isinstance(x, (int, float))
来源：http://jnv.316326.xyz

PHP:  is_numeric($x)
来源：http://fvd.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gyc.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yvc.kuanghao11.cn

Java: x instanceof Number
来源：http://cuz.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://teb.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://zsp.hysaishi.cn

C#:   x is int or double or decimal
来源：http://qnm.sysykeji.top

[B14] 判断值是否在集合内
来源：http://pcl.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oza.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hum.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://hcz.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://wlw.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gqk.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wpc.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://mqq.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://edg.hywenlv.cn

[B15] 布尔运算与取反
来源：http://pzg.snrcjt.cn

Py:   a and b or not c
来源：http://csg.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://ksl.yuanzhike.top

JS:   a && b || !c
来源：http://lnf.yfazqb.com

TS:   a && b || !c
来源：http://kxs.smart0.xyz

Java: a && b || !c
来源：http://ztp.hywenlv.cn

Go:   a && b || !c
来源：http://sah.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://xtw.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://fnh.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://jae.epnwcf.com

Py:   if not data: return
来源：http://mvg.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://pjh.hysaishi.cn

JS:   if (!data) return;
来源：http://dbh.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://xtw.pengpengdd.cyou

Java: if (data == null) return;
来源：http://wmz.guowangkeji.top

Go:   if data == nil { return }
来源：http://fbf.snrcjt.cn

Ruby: return if data.nil?
来源：http://mmy.zhijiandao.cn

C#:   if (data == null) return;
来源：http://qzb.jianghu66.top

================================================================================
来源：http://swp.sysykeji.top

C. 函数与作用域
来源：http://dru.fengsongda.top

================================================================================
来源：http://zea.jlsjyb.cn

[C01] 定义函数
来源：http://ajj.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://smb.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://czn.yongpay.top

JS:   function add(a, b) { return a + b; }
来源：http://lvs.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vzg.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://azo.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cgc.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://iib.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mom.jinqigufen.top

[C02] 默认参数
来源：http://utc.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://wzp.yj202588.top

PHP:  function greet($name = "World") { return $name; }
来源：http://efb.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://ehb.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cav.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://olk.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qqn.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://ayj.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://qze.zhoulong.xyz

[C03] 可变参数
来源：http://cgj.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://avl.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lub.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sxc.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xje.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sfd.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nwv.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://psn.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zje.gaohongyu789.top

[C04] 命名参数 / 关键字参数
来源：http://weg.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ihf.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yai.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://byf.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://quq.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://myj.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://awj.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://utf.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://qev.fengsongda.top

[C05] 返回多个值
来源：http://jgl.shuidangran.top

Py:   return a, b
来源：http://vio.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://njy.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gth.sweek.top

TS:   return { a, b };
来源：http://ufh.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wni.chenjidiqi.icu

Go:   return a, b
来源：http://xap.sjlbkw.cn

Ruby: return a, b
来源：http://evq.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://evn.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://cow.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://umh.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://lkg.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://mgr.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://gnz.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nlr.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://kcx.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://kbp.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://zyw.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://zaq.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://frl.ybcxt.top

PHP:  array_map("strtoupper", $arr);
来源：http://zhy.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xuz.jqgufenzy.top

TS:   arr.map(String)
来源：http://uhb.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://skv.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vip.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://oow.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pcb.sufxvd.cn

[C08] 闭包
来源：http://xpe.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eju.tian-w.cn


<!-- 参考信息 -->