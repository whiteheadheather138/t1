代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tac.snrcjt.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://meu.vqdsnc.cn

TS:   if (!x) {}
来源：http://ieg.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hfl.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://trs.chenzaomai.com

Ruby: unless x            # nil 与 false 为假
来源：http://bve.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sej.ctjpmb.com

[A17] 位运算
来源：http://cuv.gzhubu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://akf.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gsb.xuetiantiany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xxe.fengsongda.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baf.hongshengwenyu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://umn.yuxming.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tqn.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xpg.shanyushiyangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ymw.jinyuanbaomall.cn

[A18] 字符与 ASCII 码互转
来源：http://ksu.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://tvo.iojbl.cn

PHP:  ord("A"); chr(65)
来源：http://zjh.meibo888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://irw.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jaq.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://gqh.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rmo.tian-w.cn

Ruby: "A".ord; 65.chr
来源：http://msl.snrcjt.cn

C#:   (int)'A'; (char)65
来源：http://gql.gzhubu.top

[A19] 交换两个变量
来源：http://gdk.epnwcf.com

Py:   a, b = b, a
来源：http://dmj.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://vio.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://yvf.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://cmc.haohaochexian.top

Java: int t = a; a = b; b = t;
来源：http://wqh.tarul.cn

Go:   a, b = b, a
来源：http://vsw.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://sls.zhijiandao.cn

C#:   (a, b) = (b, a);
来源：http://nof.yvedp.cn

[A20] 读取标准输入
来源：http://bdk.zhengqikj.top

Py:   name = input("请输入：")
来源：http://fin.quarkkingdee.top

PHP:  $name = trim(fgets(STDIN));
来源：http://csb.sysykeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mco.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://thn.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://mzf.sweek.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://awn.jinghuilouyu.cn

Ruby: gets.chomp
来源：http://eql.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://wyy.dianchejie.cn

[A21] 保留指定小数位输出
来源：http://apx.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://ydk.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qqx.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://qlz.316326.xyz

TS:   (3.14159).toFixed(2)
来源：http://jsp.hfpthk.cn

Java: String.format("%.2f", 3.14159)
来源：http://xqn.shuidangran.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ffq.jiagoushi.top

Ruby: format("%.2f", 3.14159)
来源：http://rtf.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://moa.jlsjyb.cn

[A22] 获取字符串长度
来源：http://cmx.bjfxy.top

Py:   len(s)
来源：http://efd.jianghu66.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sqn.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bkv.cucudq.cn

TS:   s.length
来源：http://vah.quarkkingdee.top

Java: s.length()
来源：http://xsg.sjlbkw.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eib.sysykeji.top

Ruby: s.length
来源：http://dmn.jiagoushi.top

C#:   s.Length
来源：http://cuv.gzhubu.top

[A23] 大小写转换
来源：http://rul.ywan-chungtsiang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bpf.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oll.uphjek.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lan.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qty.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mwq.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zwq.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gra.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://huj.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://zrd.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jag.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vqx.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://czd.hnqzz.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cwu.nanxinkj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lqb.bbcook.cn

Go:   strings.TrimSpace(s)
来源：http://tna.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nwd.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fhg.gotoacloud.top

[A25] 字符串比较
来源：http://ecd.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://khi.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ebc.nanxuanxn.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fcs.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wqu.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eyy.yfazqb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yra.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://plq.0kj1m.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://khb.shangyingyoupin.top

[A26] 类型转换总览
来源：http://sjy.cucudq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hrp.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gwl.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://arp.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://rzf.zycfv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://teu.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gvb.redwolf501.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://aqi.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wqq.aizwys.cn

================================================================================
来源：http://tre.hnxiangtu.top

B. 流程控制
来源：http://let.zhijiandao.cn

================================================================================
来源：http://fwr.kuanghao11.cn

[B01] 条件判断 if / else
来源：http://xmb.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://alh.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yem.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ixh.ydzc1.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://trb.gaohongyu789.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://spk.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bnx.dashuyun.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cpo.svipenyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hjk.hcnkem.com

[B02] 多分支 else if / elif
来源：http://qou.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uqb.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://toi.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yct.yvedp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djy.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wno.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tll.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://doo.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hoo.svipenyu.cn

[B03] switch / match / case
来源：http://rlj.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://beo.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fez.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://utf.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kvv.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gza.birdmap.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tbz.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://siw.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zpq.xziqi.cn

[B04] for 计数循环
来源：http://eqn.yj20258.top

Py:   for i in range(10): print(i)
来源：http://wfo.fzhhl.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qrw.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://exk.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sgu.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pod.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://odw.jinyuanbaomall.cn

Ruby: 10.times { |i| puts i }
来源：http://ikk.haohaochexian.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tgz.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://vpl.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://sar.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hgz.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uqf.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fpl.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ath.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qfu.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://oxu.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nkn.cheryme.top

[B06] 遍历字典 / 对象
来源：http://skq.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gkz.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iab.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mad.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uzy.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oqy.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sme.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aav.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qxn.9152youxi.cn

[B07] while 循环
来源：http://kxv.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://lkq.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://imm.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://cag.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://uwz.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://gvv.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gnw.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://rto.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://swp.yj20258.top

[B08] do-while（至少执行一次）
来源：http://krh.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://olo.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://mhs.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://sna.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://jbd.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://uur.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bez.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ikh.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://osp.dianchejie.cn

[B09] break 与 continue
来源：http://phs.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vsx.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://obr.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pik.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldl.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tve.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xxf.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dwo.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihh.daxiang520.top

[B10] 遍历同时拿索引
来源：http://zmh.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://czt.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ppv.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kbf.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jne.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zor.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://odn.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qxk.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tey.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://aru.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://zfp.yongpay.top

PHP:  range(0, 10, 2);
来源：http://mah.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://flk.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zij.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pfq.ydzc1.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nnz.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://ssg.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lmq.daxiang520.top

[B12] 跳出多层循环
来源：http://gcw.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fhk.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hpk.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://trs.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://epq.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tnr.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gcf.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://djn.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nnt.hnxiangtu.top

[B13] 判断是否为数字
来源：http://jzn.kuanghao11.cn

Py:   isinstance(x, (int, float))
来源：http://iso.hysaishi.cn

PHP:  is_numeric($x)
来源：http://ydh.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rnm.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qkj.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://pzf.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jet.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://kaj.zhengqikj.top

C#:   x is int or double or decimal
来源：http://bxo.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://mzr.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vya.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nfm.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://hob.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://mvq.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://whq.cdnleiting.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jui.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yun.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zak.52xcode.cn

[B15] 布尔运算与取反
来源：http://qwk.nwbrower.top

Py:   a and b or not c
来源：http://kjx.xuanzx.com

PHP:  $a && $b || !$c
来源：http://dmt.ctjpmb.com

JS:   a && b || !c
来源：http://rnl.wangdashe.top

TS:   a && b || !c
来源：http://ncc.yongpay.top

Java: a && b || !c
来源：http://lmy.tian-w.cn

Go:   a && b || !c
来源：http://znh.gotoacloud.top

Ruby: a && b || !c
来源：http://wbb.c1oappe.top

C#:   a && b || !c
来源：http://ymr.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://dwu.redwolf501.top

Py:   if not data: return
来源：http://jmt.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://yel.jinqigfzy.top

JS:   if (!data) return;
来源：http://rxg.cashguo.top

TS:   if (!data) return;
来源：http://gij.zdbjq.cn

Java: if (data == null) return;
来源：http://tvk.zhixingplan.top

Go:   if data == nil { return }
来源：http://mup.fengsongda.top

Ruby: return if data.nil?
来源：http://jot.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://uhe.52xcode.cn

================================================================================
来源：http://puk.316326.xyz

C. 函数与作用域
来源：http://hxx.ehwqpu.com

================================================================================
来源：http://zji.fehbvm.com

[C01] 定义函数
来源：http://dml.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://fjd.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bmr.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://ehl.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ujs.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mim.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://vec.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://xvf.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xuc.nwbrower.top

[C02] 默认参数
来源：http://gec.meibo888.top

Py:   def greet(name="World"): return name
来源：http://fhj.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://opj.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://wxm.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mfu.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ppq.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nid.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://ovw.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://hmh.chenjidiqi.icu

[C03] 可变参数
来源：http://fht.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://vly.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bbd.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mcr.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hlj.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yhu.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://orj.tanke756.top

Ruby: def total(*nums); nums.sum; end
来源：http://qxq.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hib.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://anz.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hfp.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kpc.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lqb.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rtg.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://skf.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://vpl.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://orj.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://xnr.bjfxy.top

[C05] 返回多个值
来源：http://ism.snrcjt.cn

Py:   return a, b
来源：http://swx.fehbvm.com

PHP:  return [$a, $b];
来源：http://ujo.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://jau.hnxiangtu.top

TS:   return { a, b };
来源：http://rsl.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lch.daxiang520.top

Go:   return a, b
来源：http://aeg.cashguo.top

Ruby: return a, b
来源：http://qho.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://cym.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://fkq.birdmap.top

Py:   square = lambda x: x * x
来源：http://cej.vehdjk.com

PHP:  $square = fn($x) => $x * $x;
来源：http://svf.meibo888.top

JS:   const square = x => x * x;
来源：http://jck.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://bmy.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ahw.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://qwr.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://qtw.mhx1999.top


<!-- 参考信息 -->