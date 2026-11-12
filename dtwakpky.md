代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iph.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://yjm.hammf.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yab.zhaomingkeji.xyz

[A17] 位运算
来源：http://hcx.ybcxt.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rps.jinqigufen.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tye.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gcx.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nqu.yongpay.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qcq.birdmap.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://det.jinghuilouyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rol.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dyj.zycfv.cn

[A18] 字符与 ASCII 码互转
来源：http://nha.jyoumei.cn

Py:   ord("A"); chr(65)
来源：http://aks.shanyushiyangtech.top

PHP:  ord("A"); chr(65)
来源：http://utj.pengpengdd.cyou

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cxb.52xcode.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tal.cqqwz.cn

Java: (int) 'A'; (char) 65
来源：http://xcf.birdmap.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nuo.xingfuxueyuan.xyz

Ruby: "A".ord; 65.chr
来源：http://gic.tanke756.top

C#:   (int)'A'; (char)65
来源：http://zmm.zdqjudy.top

[A19] 交换两个变量
来源：http://avu.redwolf501.top

Py:   a, b = b, a
来源：http://buo.bbcook.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pci.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://icr.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://ufl.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://ozu.ivvv.top

Go:   a, b = b, a
来源：http://gci.sweek.top

Ruby: a, b = b, a
来源：http://fyl.fehbvm.com

C#:   (a, b) = (b, a);
来源：http://mxy.yonumen.top

[A20] 读取标准输入
来源：http://epk.shuidangran.top

Py:   name = input("请输入：")
来源：http://axb.fzhhl.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tey.xylfe.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hek.gotoacloud.top

TS:   // Node.js：readline 模块
来源：http://hro.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://khm.yj202588.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pzj.hesvh.cn

Ruby: gets.chomp
来源：http://ina.jqgfzy.top

C#:   Console.ReadLine();
来源：http://exb.meibo888.top

[A21] 保留指定小数位输出
来源：http://mrk.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://mfd.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lpc.shangyingyoupin.top

JS:   (3.14159).toFixed(2)
来源：http://phi.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://xla.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://rhg.sweek.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jmp.snrcjt.cn

Ruby: format("%.2f", 3.14159)
来源：http://muo.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://nnb.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://pea.yuanzhike.top

Py:   len(s)
来源：http://kzd.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mba.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ehr.andypj.xyz

TS:   s.length
来源：http://ppk.hfpthk.cn

Java: s.length()
来源：http://fbz.fzhhl.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tpz.nanxinkj.top

Ruby: s.length
来源：http://zvf.yanxiufei.cn

C#:   s.Length
来源：http://dgf.chenjidiqi.icu

[A23] 大小写转换
来源：http://kxn.haohaochexian.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kbr.havefunace.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nbr.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dmf.zhongyouzk.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zma.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ozf.yj202588.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rsb.chenjidiqi.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sln.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uac.kuanghao11.cn

[A24] 去除首尾空白
来源：http://hbp.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fbr.fanxiaobao.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://osi.sxryk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cjx.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jzp.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yda.ehwqpu.com

Go:   strings.TrimSpace(s)
来源：http://qry.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gby.ywan-chungtsiang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ixt.fzhhl.top

[A25] 字符串比较
来源：http://yvz.fehbvm.com

Py:   s1 == s2; s1 != s2
来源：http://yqd.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fyb.yanxiufei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dma.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uvc.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xho.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jkr.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://snv.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cxg.zhixingplan.top

[A26] 类型转换总览
来源：http://nwn.shanyushiyangtech.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nnc.svipenyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://phi.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qcp.yj20258.top

TS:   Number() String() Boolean() x as number
来源：http://etp.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ucl.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lgx.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yto.dashuyun.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blf.nanxinkj.top

================================================================================
来源：http://qgt.svipenyu.cn

B. 流程控制
来源：http://vib.xuanzx.com

================================================================================
来源：http://gxr.xuanzx.com

[B01] 条件判断 if / else
来源：http://mkl.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tzo.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lro.fzhhl.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zsf.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nql.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nts.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cqb.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dxj.yanxiufei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://swl.wangdashe.top

[B02] 多分支 else if / elif
来源：http://trw.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xfn.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ixb.yuxming.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxn.yj20258.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://otf.c1oappe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ssj.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ixv.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zor.tarul.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wjk.uphjek.com

[B03] switch / match / case
来源：http://rma.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yhj.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zmh.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nqs.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kcj.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://udo.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://voo.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://exz.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iyk.cdnleiting.top

[B04] for 计数循环
来源：http://fgq.birdmap.top

Py:   for i in range(10): print(i)
来源：http://ifo.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://htl.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wyi.wangshuangyany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cti.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qwz.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mzq.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://wcv.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jyq.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://mdm.sxryk.cn

Py:   for item in arr: print(item)
来源：http://yun.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xeg.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://quh.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ttj.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bbg.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sdt.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://tqh.hongshengwenyu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mca.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://jdk.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tck.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zkn.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xza.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pcj.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xoi.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gtx.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lij.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lyz.meibo888.top

[B07] while 循环
来源：http://hoo.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://kyn.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://geo.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://iog.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://jge.jianghu66.top

Java: while (i < 10) { i++; }
来源：http://scc.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dao.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://luc.hywenlv.cn

C#:   while (i < 10) { i++; }
来源：http://cso.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://tat.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://wcr.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://voy.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://nru.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://mpb.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://eqv.gaohongyu789.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dnl.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ogg.feifeiyinyue.top

C#:   do { i++; } while (i < 10);
来源：http://vfi.haohaochexian.top

[B09] break 与 continue
来源：http://pdy.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dck.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jhh.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://glc.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hzq.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxt.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ail.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xfv.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rng.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://mwv.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ltk.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ill.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eub.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://usq.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://beg.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yoe.jinqigfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bqr.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://adx.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://joq.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://fct.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://oyf.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://goo.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xag.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bkb.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xxg.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://tgt.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kgk.vehdjk.com

[B12] 跳出多层循环
来源：http://dfu.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vpa.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bwg.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wzx.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fck.xziqi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tfc.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hna.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vqb.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ico.sysykeji.top

[B13] 判断是否为数字
来源：http://osa.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://ijq.cqqwz.cn

PHP:  is_numeric($x)
来源：http://rdn.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://juq.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wbi.hnxiangtu.top

Java: x instanceof Number
来源：http://kny.nanxinkj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zdh.hnqzz.top

Ruby: x.is_a?(Numeric)
来源：http://fvj.ivvv.top

C#:   x is int or double or decimal
来源：http://iqk.fzhhl.top

[B14] 判断值是否在集合内
来源：http://yek.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ibg.chenzaomai.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://anl.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://meq.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://olc.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lxf.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wav.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://ymj.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ftu.yangfankeji.com

[B15] 布尔运算与取反
来源：http://pjh.cdnleiting.top

Py:   a and b or not c
来源：http://ipz.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://fap.zhongyouzk.top

JS:   a && b || !c
来源：http://edc.kuanghao11.cn

TS:   a && b || !c
来源：http://fzp.nanxuanxn.top

Java: a && b || !c
来源：http://nji.xziqi.cn

Go:   a && b || !c
来源：http://ydg.epnwcf.com

Ruby: a && b || !c
来源：http://qge.gaohongyu789.top

C#:   a && b || !c
来源：http://byb.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://pmj.hongshengwenyu.top

Py:   if not data: return
来源：http://pnj.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://pwk.jiagoushi.top

JS:   if (!data) return;
来源：http://kxg.vqdsnc.cn

TS:   if (!data) return;
来源：http://opt.shanyushiyangtech.top

Java: if (data == null) return;
来源：http://mhr.52xcode.cn

Go:   if data == nil { return }
来源：http://ryo.redwolf501.top

Ruby: return if data.nil?
来源：http://gds.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://wtg.haohaochexian.top

================================================================================
来源：http://glk.sxryk.cn

C. 函数与作用域
来源：http://ivj.ehwqpu.com

================================================================================
来源：http://nuu.gaohongyu789.top

[C01] 定义函数
来源：http://kjh.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://dni.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kzm.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://nii.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://frn.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yfe.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ssy.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://cef.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dyd.yuxming.cn

[C02] 默认参数
来源：http://ijt.uphjek.com

Py:   def greet(name="World"): return name
来源：http://mno.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cfk.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://pfs.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dly.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://llu.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fpg.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://rdu.snrcjt.cn

C#:   string Greet(string name = "World") => name;
来源：http://lqi.hywenlv.cn

[C03] 可变参数
来源：http://vav.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://ung.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://swl.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qce.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vah.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rbf.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lcn.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://exp.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gkt.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://yxc.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://axx.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jom.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ufw.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wzn.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://lky.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://pia.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://ped.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://zsj.jlsjyb.cn

[C05] 返回多个值
来源：http://cim.gogol.net.cn

Py:   return a, b
来源：http://xdn.shuidangran.top

PHP:  return [$a, $b];
来源：http://vpq.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ysl.fzhhl.top

TS:   return { a, b };
来源：http://qls.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qdz.jlsjyb.cn

Go:   return a, b
来源：http://prl.hnxiangtu.top

Ruby: return a, b
来源：http://yeu.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://hkb.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://xpa.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://fkc.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uvn.zdbjq.cn

JS:   const square = x => x * x;
来源：http://mvf.zhoulong.xyz

TS:   const square = (x: number): number => x * x;
来源：http://xsf.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jcq.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tvk.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://svr.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://oss.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://ntz.hnxiangtu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yik.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://fmf.nanxuanxn.top


<!-- 参考信息 -->