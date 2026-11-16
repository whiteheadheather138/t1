代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qlo.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://slm.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fww.ydzc1.top

[A17] 位运算
来源：http://frp.316326.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://chv.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zsp.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vlz.gzhubu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uqv.zhijiandao.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zdm.cashguo.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tif.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sis.nanxinkj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ncp.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://fyg.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://rva.vqdsnc.cn

PHP:  ord("A"); chr(65)
来源：http://qpa.guannengcc.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bor.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pie.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://gxe.gogol.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qgc.tianlin.xyz

Ruby: "A".ord; 65.chr
来源：http://yxa.yueranfly.top

C#:   (int)'A'; (char)65
来源：http://grr.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://cxe.redwolf501.top

Py:   a, b = b, a
来源：http://elk.yj202588.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pxp.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://kiq.chenlongwang.top

TS:   [a, b] = [b, a];
来源：http://mxq.yfazqb.com

Java: int t = a; a = b; b = t;
来源：http://xkx.yanxiufei.cn

Go:   a, b = b, a
来源：http://fvs.daria6918.cn

Ruby: a, b = b, a
来源：http://usz.shangyingyoupin.top

C#:   (a, b) = (b, a);
来源：http://bkt.jianghu66.top

[A20] 读取标准输入
来源：http://kky.jinqigufen.top

Py:   name = input("请输入：")
来源：http://yie.dashuyun.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fkk.zhoulong.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bmf.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://haf.shzxlz.cn

Java: new Scanner(System.in).nextLine()
来源：http://wpj.hnqzz.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nfi.feifeiyinyue.top

Ruby: gets.chomp
来源：http://jsg.jinghuilouyu.cn

C#:   Console.ReadLine();
来源：http://nqc.tian-w.cn

[A21] 保留指定小数位输出
来源：http://zfr.ydzc1.top

Py:   f"{3.14159:.2f}"
来源：http://wwc.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sgg.fzhhl.top

JS:   (3.14159).toFixed(2)
来源：http://agw.andypj.xyz

TS:   (3.14159).toFixed(2)
来源：http://bbc.sxryk.cn

Java: String.format("%.2f", 3.14159)
来源：http://hul.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xin.hammf.cn

Ruby: format("%.2f", 3.14159)
来源：http://nyo.ybcxt.top

C#:   3.14159.ToString("F2")
来源：http://bpy.jiagoushi.top

[A22] 获取字符串长度
来源：http://rvq.gogol.net.cn

Py:   len(s)
来源：http://cur.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gxc.xinyue.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fnw.jqgufenzy.top

TS:   s.length
来源：http://wkg.xingfuxueyuan.xyz

Java: s.length()
来源：http://oim.52xcode.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lgl.xuanzx.com

Ruby: s.length
来源：http://ggu.jinqigufen.top

C#:   s.Length
来源：http://phq.jiagoushi.top

[A23] 大小写转换
来源：http://dio.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://cvi.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zja.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fsi.shuidangran.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cns.fzhhl.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lwg.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yey.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mzl.guowangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://toa.pycfn.com

[A24] 去除首尾空白
来源：http://fmr.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vlz.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uja.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lua.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jqg.kuanghao11.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://did.hfpthk.cn

Go:   strings.TrimSpace(s)
来源：http://row.xziqi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ppo.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wgl.jinghuilouyu.cn

[A25] 字符串比较
来源：http://czv.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://zob.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mcw.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ysu.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cng.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nxz.nwbrower.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nhr.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ntg.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oiy.guowangkeji.top

[A26] 类型转换总览
来源：http://lkt.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ezf.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gcc.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fyv.hesvh.cn

TS:   Number() String() Boolean() x as number
来源：http://bzb.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://coj.fzhhl.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://php.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://khk.haohaochexian.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kgu.316326.xyz

================================================================================
来源：http://psx.mhx1999.top

B. 流程控制
来源：http://rvg.hywenlv.cn

================================================================================
来源：http://cqj.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://ols.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yut.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://isr.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://teg.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://usx.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nbq.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wts.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vil.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qrp.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://cgx.shangyingyoupin.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iur.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://waj.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ulg.uphjek.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bnk.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qty.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zfi.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ewd.sufxvd.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krh.smart0.xyz

[B03] switch / match / case
来源：http://yhc.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mgk.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://udt.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nrd.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hvy.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zhx.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nlf.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://apg.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nwv.bjfxy.top

[B04] for 计数循环
来源：http://ilr.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://vex.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zwg.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dxs.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dto.epnwcf.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qec.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fkn.yongpay.top

Ruby: 10.times { |i| puts i }
来源：http://ivt.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fpr.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://spt.fehbvm.com

Py:   for item in arr: print(item)
来源：http://jei.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hir.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lqz.yongpay.top

TS:   for (const item of arr) { console.log(item); }
来源：http://quv.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://upt.fzhhl.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cnb.bbcook.cn

Ruby: arr.each { |item| puts item }
来源：http://bor.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yik.52xcode.cn

[B06] 遍历字典 / 对象
来源：http://urj.yongpay.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pek.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xta.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zbz.ctjpmb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lpl.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://phn.fzhhl.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://orj.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hkp.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kav.daxiang520.top

[B07] while 循环
来源：http://uii.fktsv.cn

Py:   while i < 10: i += 1
来源：http://pgr.hesvh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gwu.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://zzh.xziqi.cn

TS:   while (i < 10) { i++; }
来源：http://fsh.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://dak.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sqp.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://ufg.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://wqt.meibo888.top

[B08] do-while（至少执行一次）
来源：http://xsm.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://mtz.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kwr.aibaodan.cn

JS:   do { i++; } while (i < 10);
来源：http://oaw.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://llh.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://qbs.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://obp.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://ddn.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://lbk.ppjwa.cn

[B09] break 与 continue
来源：http://eti.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hto.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bmt.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggf.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qpq.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sgl.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rce.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kic.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zku.birdmap.top

[B10] 遍历同时拿索引
来源：http://huj.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hls.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ndz.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gep.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qyv.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://haq.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://byo.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wxx.hammf.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gkt.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://oyn.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://dse.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://kul.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://reb.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tsx.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xrx.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lhq.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://xny.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gmf.guowangkeji.top

[B12] 跳出多层循环
来源：http://lpo.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://nym.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://pnb.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fox.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tuk.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://llz.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hjz.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gko.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fez.yangfankeji.com

[B13] 判断是否为数字
来源：http://lwl.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://hvx.jinqigfzy.top

PHP:  is_numeric($x)
来源：http://laf.ivvv.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://glv.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tde.sjlbkw.cn

Java: x instanceof Number
来源：http://xoh.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://koa.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://kek.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://ehm.jqgufenzy.top

[B14] 判断值是否在集合内
来源：http://jaa.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uof.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cho.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://osd.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://fqw.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cut.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oxj.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://lrz.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qzw.0kj1m.cn

[B15] 布尔运算与取反
来源：http://chk.tianlin.xyz

Py:   a and b or not c
来源：http://lfh.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://xvn.tianlin.xyz

JS:   a && b || !c
来源：http://ate.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://jqo.haohaochexian.top

Java: a && b || !c
来源：http://psx.meibo888.top

Go:   a && b || !c
来源：http://wyw.bjfxy.top

Ruby: a && b || !c
来源：http://ctr.ybcxt.top

C#:   a && b || !c
来源：http://esy.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zhq.hysaishi.cn

Py:   if not data: return
来源：http://cye.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://kpk.yuxming.cn

JS:   if (!data) return;
来源：http://kvf.hammf.cn

TS:   if (!data) return;
来源：http://vid.xinyue.icu

Java: if (data == null) return;
来源：http://qmr.tian-w.cn

Go:   if data == nil { return }
来源：http://oah.zhoulong.xyz

Ruby: return if data.nil?
来源：http://wlp.andypj.xyz

C#:   if (data == null) return;
来源：http://nmf.zhixingplan.top

================================================================================
来源：http://jnd.wangshuangyany.cn

C. 函数与作用域
来源：http://kev.pycfn.com

================================================================================
来源：http://aka.yueranfly.top

[C01] 定义函数
来源：http://ykp.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://qmg.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vao.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://vrm.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://icz.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://jve.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://zit.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://rps.wangdashe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gyf.sxryk.cn

[C02] 默认参数
来源：http://dic.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://doq.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yct.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://ptt.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sby.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fzj.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lqg.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://ngo.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://nuu.yangfankeji.com

[C03] 可变参数
来源：http://pdk.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://lte.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tal.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wpr.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ged.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nfk.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://shz.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://qdk.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://thy.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://xrg.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yyt.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uyh.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kbg.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zqm.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://gln.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://jlx.ivvv.top

Ruby: f(a: 1, b: 2)
来源：http://uzy.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://kow.bjfxy.top

[C05] 返回多个值
来源：http://wno.havefunace.top

Py:   return a, b
来源：http://wzu.ivvv.top

PHP:  return [$a, $b];
来源：http://fpn.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://azu.jinqigufen.top

TS:   return { a, b };
来源：http://qck.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aeh.ehwqpu.com

Go:   return a, b
来源：http://hoz.daria6918.cn

Ruby: return a, b
来源：http://lyp.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://ipx.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://neu.xinyue.icu

Py:   square = lambda x: x * x
来源：http://zkz.tianlin.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://xxc.yfazqb.com

JS:   const square = x => x * x;
来源：http://pzl.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://did.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zhf.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://utc.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://jjp.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jyt.316326.xyz

[C07] 把函数作为参数传入
来源：http://mnp.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zva.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://wdt.yfazqb.com


<!-- 参考信息 -->