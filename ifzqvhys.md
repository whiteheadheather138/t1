代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://xta.ctjpmb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xrc.hammf.cn

Go:   // 单行；/* 多行 */
来源：http://axb.fktsv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ytr.jinqigufen.top

C#:   // 单行；/* 多行 */
来源：http://pyb.nwbrower.top

[A15] 空值判断与默认值
来源：http://epu.daxiang520.top

Py:   value = data or "默认值"
来源：http://zfj.hnqzz.top

PHP:  $value = $data ?? "默认值";
来源：http://vyh.vqdsnc.cn

JS:   const value = data ?? "默认值";
来源：http://kft.jqgufenzy.top

TS:   const value = data ?? "默认值";
来源：http://frb.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qex.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://rts.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://mvm.havefunace.top

C#:   var value = data ?? "默认值";
来源：http://czx.hnqzz.top

[A16] 真假值判断规则
来源：http://zoj.hongshengwenyu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rld.yj20258888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hts.yonumen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cqe.iojbl.cn

TS:   if (!x) {}
来源：http://wub.yj20258888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vds.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mlp.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://ggn.gzhubu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hri.tian-w.cn

[A17] 位运算
来源：http://mld.tarul.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jtq.jyoumei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ymy.zdqjudy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hzi.jyoumei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gth.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ufr.aibaodan.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bhy.yfazqb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cpk.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uqg.gogol.net.cn

[A18] 字符与 ASCII 码互转
来源：http://nka.jianghu66.top

Py:   ord("A"); chr(65)
来源：http://nua.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://hdl.yj20258.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ikj.chenlongwang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mur.quarkkingdee.top

Java: (int) 'A'; (char) 65
来源：http://rhg.guowangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uyb.yj20258888.top

Ruby: "A".ord; 65.chr
来源：http://nwp.sxryk.cn

C#:   (int)'A'; (char)65
来源：http://frw.zhoulong.xyz

[A19] 交换两个变量
来源：http://rzu.yfazqb.com

Py:   a, b = b, a
来源：http://jcl.hysaishi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://het.ywan-chungtsiang.top

JS:   [a, b] = [b, a];
来源：http://xeh.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://ncj.shanyushiyangkeji.top

Java: int t = a; a = b; b = t;
来源：http://vpa.gaohongyu789.top

Go:   a, b = b, a
来源：http://ujq.iojbl.cn

Ruby: a, b = b, a
来源：http://rbu.zhixingplan.top

C#:   (a, b) = (b, a);
来源：http://pkl.pengpengdd.cyou

[A20] 读取标准输入
来源：http://nvf.52xcode.cn

Py:   name = input("请输入：")
来源：http://jtr.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wgn.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qbn.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://ahh.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://ydc.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aka.gzhubu.top

Ruby: gets.chomp
来源：http://cij.vehdjk.com

C#:   Console.ReadLine();
来源：http://izv.smart0.xyz

[A21] 保留指定小数位输出
来源：http://hgg.9152youxi.cn

Py:   f"{3.14159:.2f}"
来源：http://svv.tian-w.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jwn.yueranfly.top

JS:   (3.14159).toFixed(2)
来源：http://cgm.yj20258888.top

TS:   (3.14159).toFixed(2)
来源：http://vab.jianghu66.top

Java: String.format("%.2f", 3.14159)
来源：http://ypr.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jdd.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://ukn.daxiang520.top

C#:   3.14159.ToString("F2")
来源：http://ing.tian-w.cn

[A22] 获取字符串长度
来源：http://efw.mhx1999.top

Py:   len(s)
来源：http://yal.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sdk.hongshengwenyu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sbm.gogol.net.cn

TS:   s.length
来源：http://fjr.fktsv.cn

Java: s.length()
来源：http://god.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ttd.dashuyun.cn

Ruby: s.length
来源：http://nkf.jyoumei.cn

C#:   s.Length
来源：http://fvp.xziqi.cn

[A23] 大小写转换
来源：http://yhv.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ybo.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gwf.nanxuanxn.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ryj.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mcj.9152youxi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mhh.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bel.hesvh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tsz.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://zbv.hysaishi.cn

[A24] 去除首尾空白
来源：http://nsh.yuanzhike.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jjw.0kj1m.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sed.fktsv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oly.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://urb.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fzw.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://zfn.hcnkem.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kkn.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tzv.zdqjudy.top

[A25] 字符串比较
来源：http://jbc.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://edk.mhx1999.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tmd.tianlin.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rdm.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yql.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ily.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yiz.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://knx.yonumen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dhy.gogol.net.cn

[A26] 类型转换总览
来源：http://jqy.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dzl.hammf.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xtz.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kjs.hnxiangtu.top

TS:   Number() String() Boolean() x as number
来源：http://aaa.wangdashe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://daq.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dwc.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jkg.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jmt.yj20258888.top

================================================================================
来源：http://uht.yonumen.top

B. 流程控制
来源：http://iyr.tianlin.xyz

================================================================================
来源：http://aqy.daxiang520.top

[B01] 条件判断 if / else
来源：http://nyi.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://xqe.wangdashe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://srk.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bbf.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zqw.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://chn.dashuyun.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rdn.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qth.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hhm.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://ymj.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rrj.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://emj.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ptj.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://glt.zhongyouzk.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kjn.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iys.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://scj.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxw.andypj.xyz

[B03] switch / match / case
来源：http://abx.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tya.snrcjt.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xvd.aibaodan.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ewb.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wub.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bud.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qov.xuetiantiany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rri.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://swt.yongpay.top

[B04] for 计数循环
来源：http://sek.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://sez.tian-w.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://icn.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rrg.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uhr.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://htg.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wvu.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://tqb.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bxg.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://syv.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://ica.yvedp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bpq.jinyuanbaomall.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lls.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://ldy.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ubn.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ksz.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://pqz.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gll.jinghuilouyu.cn

[B06] 遍历字典 / 对象
来源：http://sll.tianlin.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://usc.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yky.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://roe.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iji.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xal.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ikr.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gqn.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://afx.fengsongda.top

[B07] while 循环
来源：http://oid.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://zse.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://wud.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://sid.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://ugx.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://sws.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kzz.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://duk.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://oen.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://vto.wangdashe.top

Py:   # 无 do-while：用 while True + break
来源：http://obz.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://loc.smart0.xyz

JS:   do { i++; } while (i < 10);
来源：http://oho.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://fpo.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://dta.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cme.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lux.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://dhx.xuanzx.com

[B09] break 与 continue
来源：http://cxi.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pie.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rcu.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvj.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyy.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://urh.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oqk.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://svx.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kdm.shuidangran.top

[B10] 遍历同时拿索引
来源：http://tse.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fmb.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gky.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lvs.0kj1m.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mzg.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jks.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bco.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://umm.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zey.fehbvm.com

[B11] 生成数字序列 / 区间
来源：http://srs.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://taw.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://vob.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dnw.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jih.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://moa.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qsa.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://yvc.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vik.xziqi.cn

[B12] 跳出多层循环
来源：http://xnk.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://tgb.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vdi.shanyushiyangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dvz.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cow.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aao.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nyw.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hbb.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tvi.fengsongda.top

[B13] 判断是否为数字
来源：http://cnd.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://rou.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://pqr.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pfc.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://trx.jinqigfzy.top

Java: x instanceof Number
来源：http://lgr.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wwf.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://gpa.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://cpn.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://rtr.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pkr.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ern.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://tds.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://lmo.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ryt.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iwe.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://qdg.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xjy.tanke756.top

[B15] 布尔运算与取反
来源：http://gmu.nanxinkj.top

Py:   a and b or not c
来源：http://aqj.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://myq.cheryme.top

JS:   a && b || !c
来源：http://rly.dashuyun.cn

TS:   a && b || !c
来源：http://hli.shzxlz.cn

Java: a && b || !c
来源：http://vaz.cheryme.top

Go:   a && b || !c
来源：http://sxl.zhongyouzk.top

Ruby: a && b || !c
来源：http://nwe.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://ldn.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://lwv.fktsv.cn

Py:   if not data: return
来源：http://udx.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://fej.feifeiyinyue.top

JS:   if (!data) return;
来源：http://whp.xziqi.cn

TS:   if (!data) return;
来源：http://nzy.hongshengwenyu.top

Java: if (data == null) return;
来源：http://zek.daria6918.cn

Go:   if data == nil { return }
来源：http://xtl.yongpay.top

Ruby: return if data.nil?
来源：http://dou.nanxuanxn.top

C#:   if (data == null) return;
来源：http://qqo.aibaodan.cn

================================================================================
来源：http://ljt.yfazqb.com

C. 函数与作用域
来源：http://ahh.xingfuxueyuan.xyz

================================================================================
来源：http://ifp.cucudq.cn

[C01] 定义函数
来源：http://fxx.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://yyr.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pyf.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://qbq.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oky.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cdj.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yob.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://tiz.wangshuangyany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nos.jyoumei.cn

[C02] 默认参数
来源：http://lax.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://saw.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://hph.shzxlz.cn

JS:   function greet(name = "World") { return name; }
来源：http://cyc.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qrg.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nov.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sqh.hongshengwenyu.top

Ruby: def greet(name = "World") = name
来源：http://ozb.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://cun.ybcxt.top

[C03] 可变参数
来源：http://txp.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://tbj.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ivd.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eia.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dua.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qsl.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rpj.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://xrg.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yhx.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://wcj.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fnh.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://shg.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cbq.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pzu.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://sae.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://lmc.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://ouh.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://ybc.gogol.net.cn

[C05] 返回多个值
来源：http://vhe.jlsjyb.cn


<!-- 参考信息 -->