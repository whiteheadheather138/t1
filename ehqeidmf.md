代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pfr.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jsi.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xig.shzxlz.cn

[A17] 位运算
来源：http://gwx.chenjidiqi.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykr.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://usi.chenlongwang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pud.havefunace.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://trc.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ufq.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kvs.guannengcc.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qiy.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olu.shangyingyoupin.top

[A18] 字符与 ASCII 码互转
来源：http://fro.jlsjyb.cn

Py:   ord("A"); chr(65)
来源：http://iso.aibaodan.cn

PHP:  ord("A"); chr(65)
来源：http://tmj.mhx1999.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yhd.ivvv.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://puj.vehdjk.com

Java: (int) 'A'; (char) 65
来源：http://khq.yongpay.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qxu.zhaomingkeji.xyz

Ruby: "A".ord; 65.chr
来源：http://psn.xuetiantiany.cn

C#:   (int)'A'; (char)65
来源：http://pdi.yueranfly.top

[A19] 交换两个变量
来源：http://fvc.tarul.cn

Py:   a, b = b, a
来源：http://tup.nanxuanxn.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mqj.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://vvd.chenjidiqi.icu

TS:   [a, b] = [b, a];
来源：http://bmr.chenzaomai.com

Java: int t = a; a = b; b = t;
来源：http://xad.cucudq.cn

Go:   a, b = b, a
来源：http://orp.guannengcc.top

Ruby: a, b = b, a
来源：http://bwd.aibaodan.cn

C#:   (a, b) = (b, a);
来源：http://qdh.fktsv.cn

[A20] 读取标准输入
来源：http://zzu.sufxvd.cn

Py:   name = input("请输入：")
来源：http://ufb.zdqjudy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bcn.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zwy.daria6918.cn

TS:   // Node.js：readline 模块
来源：http://yyg.gzhubu.top

Java: new Scanner(System.in).nextLine()
来源：http://yky.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xeu.cdnleiting.top

Ruby: gets.chomp
来源：http://bcz.0kj1m.cn

C#:   Console.ReadLine();
来源：http://ptv.sweek.top

[A21] 保留指定小数位输出
来源：http://vim.wangshuangyany.cn

Py:   f"{3.14159:.2f}"
来源：http://psx.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ujf.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://lsr.vehdjk.com

TS:   (3.14159).toFixed(2)
来源：http://jva.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://dlw.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zfy.iojbl.cn

Ruby: format("%.2f", 3.14159)
来源：http://bra.zdbjq.cn

C#:   3.14159.ToString("F2")
来源：http://rox.redwolf501.top

[A22] 获取字符串长度
来源：http://yft.sxryk.cn

Py:   len(s)
来源：http://bkl.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vqh.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xae.yongpay.top

TS:   s.length
来源：http://ppt.ivvv.top

Java: s.length()
来源：http://ayz.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ubv.hfpthk.cn

Ruby: s.length
来源：http://djb.0kj1m.cn

C#:   s.Length
来源：http://pbk.tianlin.xyz

[A23] 大小写转换
来源：http://por.haohaochexian.top

Py:   s.upper(); s.lower(); s.title()
来源：http://avl.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rjw.0kj1m.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zhc.aizwys.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gnw.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qpz.zycfv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vmz.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iai.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://woe.zhijiandao.cn

[A24] 去除首尾空白
来源：http://gvo.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bmf.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mjj.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iuj.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dpu.ppjwa.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dnm.zhengqikj.top

Go:   strings.TrimSpace(s)
来源：http://elj.shanyushiyangtech.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rrp.daria6918.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tbx.wangshuangyany.cn

[A25] 字符串比较
来源：http://qic.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://poa.shzxlz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hpz.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bmz.jinghuilouyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fue.fktsv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yoh.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://psm.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uxp.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oci.shangyingyoupin.top

[A26] 类型转换总览
来源：http://jff.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://clm.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vww.sysykeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tqe.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://hht.cashguo.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vjq.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xkq.epnwcf.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://fzo.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://knl.ybcxt.top

================================================================================
来源：http://ukl.nwbrower.top

B. 流程控制
来源：http://eca.iojbl.cn

================================================================================
来源：http://gcs.jinqigufen.top

[B01] 条件判断 if / else
来源：http://hab.ywan-chungtsiang.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ixx.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ati.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nqt.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ueb.gaohongyu789.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jec.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://niu.sufxvd.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uwz.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ghi.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://kjo.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kox.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qhy.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubh.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sft.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jpu.yj20258.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pqx.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oui.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://apx.bbcook.cn

[B03] switch / match / case
来源：http://ruv.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pxx.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ylb.aizwys.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wux.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ebb.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fku.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uun.316326.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xse.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jea.yfazqb.com

[B04] for 计数循环
来源：http://yst.feifeiyinyue.top

Py:   for i in range(10): print(i)
来源：http://cat.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ejf.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://roe.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vbg.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ptj.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://unh.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://gtp.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iww.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://mha.zdbjq.cn

Py:   for item in arr: print(item)
来源：http://pms.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fwd.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://atp.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://bmb.fktsv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cjy.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sxq.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://seq.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://woj.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://heg.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://kvn.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ugk.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oay.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uhl.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fdi.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hwj.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rsv.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ccp.cqqwz.cn

[B07] while 循环
来源：http://neq.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://xrm.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://kmm.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://fsj.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://sio.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://iqi.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pwh.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://cph.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://czx.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://tai.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://bdf.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fji.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://vmj.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://hpj.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://nnh.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gcs.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://kyp.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://foh.kuanghao11.cn

[B09] break 与 continue
来源：http://qgi.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kcg.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dcu.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihp.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iuy.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zlq.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zgm.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bdw.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocz.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://pvj.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eey.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://irz.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jqw.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nfg.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uhc.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cfh.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pdr.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gnj.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://pze.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://euh.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://rhe.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yop.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cjo.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rmp.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cyy.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://oad.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xva.yueranfly.top

[B12] 跳出多层循环
来源：http://wcz.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ans.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ohs.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vwe.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lml.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://muv.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ozg.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dyt.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lok.zhixingplan.top

[B13] 判断是否为数字
来源：http://aov.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://ksv.yj20258888.top

PHP:  is_numeric($x)
来源：http://qte.xuetiantiany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zbn.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tpk.yj20258888.top

Java: x instanceof Number
来源：http://lvt.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kkk.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://kwm.smart0.xyz

C#:   x is int or double or decimal
来源：http://dzn.yj20258888.top

[B14] 判断值是否在集合内
来源：http://tie.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ihc.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jqn.jqgufenzy.top

JS:   [1, 2, 3].includes(x)
来源：http://urb.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://tam.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ikz.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oes.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://poe.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kpv.hywenlv.cn

[B15] 布尔运算与取反
来源：http://vmx.shangyingyoupin.top

Py:   a and b or not c
来源：http://inx.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://cmf.cucudq.cn

JS:   a && b || !c
来源：http://jxz.quarkkingdee.top

TS:   a && b || !c
来源：http://rbs.sxryk.cn

Java: a && b || !c
来源：http://chv.yuanzhike.top

Go:   a && b || !c
来源：http://lbd.ydzc1.top

Ruby: a && b || !c
来源：http://ykb.zhixingplan.top

C#:   a && b || !c
来源：http://psv.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pww.ybcxt.top

Py:   if not data: return
来源：http://sti.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://lsb.zhiwuduotai.top

JS:   if (!data) return;
来源：http://adg.cqqwz.cn

TS:   if (!data) return;
来源：http://ffi.tianlin.xyz

Java: if (data == null) return;
来源：http://lpn.xziqi.cn

Go:   if data == nil { return }
来源：http://txn.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://frk.jlsjyb.cn

C#:   if (data == null) return;
来源：http://jtb.52xcode.cn

================================================================================
来源：http://ffh.zycfv.cn

C. 函数与作用域
来源：http://kgx.jlsjyb.cn

================================================================================
来源：http://cls.yuanzhike.top

[C01] 定义函数
来源：http://wfv.meibo888.top

Py:   def add(a, b): return a + b
来源：http://zns.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ldr.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://ydp.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfg.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mog.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://mtg.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://pql.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xtv.cqqwz.cn

[C02] 默认参数
来源：http://xsn.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://nqd.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://gxb.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://ado.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ghb.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zda.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sud.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://vlt.nwbrower.top

C#:   string Greet(string name = "World") => name;
来源：http://swe.epnwcf.com

[C03] 可变参数
来源：http://jss.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://xqj.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://brb.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nhm.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iln.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://raj.c1oappe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://djf.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://sao.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zlo.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://qpn.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ifs.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qac.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pfq.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zrj.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://efx.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://jfs.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://xhp.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://qrv.yuxming.cn

[C05] 返回多个值
来源：http://psg.cqqwz.cn

Py:   return a, b
来源：http://tcc.chenlongwang.top

PHP:  return [$a, $b];
来源：http://syx.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mdv.hfpthk.cn

TS:   return { a, b };
来源：http://elj.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mmc.jyoumei.cn

Go:   return a, b
来源：http://dvn.chenjidiqi.icu

Ruby: return a, b
来源：http://ojp.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://epq.guannengcc.top

[C06] 匿名函数 / lambda
来源：http://bfd.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://ndt.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jnq.cdnleiting.top

JS:   const square = x => x * x;
来源：http://zwy.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://uhx.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://par.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cvr.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://sxh.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://leu.hammf.cn

[C07] 把函数作为参数传入
来源：http://wet.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://owj.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://vdy.gogol.net.cn


<!-- 参考信息 -->