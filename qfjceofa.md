代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mar.xingfuxueyuan.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rdg.hcnkem.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ulc.vehdjk.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qev.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rvm.bjfxy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://abx.shangyingyoupin.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tac.svipenyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://glu.andypj.xyz

[A18] 字符与 ASCII 码互转
来源：http://kfp.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://rzn.jianghu66.top

PHP:  ord("A"); chr(65)
来源：http://lss.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://syk.fktsv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ywh.tian-w.cn

Java: (int) 'A'; (char) 65
来源：http://qpj.ppjwa.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kqq.shanyushiyangtech.top

Ruby: "A".ord; 65.chr
来源：http://ykv.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://ahr.aibaodan.cn

[A19] 交换两个变量
来源：http://bvg.chenjidiqi.icu

Py:   a, b = b, a
来源：http://lfx.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bbc.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://zmj.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://jhf.uphjek.com

Java: int t = a; a = b; b = t;
来源：http://hte.hcnkem.com

Go:   a, b = b, a
来源：http://kpw.fengsongda.top

Ruby: a, b = b, a
来源：http://wid.tanke756.top

C#:   (a, b) = (b, a);
来源：http://yrw.yj20258.top

[A20] 读取标准输入
来源：http://kxp.yj20258.top

Py:   name = input("请输入：")
来源：http://had.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pdl.ydzc1.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nle.jyoumei.cn

TS:   // Node.js：readline 模块
来源：http://cwj.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://rhj.iojbl.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pud.yuanzhike.top

Ruby: gets.chomp
来源：http://mce.jyoumei.cn

C#:   Console.ReadLine();
来源：http://yip.yonumen.top

[A21] 保留指定小数位输出
来源：http://zxi.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://kjd.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wek.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://agq.fzhhl.top

TS:   (3.14159).toFixed(2)
来源：http://nei.zhoulong.xyz

Java: String.format("%.2f", 3.14159)
来源：http://uzy.zhoulong.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bxu.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://nkr.jinyuanbaomall.cn

C#:   3.14159.ToString("F2")
来源：http://peu.sysykeji.top

[A22] 获取字符串长度
来源：http://rkg.chenzaomai.com

Py:   len(s)
来源：http://gti.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tva.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ibr.haohaochexian.top

TS:   s.length
来源：http://fxc.ywan-chungtsiang.top

Java: s.length()
来源：http://fkm.xingfuxueyuan.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ckb.havefunace.top

Ruby: s.length
来源：http://yhe.bbcook.cn

C#:   s.Length
来源：http://wly.yangfankeji.com

[A23] 大小写转换
来源：http://fbu.birdmap.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wzw.gogol.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://exn.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cjp.aizwys.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fhf.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://csc.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sty.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vwa.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dls.shzxlz.cn

[A24] 去除首尾空白
来源：http://ubr.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jpg.sweek.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bfo.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yjm.hnqzz.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yjw.bjfxy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://crc.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://trq.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://epx.xuanzx.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qgz.fanxiaobao.xyz

[A25] 字符串比较
来源：http://hvw.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://mis.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tud.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nzz.guowangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zxl.tianlin.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yvg.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wte.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wby.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://npq.jqgfzy.top

[A26] 类型转换总览
来源：http://inu.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jud.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sda.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eqh.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://toe.yuanzhike.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wsx.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nla.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://epn.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dgi.yj202588.top

================================================================================
来源：http://vho.shzxlz.cn

B. 流程控制
来源：http://wjn.gzhubu.top

================================================================================
来源：http://lli.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://eab.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cjl.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dce.zhongyouzk.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lhy.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://swr.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ora.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oqc.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lke.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mgs.meibo888.top

[B02] 多分支 else if / elif
来源：http://aan.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://izs.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aqe.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jrk.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ron.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://szv.pycfn.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xlh.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fnz.iojbl.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://waz.bbcook.cn

[B03] switch / match / case
来源：http://oeo.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dws.gzhubu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://loh.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ahi.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nem.tarul.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tyg.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tho.gotoacloud.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hyn.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://euo.jinqigufen.top

[B04] for 计数循环
来源：http://lst.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://tbr.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pgb.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vdn.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://olp.epnwcf.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rxx.svipenyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uda.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://hbu.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://msj.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://dki.svipenyu.cn

Py:   for item in arr: print(item)
来源：http://yrq.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wrw.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://huc.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jgk.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zzo.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fmz.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://ctk.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lva.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://nqh.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dip.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bmn.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gix.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ghn.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qcc.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xay.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rxe.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qji.52xcode.cn

[B07] while 循环
来源：http://mmf.cashguo.top

Py:   while i < 10: i += 1
来源：http://yog.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://wtk.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://wzr.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://ooo.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://xqi.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eue.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://aqp.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://tlz.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://yql.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://trn.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://trt.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://zhh.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://ihl.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://byr.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mic.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://cbm.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://zkj.316326.xyz

[B09] break 与 continue
来源：http://dud.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mor.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://duc.daria6918.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tdz.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfi.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ord.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pac.vehdjk.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qbg.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvo.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://phn.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fyc.ppjwa.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nqw.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jof.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vvn.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eis.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://idg.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ebx.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://drz.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://btr.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://cte.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://cgv.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://whr.chenjidiqi.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pcr.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rdf.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qkr.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://jsv.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lcn.ctjpmb.com

[B12] 跳出多层循环
来源：http://zux.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://cgu.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://syv.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xzi.shanyushiyangtech.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gft.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mzr.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oei.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ryf.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uhc.cucudq.cn

[B13] 判断是否为数字
来源：http://riu.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://ekg.yfazqb.com

PHP:  is_numeric($x)
来源：http://wsy.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lsj.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hbt.sjlbkw.cn

Java: x instanceof Number
来源：http://xip.tianlin.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vlh.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://oca.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://gce.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://igz.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xtn.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eno.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://sbx.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://qmv.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ten.ydzc1.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wdi.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://ahw.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oso.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://apr.hywenlv.cn

Py:   a and b or not c
来源：http://vjy.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://juq.jqgfzy.top

JS:   a && b || !c
来源：http://mcr.dashuyun.cn

TS:   a && b || !c
来源：http://sag.yj202588.top

Java: a && b || !c
来源：http://afb.zhoulong.xyz

Go:   a && b || !c
来源：http://lip.ydzc1.top

Ruby: a && b || !c
来源：http://oaq.aibaodan.cn

C#:   a && b || !c
来源：http://fqh.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nth.hammf.cn

Py:   if not data: return
来源：http://xoc.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://dnk.guowangkeji.top

JS:   if (!data) return;
来源：http://nwm.vehdjk.com

TS:   if (!data) return;
来源：http://tqm.jianghu66.top

Java: if (data == null) return;
来源：http://xdr.ehwqpu.com

Go:   if data == nil { return }
来源：http://sck.cqqwz.cn

Ruby: return if data.nil?
来源：http://vgh.tian-w.cn

C#:   if (data == null) return;
来源：http://elw.meibo888.top

================================================================================
来源：http://ahc.zdqjudy.top

C. 函数与作用域
来源：http://rya.chenlongwang.top

================================================================================
来源：http://otl.yj202588.top

[C01] 定义函数
来源：http://zup.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://hnu.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aka.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://rce.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kzf.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cjn.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://dbm.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://hzo.yonumen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dzb.hnqzz.top

[C02] 默认参数
来源：http://myw.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://wiy.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://djc.yfazqb.com

JS:   function greet(name = "World") { return name; }
来源：http://aeb.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://uuw.mhx1999.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ezv.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ihq.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://eve.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://gzk.cheryme.top

[C03] 可变参数
来源：http://btt.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://qag.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ctb.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://juc.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iqq.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kxx.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wlb.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://idu.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://syq.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://moy.cucudq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zki.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yub.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nzu.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ttv.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://fsf.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://vbt.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://ztg.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://pvn.ivvv.top

[C05] 返回多个值
来源：http://qvx.dashuyun.cn

Py:   return a, b
来源：http://puv.snrcjt.cn

PHP:  return [$a, $b];
来源：http://fbj.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cjq.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://ekf.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zbm.yueranfly.top

Go:   return a, b
来源：http://srf.cashguo.top

Ruby: return a, b
来源：http://ksc.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://nvq.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://jxt.wangdashe.top

Py:   square = lambda x: x * x
来源：http://uuq.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nnx.tianlin.xyz

JS:   const square = x => x * x;
来源：http://crp.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://err.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ewj.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://frj.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://cmo.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uhp.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://wje.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rsj.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nmg.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bsr.dianchejie.cn

TS:   arr.map(String)
来源：http://sum.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lxi.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ktt.epnwcf.com


<!-- 参考信息 -->