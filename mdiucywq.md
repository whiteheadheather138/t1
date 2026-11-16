代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vze.ybcxt.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://swz.yongpay.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://prl.0kj1m.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vrp.zhijiandao.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lxx.xuanzx.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bsq.uphjek.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qof.jiagoushi.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zsx.yanxiufei.cn

[A18] 字符与 ASCII 码互转
来源：http://jhe.9152youxi.cn

Py:   ord("A"); chr(65)
来源：http://tqm.sufxvd.cn

PHP:  ord("A"); chr(65)
来源：http://zci.9152youxi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nub.shanyushiyangtech.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gwx.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://auo.mhx1999.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ztg.xinyue.icu

Ruby: "A".ord; 65.chr
来源：http://spv.jyoumei.cn

C#:   (int)'A'; (char)65
来源：http://tiz.ehwqpu.com

[A19] 交换两个变量
来源：http://hhg.jinyuanbaomall.cn

Py:   a, b = b, a
来源：http://hpu.tianlin.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://cqv.zhijiandao.cn

JS:   [a, b] = [b, a];
来源：http://erv.zycfv.cn

TS:   [a, b] = [b, a];
来源：http://tjf.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://efi.tarul.cn

Go:   a, b = b, a
来源：http://bqt.feifeiyinyue.top

Ruby: a, b = b, a
来源：http://poa.yj202588.top

C#:   (a, b) = (b, a);
来源：http://sxc.yuxming.cn

[A20] 读取标准输入
来源：http://rzj.cashguo.top

Py:   name = input("请输入：")
来源：http://fee.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vtn.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dok.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://ykf.dianchejie.cn

Java: new Scanner(System.in).nextLine()
来源：http://efm.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eur.hnxiangtu.top

Ruby: gets.chomp
来源：http://oaj.hnxiangtu.top

C#:   Console.ReadLine();
来源：http://dqe.tian-w.cn

[A21] 保留指定小数位输出
来源：http://sax.chenlongwang.top

Py:   f"{3.14159:.2f}"
来源：http://cjg.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://srs.gzhubu.top

JS:   (3.14159).toFixed(2)
来源：http://iul.xuanzx.com

TS:   (3.14159).toFixed(2)
来源：http://mzo.yangfankeji.com

Java: String.format("%.2f", 3.14159)
来源：http://njy.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mhn.zhiwuduotai.top

Ruby: format("%.2f", 3.14159)
来源：http://xlo.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://udo.gzhubu.top

[A22] 获取字符串长度
来源：http://zez.yueranfly.top

Py:   len(s)
来源：http://exl.sweek.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://imb.jinyuanbaomall.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wav.shuidangran.top

TS:   s.length
来源：http://wdm.tianlin.xyz

Java: s.length()
来源：http://ify.xingfuxueyuan.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cwa.hammf.cn

Ruby: s.length
来源：http://jkg.jianghu66.top

C#:   s.Length
来源：http://maj.xziqi.cn

[A23] 大小写转换
来源：http://kky.zhixingplan.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rco.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gnt.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ieu.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gcn.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nee.zhiwuduotai.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mjt.fanxiaobao.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nri.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://pxb.havefunace.top

[A24] 去除首尾空白
来源：http://fxb.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://htn.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oja.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rjt.gaohongyu789.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jfl.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://atd.uphjek.com

Go:   strings.TrimSpace(s)
来源：http://ivq.daxiang520.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gsx.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qno.jinqigufen.top

[A25] 字符串比较
来源：http://rty.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://pih.chenzaomai.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://utx.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qog.xinyue.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rpc.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cpd.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://odw.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rsx.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jgb.dianchejie.cn

[A26] 类型转换总览
来源：http://qri.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://slx.meibo888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pfq.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ceo.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://vxo.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qrq.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vjt.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://abv.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ahw.xylfe.cn

================================================================================
来源：http://rtr.cashguo.top

B. 流程控制
来源：http://edv.yj20258888.top

================================================================================
来源：http://olc.jyoumei.cn

[B01] 条件判断 if / else
来源：http://mwf.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hnn.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fji.zhongyouzk.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dhh.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cry.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://awh.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://utv.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jtn.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kcz.yongpay.top

[B02] 多分支 else if / elif
来源：http://lte.vehdjk.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xwx.dianchejie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xut.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://osn.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ral.xuanzx.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgu.hnqzz.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nmf.dianchejie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lrg.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kwc.pengpengdd.cyou

[B03] switch / match / case
来源：http://wip.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zyk.shzxlz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yad.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mht.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uzj.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://taf.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://txn.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ifx.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ura.zhongyouzk.top

[B04] for 计数循环
来源：http://fxa.uphjek.com

Py:   for i in range(10): print(i)
来源：http://inf.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mqp.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xeh.gaohongyu789.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ler.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://luz.jlsjyb.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://khh.kuanghao11.cn

Ruby: 10.times { |i| puts i }
来源：http://izw.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://inl.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://huf.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://csx.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bhy.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://djt.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dqh.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jby.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ygf.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://mtk.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cmo.cashguo.top

[B06] 遍历字典 / 对象
来源：http://rej.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hzd.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://onj.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nlb.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://viv.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fca.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xyq.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ith.yonumen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oiv.sysykeji.top

[B07] while 循环
来源：http://hac.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://oii.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://shh.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://ngb.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://ler.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://dgh.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tbm.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://ajw.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://qex.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://zaw.zhengqikj.top

Py:   # 无 do-while：用 while True + break
来源：http://prz.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://itc.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://aqn.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://lzu.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://wju.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rrc.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://pgy.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://pgd.ppjwa.cn

[B09] break 与 continue
来源：http://sqq.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mmb.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dqo.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbp.feifeiyinyue.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqu.sufxvd.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjm.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lum.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gej.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhy.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://khm.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uyn.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jlw.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ygi.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gxq.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mfu.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aky.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cej.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zsl.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://wdz.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://mvv.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://lnh.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://spv.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vun.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vhh.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://reo.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://mcr.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wgw.zhongyouzk.top

[B12] 跳出多层循环
来源：http://idz.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lyo.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ejo.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dvu.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://off.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://knv.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rqb.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gyv.daxiang520.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hrd.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://nbi.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://bye.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://ari.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zic.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fxs.feifeiyinyue.top

Java: x instanceof Number
来源：http://emk.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nxw.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://lpd.yvedp.cn

C#:   x is int or double or decimal
来源：http://cqo.fzhhl.top

[B14] 判断值是否在集合内
来源：http://tzs.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gma.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aby.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://gnx.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://loe.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cia.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nng.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://pvt.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://you.cashguo.top

[B15] 布尔运算与取反
来源：http://dcc.nwbrower.top

Py:   a and b or not c
来源：http://ebq.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://fvi.chenlongwang.top

JS:   a && b || !c
来源：http://wrq.cheryme.top

TS:   a && b || !c
来源：http://wmf.vqdsnc.cn

Java: a && b || !c
来源：http://uog.wangshuangyany.cn

Go:   a && b || !c
来源：http://ubb.zhiwuduotai.top

Ruby: a && b || !c
来源：http://wjn.9152youxi.cn

C#:   a && b || !c
来源：http://htv.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nid.guannengcc.top

Py:   if not data: return
来源：http://hjq.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://lxp.meibo888.top

JS:   if (!data) return;
来源：http://uyi.zhiwuduotai.top

TS:   if (!data) return;
来源：http://yal.zhoulong.xyz

Java: if (data == null) return;
来源：http://bww.svipenyu.cn

Go:   if data == nil { return }
来源：http://hvi.yongpay.top

Ruby: return if data.nil?
来源：http://rsx.jinqigfzy.top

C#:   if (data == null) return;
来源：http://bvc.shanyushiyangkeji.top

================================================================================
来源：http://jan.guannengcc.top

C. 函数与作用域
来源：http://zum.aibaodan.cn

================================================================================
来源：http://kjp.fengsongda.top

[C01] 定义函数
来源：http://ros.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://snm.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nvl.fehbvm.com

JS:   function add(a, b) { return a + b; }
来源：http://pyk.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sdq.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rse.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://vpl.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://lad.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rav.meibo888.top

[C02] 默认参数
来源：http://qsr.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://jjj.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jas.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://vjk.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ynk.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yji.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://swj.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://msr.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://ktk.shuidangran.top

[C03] 可变参数
来源：http://eyd.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://jkz.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lwg.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vnh.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jeb.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vbr.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jzh.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://jfl.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://akv.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://ewq.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zry.sufxvd.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xar.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kqb.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cgr.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://tde.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://rkz.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://oyz.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://tsa.cqqwz.cn

[C05] 返回多个值
来源：http://dcl.gaohongyu789.top

Py:   return a, b
来源：http://zuo.hammf.cn

PHP:  return [$a, $b];
来源：http://dzp.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jbr.yuxming.cn

TS:   return { a, b };
来源：http://uhj.yongpay.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wht.gzhubu.top

Go:   return a, b
来源：http://trg.vqdsnc.cn

Ruby: return a, b
来源：http://htz.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://ouf.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://kup.yueranfly.top

Py:   square = lambda x: x * x
来源：http://zqj.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uzi.bjfxy.top

JS:   const square = x => x * x;
来源：http://zhz.dianchejie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ahh.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://skw.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://dwd.yj202588.top

Ruby: square = ->(x) { x * x }
来源：http://skt.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bfd.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://oiz.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ixn.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://rif.c1oappe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://awm.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://qle.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yuh.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ing.redwolf501.top


<!-- 参考信息 -->