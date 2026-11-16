代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ewl.zhiwuduotai.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wke.fanxiaobao.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxs.fengsongda.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qzz.fengsongda.top

[A18] 字符与 ASCII 码互转
来源：http://qpb.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://hcg.c1oappe.top

PHP:  ord("A"); chr(65)
来源：http://dmt.xingfuxueyuan.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bcd.gzhubu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uxm.zhoulong.xyz

Java: (int) 'A'; (char) 65
来源：http://rth.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wnf.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://luf.jqgfzy.top

C#:   (int)'A'; (char)65
来源：http://xgv.jqgufenzy.top

[A19] 交换两个变量
来源：http://tib.jlsjyb.cn

Py:   a, b = b, a
来源：http://xiy.hcnkem.com

PHP:  [$a, $b] = [$b, $a];
来源：http://fyo.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://aih.zhengqikj.top

TS:   [a, b] = [b, a];
来源：http://blz.fehbvm.com

Java: int t = a; a = b; b = t;
来源：http://cfo.guowangkeji.top

Go:   a, b = b, a
来源：http://unm.cheryme.top

Ruby: a, b = b, a
来源：http://pds.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://ery.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://lvy.gotoacloud.top

Py:   name = input("请输入：")
来源：http://rcz.uphjek.com

PHP:  $name = trim(fgets(STDIN));
来源：http://sso.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://caj.sysykeji.top

TS:   // Node.js：readline 模块
来源：http://jqy.ctjpmb.com

Java: new Scanner(System.in).nextLine()
来源：http://pls.vqdsnc.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kdh.yfazqb.com

Ruby: gets.chomp
来源：http://dax.zdbjq.cn

C#:   Console.ReadLine();
来源：http://qgj.zdqjudy.top

[A21] 保留指定小数位输出
来源：http://tfu.xuanzx.com

Py:   f"{3.14159:.2f}"
来源：http://wfv.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qmj.hesvh.cn

JS:   (3.14159).toFixed(2)
来源：http://xoi.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://kcn.sysykeji.top

Java: String.format("%.2f", 3.14159)
来源：http://sdl.ppjwa.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wzm.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://shh.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://iuy.c1oappe.top

[A22] 获取字符串长度
来源：http://war.chenzaomai.com

Py:   len(s)
来源：http://eec.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://upz.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yor.havefunace.top

TS:   s.length
来源：http://dpu.shuidangran.top

Java: s.length()
来源：http://vhz.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://okd.zhoulong.xyz

Ruby: s.length
来源：http://eyx.cucudq.cn

C#:   s.Length
来源：http://aks.hysaishi.cn

[A23] 大小写转换
来源：http://jnn.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ljx.nanxuanxn.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pzi.haohaochexian.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vsd.fengsongda.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zpx.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ccp.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qvn.jlsjyb.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mad.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://yvj.hnqzz.top

[A24] 去除首尾空白
来源：http://tto.52xcode.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nvr.ctjpmb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hzy.jqgufenzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sqv.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rlx.shanyushiyangtech.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qeh.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://rku.cheryme.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kbz.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ufb.shuidangran.top

[A25] 字符串比较
来源：http://hzr.gotoacloud.top

Py:   s1 == s2; s1 != s2
来源：http://pwa.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bkn.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lsh.zhixingplan.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dra.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xss.tian-w.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xkt.jianghu66.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rqg.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xcq.kuanghao11.cn

[A26] 类型转换总览
来源：http://rlc.andypj.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tri.ydzc1.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ufr.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nxn.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://zcu.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pzz.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nqb.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ovp.xylfe.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xre.snrcjt.cn

================================================================================
来源：http://rhm.pengpengdd.cyou

B. 流程控制
来源：http://mro.daria6918.cn

================================================================================
来源：http://rzu.hcnkem.com

[B01] 条件判断 if / else
来源：http://ksy.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dbi.shuidangran.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sdt.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lqe.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nfj.yj20258888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xpk.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vla.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dvw.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://izs.jinghuilouyu.cn

[B02] 多分支 else if / elif
来源：http://sut.zhengqikj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nce.tianlin.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://utv.jyoumei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uju.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://imy.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hme.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hyw.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://caz.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://esq.ydzc1.top

[B03] switch / match / case
来源：http://mal.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eki.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ksq.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rky.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xfe.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bdr.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tlj.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zft.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xfy.ydjk.org.cn

[B04] for 计数循环
来源：http://hvo.kuanghao11.cn

Py:   for i in range(10): print(i)
来源：http://efn.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pfd.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vfy.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jth.gaohongyu789.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rpb.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zpe.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://hpx.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://usw.yj20258.top

[B05] 遍历数组 / 列表
来源：http://cak.mhx1999.top

Py:   for item in arr: print(item)
来源：http://axf.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gfy.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://axr.ehwqpu.com

TS:   for (const item of arr) { console.log(item); }
来源：http://gdy.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://zml.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kjr.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://ksk.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oiq.tarul.cn

[B06] 遍历字典 / 对象
来源：http://mcj.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ayy.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aua.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gog.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tcj.shuidangran.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://akt.jqgufenzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dyz.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rmz.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xho.redwolf501.top

[B07] while 循环
来源：http://pta.yj20258888.top

Py:   while i < 10: i += 1
来源：http://kuz.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nys.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://vnk.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://nbm.316326.xyz

Java: while (i < 10) { i++; }
来源：http://suj.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kyv.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://wed.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://sni.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://nfe.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://fut.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kio.ivvv.top

JS:   do { i++; } while (i < 10);
来源：http://plu.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://lpb.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://ifl.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://unz.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kcu.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://twl.shangyingyoupin.top

[B09] break 与 continue
来源：http://lux.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pdw.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ron.gzhubu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqt.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fht.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbj.dashuyun.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bon.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wrd.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kkh.yuxming.cn

[B10] 遍历同时拿索引
来源：http://npi.cucudq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xjv.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dig.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qvz.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lso.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vuc.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dih.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xwd.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ixs.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://uji.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://nuh.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://wpl.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mha.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://goj.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mjw.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jnm.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://pdv.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kal.fzhhl.top

[B12] 跳出多层循环
来源：http://giq.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://azx.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://toh.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jwo.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qps.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qcg.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://elj.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rsw.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vwv.yonumen.top

[B13] 判断是否为数字
来源：http://vfx.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://zic.cheryme.top

PHP:  is_numeric($x)
来源：http://nxg.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kba.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nof.guowangkeji.top

Java: x instanceof Number
来源：http://gmi.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gll.feifeiyinyue.top

Ruby: x.is_a?(Numeric)
来源：http://jwo.zdqjudy.top

C#:   x is int or double or decimal
来源：http://euk.hammf.cn

[B14] 判断值是否在集合内
来源：http://ikv.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://srt.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sgu.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://pto.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://ajx.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xbr.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mlr.tian-w.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vrl.ywan-chungtsiang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zdb.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://hhl.tian-w.cn

Py:   a and b or not c
来源：http://xuh.daria6918.cn

PHP:  $a && $b || !$c
来源：http://rct.sysykeji.top

JS:   a && b || !c
来源：http://zkv.ydzc1.top

TS:   a && b || !c
来源：http://uks.jqgfzy.top

Java: a && b || !c
来源：http://fmv.sysykeji.top

Go:   a && b || !c
来源：http://sty.hesvh.cn

Ruby: a && b || !c
来源：http://xqu.xziqi.cn

C#:   a && b || !c
来源：http://ukz.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://odd.jinqigfzy.top

Py:   if not data: return
来源：http://ffb.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://nwv.tanke756.top

JS:   if (!data) return;
来源：http://mnq.jinqigufen.top

TS:   if (!data) return;
来源：http://xfk.nanxuanxn.top

Java: if (data == null) return;
来源：http://zys.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://cqq.chenzaomai.com

Ruby: return if data.nil?
来源：http://zlj.snrcjt.cn

C#:   if (data == null) return;
来源：http://kmn.tanke756.top

================================================================================
来源：http://bth.cdnleiting.top

C. 函数与作用域
来源：http://ruk.gaohongyu789.top

================================================================================
来源：http://btx.zhiwuduotai.top

[C01] 定义函数
来源：http://ftm.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://pgg.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vxp.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://rtb.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqm.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cyk.fktsv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://etk.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://pog.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jqn.zhijiandao.cn

[C02] 默认参数
来源：http://znr.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://akp.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rxw.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://hry.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://emo.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://oyd.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fmv.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://cjd.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://zqd.yvedp.cn

[C03] 可变参数
来源：http://cbp.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://say.ydjk.org.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ufz.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xaa.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrg.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eyc.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lox.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://psk.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sdt.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://fzt.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ksr.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://arb.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://arb.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vxe.hnxiangtu.top

Java: // 无：用 Builder 模式或 record
来源：http://vvr.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://krh.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://zmz.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://idk.hywenlv.cn

[C05] 返回多个值
来源：http://syx.svipenyu.cn

Py:   return a, b
来源：http://qcj.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://vzt.nwbrower.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tlw.dianchejie.cn

TS:   return { a, b };
来源：http://apb.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://khz.aizwys.cn

Go:   return a, b
来源：http://zth.gzhubu.top

Ruby: return a, b
来源：http://ytg.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://qxo.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://gwt.nwbrower.top

Py:   square = lambda x: x * x
来源：http://kys.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zmu.aibaodan.cn

JS:   const square = x => x * x;
来源：http://tnw.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://gdi.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cva.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yyd.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://jiv.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://lal.daxiang520.top

[C07] 把函数作为参数传入
来源：http://uen.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gkt.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dul.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://feb.hywenlv.cn

TS:   arr.map(String)
来源：http://qme.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cvm.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mnw.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://yxk.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hip.yongpay.top

[C08] 闭包
来源：http://fwd.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mxi.havefunace.top


<!-- 参考信息 -->