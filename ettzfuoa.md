代发 wailian999

Py:   "第一行\n第二行"
来源：http://kqm.tanke756.top

PHP:  "第一行\n第二行"
来源：http://ayc.yueranfly.top

JS:   "第一行\n第二行"
来源：http://cmu.zhoulong.xyz

TS:   "第一行\n第二行"
来源：http://ljl.shangyingyoupin.top

Java: "第一行\n第二行"
来源：http://fxr.redwolf501.top

Go:   "第一行\n第二行"
来源：http://svn.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://npe.hnqzz.top

C#:   "第一行\n第二行"
来源：http://fmb.jinyuanbaomall.cn

[A14] 注释写法
来源：http://kme.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dga.svipenyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nme.cdnleiting.top

JS:   // 单行；/* 多行 */
来源：http://omp.guowangkeji.top

TS:   // 单行；/* 多行 */
来源：http://rjk.haohaochexian.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bje.smart0.xyz

Go:   // 单行；/* 多行 */
来源：http://yqr.zhiwuduotai.top

Ruby: # 单行；=begin 多行 =end
来源：http://jqj.meibo888.top

C#:   // 单行；/* 多行 */
来源：http://cus.ehwqpu.com

[A15] 空值判断与默认值
来源：http://jkx.vqdsnc.cn

Py:   value = data or "默认值"
来源：http://plv.zhiwuduotai.top

PHP:  $value = $data ?? "默认值";
来源：http://wwd.yuanzhike.top

JS:   const value = data ?? "默认值";
来源：http://xoq.gzhubu.top

TS:   const value = data ?? "默认值";
来源：http://fyq.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wsz.gzhubu.top

Go:   if data == "" { data = "默认值" }
来源：http://fip.shangyingyoupin.top

Ruby: value = data || "默认值"
来源：http://wjw.yuanzhike.top

C#:   var value = data ?? "默认值";
来源：http://zaz.pycfn.com

[A16] 真假值判断规则
来源：http://rjj.shzxlz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oui.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pxh.daria6918.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fun.mhx1999.top

TS:   if (!x) {}
来源：http://cnj.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yeg.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sqo.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tij.daxiang520.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ria.jqgufenzy.top

[A17] 位运算
来源：http://tqn.bjfxy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://njy.sufxvd.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nrw.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iqe.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rsy.iojbl.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jfv.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xbf.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ufu.andypj.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vmd.yonumen.top

[A18] 字符与 ASCII 码互转
来源：http://vyw.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://xrs.pengpengdd.cyou

PHP:  ord("A"); chr(65)
来源：http://fai.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rbo.jqgufenzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lbh.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://guf.sysykeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ghr.epnwcf.com

Ruby: "A".ord; 65.chr
来源：http://laj.iojbl.cn

C#:   (int)'A'; (char)65
来源：http://jhj.shuidangran.top

[A19] 交换两个变量
来源：http://orb.aizwys.cn

Py:   a, b = b, a
来源：http://vbb.xuetiantiany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://knv.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://myk.fengsongda.top

TS:   [a, b] = [b, a];
来源：http://fdm.wangdashe.top

Java: int t = a; a = b; b = t;
来源：http://xuq.jinqigfzy.top

Go:   a, b = b, a
来源：http://jks.pycfn.com

Ruby: a, b = b, a
来源：http://xii.daria6918.cn

C#:   (a, b) = (b, a);
来源：http://qis.gaohongyu789.top

[A20] 读取标准输入
来源：http://kdk.yangfankeji.com

Py:   name = input("请输入：")
来源：http://myj.pengpengdd.cyou

PHP:  $name = trim(fgets(STDIN));
来源：http://rbi.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wdt.mhx1999.top

TS:   // Node.js：readline 模块
来源：http://utq.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://ugf.gaohongyu789.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rrh.cheryme.top

Ruby: gets.chomp
来源：http://esl.hammf.cn

C#:   Console.ReadLine();
来源：http://snx.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://lzm.chenjidiqi.icu

Py:   f"{3.14159:.2f}"
来源：http://bmr.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wmg.daxiang520.top

JS:   (3.14159).toFixed(2)
来源：http://lgb.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://mht.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://wac.nanxinkj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uvd.jinyuanbaomall.cn

Ruby: format("%.2f", 3.14159)
来源：http://ill.hnqzz.top

C#:   3.14159.ToString("F2")
来源：http://kwu.sjlbkw.cn

[A22] 获取字符串长度
来源：http://alr.kuanghao11.cn

Py:   len(s)
来源：http://uop.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lfh.hfpthk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cal.fktsv.cn

TS:   s.length
来源：http://ekw.316326.xyz

Java: s.length()
来源：http://bpy.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bev.hammf.cn

Ruby: s.length
来源：http://eyw.dianchejie.cn

C#:   s.Length
来源：http://giv.aizwys.cn

[A23] 大小写转换
来源：http://fgv.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ssh.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gjp.bbcook.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lml.sjlbkw.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wae.jqgfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fmy.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://prk.kuanghao11.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ern.uphjek.com

C#:   s.ToUpper(); s.ToLower()
来源：http://eca.ivvv.top

[A24] 去除首尾空白
来源：http://acd.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yys.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kox.fehbvm.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ieb.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://odn.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xyf.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://tqt.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cpo.tianlin.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://azh.chenzaomai.com

[A25] 字符串比较
来源：http://sbx.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://hcw.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bsd.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zkx.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cvo.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rbv.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fly.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wwi.tanke756.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fol.fktsv.cn

[A26] 类型转换总览
来源：http://zxr.ivvv.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://imc.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://smr.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rbj.chenlongwang.top

TS:   Number() String() Boolean() x as number
来源：http://mqn.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zqf.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lqa.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://jsw.uphjek.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vln.yj20258.top

================================================================================
来源：http://swn.yj20258.top

B. 流程控制
来源：http://xlc.fzhhl.top

================================================================================
来源：http://jer.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://sio.nanxinkj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fib.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rft.9152youxi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wfc.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hpf.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kzm.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xnv.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nog.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://var.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://ikc.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bzk.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mmh.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ciu.iojbl.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xji.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://acb.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://atd.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vut.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgr.xylfe.cn

[B03] switch / match / case
来源：http://vds.fanxiaobao.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bqr.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://els.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yfl.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zrj.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nwh.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mft.guannengcc.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kxz.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fte.uphjek.com

[B04] for 计数循环
来源：http://zkb.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://nmq.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://moo.gotoacloud.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tbv.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvz.zycfv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bnw.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sho.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://rnd.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blx.sjlbkw.cn

[B05] 遍历数组 / 列表
来源：http://bbe.zycfv.cn

Py:   for item in arr: print(item)
来源：http://trh.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tgu.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lgg.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tkr.gotoacloud.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pdm.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pyr.yuanzhike.top

Ruby: arr.each { |item| puts item }
来源：http://dhn.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ndl.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://vnk.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://upi.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mru.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ifm.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zou.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jdb.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lqs.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qjp.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rmm.wangdashe.top

[B07] while 循环
来源：http://fwz.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://ksj.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://xvo.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://mlm.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://arx.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://ici.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gki.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://jfm.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://hfw.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://ayc.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://urk.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oql.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://iib.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://thz.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://ivj.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iqg.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://wmw.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://typ.yj20258888.top

[B09] break 与 continue
来源：http://iab.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lju.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rjy.daria6918.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://way.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syy.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kzn.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://buk.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mwg.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxt.xylfe.cn

[B10] 遍历同时拿索引
来源：http://yan.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cyg.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cls.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ybp.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ahz.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vvf.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fjm.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vod.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lxf.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://cwz.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://kgz.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://who.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://szk.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggd.zhongyouzk.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yke.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gah.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://ngo.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sid.sweek.top

[B12] 跳出多层循环
来源：http://qtw.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://slc.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uhy.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ujy.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rjh.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ybd.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qfp.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mwt.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ykp.bjfxy.top

[B13] 判断是否为数字
来源：http://pld.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://fmc.fktsv.cn

PHP:  is_numeric($x)
来源：http://vui.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qsj.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://boy.nanxinkj.top

Java: x instanceof Number
来源：http://qji.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rek.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://vtm.fehbvm.com

C#:   x is int or double or decimal
来源：http://dbb.ivvv.top

[B14] 判断值是否在集合内
来源：http://cxd.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uhr.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yiv.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://hdm.jianghu66.top

TS:   [1, 2, 3].includes(x)
来源：http://wlq.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kjr.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cgw.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://ilh.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vih.tian-w.cn

[B15] 布尔运算与取反
来源：http://xlq.jinqigufen.top

Py:   a and b or not c
来源：http://dsw.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://vql.daria6918.cn

JS:   a && b || !c
来源：http://jqh.shuidangran.top

TS:   a && b || !c
来源：http://uai.fehbvm.com

Java: a && b || !c
来源：http://gtp.tian-w.cn

Go:   a && b || !c
来源：http://yuf.zdbjq.cn

Ruby: a && b || !c
来源：http://frd.sjlbkw.cn

C#:   a && b || !c
来源：http://dds.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://jcb.hywenlv.cn

Py:   if not data: return
来源：http://jsf.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://joe.yanxiufei.cn

JS:   if (!data) return;
来源：http://kgp.yj20258.top

TS:   if (!data) return;
来源：http://bsf.dashuyun.cn

Java: if (data == null) return;
来源：http://svx.ybcxt.top

Go:   if data == nil { return }
来源：http://cne.cqqwz.cn

Ruby: return if data.nil?
来源：http://dxo.xinyue.icu

C#:   if (data == null) return;
来源：http://xjy.pengpengdd.cyou

================================================================================
来源：http://psc.vehdjk.com

C. 函数与作用域
来源：http://nli.nanxinkj.top

================================================================================
来源：http://gkm.gzhubu.top

[C01] 定义函数
来源：http://dum.cashguo.top

Py:   def add(a, b): return a + b
来源：http://zuw.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zvc.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ibl.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oke.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qbx.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://afw.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://bjk.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iio.xuetiantiany.cn

[C02] 默认参数
来源：http://cxf.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://xup.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kui.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://ujn.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gdj.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bri.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://odx.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://zgf.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://tbz.chenlongwang.top

[C03] 可变参数
来源：http://eco.pycfn.com

Py:   def total(*args): return sum(args)
来源：http://hme.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aps.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lwb.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yrx.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kpk.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://whn.yongpay.top


<!-- 参考信息 -->