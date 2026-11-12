代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://bkk.hcnkem.com

TS:   const value = data ?? "默认值";
来源：http://xoo.bjfxy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bkg.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://snx.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://vpl.cdnleiting.top

C#:   var value = data ?? "默认值";
来源：http://dud.jinqigfzy.top

[A16] 真假值判断规则
来源：http://aju.shangyingyoupin.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jwt.gzhubu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mku.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zdb.tarul.cn

TS:   if (!x) {}
来源：http://utn.bjfxy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uqi.hywenlv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ejn.svipenyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rlm.jiagoushi.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fjc.xinyue.icu

[A17] 位运算
来源：http://zjj.gotoacloud.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cqn.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tht.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iiw.snrcjt.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ajh.hnqzz.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bid.andypj.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tnn.shanyushiyangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://evh.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvm.aizwys.cn

[A18] 字符与 ASCII 码互转
来源：http://dej.epnwcf.com

Py:   ord("A"); chr(65)
来源：http://umq.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://ydv.iojbl.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hpj.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hlk.ivvv.top

Java: (int) 'A'; (char) 65
来源：http://tas.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qzg.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://ocp.sjlbkw.cn

C#:   (int)'A'; (char)65
来源：http://lhd.zhijiandao.cn

[A19] 交换两个变量
来源：http://ztn.52xcode.cn

Py:   a, b = b, a
来源：http://vel.jiagoushi.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nzp.9152youxi.cn

JS:   [a, b] = [b, a];
来源：http://yfd.zhongyouzk.top

TS:   [a, b] = [b, a];
来源：http://pvt.sjlbkw.cn

Java: int t = a; a = b; b = t;
来源：http://zjb.jyoumei.cn

Go:   a, b = b, a
来源：http://nug.c1oappe.top

Ruby: a, b = b, a
来源：http://cwm.wangdashe.top

C#:   (a, b) = (b, a);
来源：http://ubo.feifeiyinyue.top

[A20] 读取标准输入
来源：http://mtu.c1oappe.top

Py:   name = input("请输入：")
来源：http://fkm.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ydh.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yag.gogol.net.cn

TS:   // Node.js：readline 模块
来源：http://daf.xingfuxueyuan.xyz

Java: new Scanner(System.in).nextLine()
来源：http://qrn.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://brj.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://etc.ppjwa.cn

C#:   Console.ReadLine();
来源：http://vly.wangshuangyany.cn

[A21] 保留指定小数位输出
来源：http://ezq.tian-w.cn

Py:   f"{3.14159:.2f}"
来源：http://yjl.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qnj.xuanzx.com

JS:   (3.14159).toFixed(2)
来源：http://wez.hnqzz.top

TS:   (3.14159).toFixed(2)
来源：http://hjt.daria6918.cn

Java: String.format("%.2f", 3.14159)
来源：http://dti.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dhf.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://nrb.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://xlh.jinghuilouyu.cn

[A22] 获取字符串长度
来源：http://jpd.fktsv.cn

Py:   len(s)
来源：http://qxp.hcnkem.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://avl.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kmr.sufxvd.cn

TS:   s.length
来源：http://vye.hesvh.cn

Java: s.length()
来源：http://thz.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zbu.shuidangran.top

Ruby: s.length
来源：http://huu.shanyushiyangtech.top

C#:   s.Length
来源：http://sii.zhijiandao.cn

[A23] 大小写转换
来源：http://xhj.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ugm.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ezk.ctjpmb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qao.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zwo.bjfxy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tok.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bxd.xinyue.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://odj.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cff.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://uhi.aibaodan.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qkz.cucudq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pru.xinyue.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ils.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ayn.guowangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ykl.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://ifb.zycfv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://smq.hywenlv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://joj.yj20258888.top

[A25] 字符串比较
来源：http://ygg.havefunace.top

Py:   s1 == s2; s1 != s2
来源：http://kpn.cdnleiting.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mas.cheryme.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iky.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jcc.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tfd.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eju.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aaq.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nrm.iojbl.cn

[A26] 类型转换总览
来源：http://ilj.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mfy.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nqm.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://isi.xylfe.cn

TS:   Number() String() Boolean() x as number
来源：http://etn.nanxinkj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cbx.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ngg.hesvh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rtq.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://opw.9152youxi.cn

================================================================================
来源：http://bks.yueranfly.top

B. 流程控制
来源：http://swb.jinyuanbaomall.cn

================================================================================
来源：http://iey.bbcook.cn

[B01] 条件判断 if / else
来源：http://bqm.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://eiq.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kzz.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://psa.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ved.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ceu.chenzaomai.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tdu.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kzi.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rce.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://mqf.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zvm.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wmt.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xur.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xii.pengpengdd.cyou

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ktw.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://khr.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dnn.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yxj.gaohongyu789.top

[B03] switch / match / case
来源：http://dni.yuanzhike.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rfu.c1oappe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tzh.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hex.zhoulong.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tel.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://doq.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nri.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gme.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ncy.cheryme.top

[B04] for 计数循环
来源：http://kyk.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://yyg.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oon.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bbs.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nqc.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jzf.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zdp.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://xwi.hnxiangtu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ltx.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://wzj.aizwys.cn

Py:   for item in arr: print(item)
来源：http://klb.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eus.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://ajt.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://tis.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://gow.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://smu.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://fev.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://erh.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://ocu.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://tdv.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://siv.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ryj.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sxc.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://igd.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://npd.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jca.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iju.uphjek.com

[B07] while 循环
来源：http://agc.sysykeji.top

Py:   while i < 10: i += 1
来源：http://mjm.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://mbq.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://qkx.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://ehl.ivvv.top

Java: while (i < 10) { i++; }
来源：http://vpb.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://voz.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://tos.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://aij.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://yca.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://fhn.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://skp.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://wjm.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://qvb.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://zig.meibo888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hka.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fca.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://iww.zhiwuduotai.top

[B09] break 与 continue
来源：http://fer.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lnn.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yhg.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpp.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sxd.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://btk.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uqv.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nbn.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://klq.daria6918.cn

[B10] 遍历同时拿索引
来源：http://prq.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ask.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hll.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pkj.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nod.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hmz.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wpz.vehdjk.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yvy.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zdl.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://jpp.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://jcj.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://wnw.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rqr.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lrr.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cth.havefunace.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oeq.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://xjo.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://llj.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://ekx.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zjl.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://aml.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bvb.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nmz.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xmz.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fbb.fengsongda.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aff.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://thf.vehdjk.com

[B13] 判断是否为数字
来源：http://tam.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://yun.jiagoushi.top

PHP:  is_numeric($x)
来源：http://zow.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sir.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gkk.9152youxi.cn

Java: x instanceof Number
来源：http://ram.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fac.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://ktg.jiagoushi.top

C#:   x is int or double or decimal
来源：http://eyr.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://esf.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://stt.ydjk.org.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cpa.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://jqw.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://csp.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gkb.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gre.shuidangran.top

Ruby: [1, 2, 3].include?(x)
来源：http://zoi.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://muj.yj202588.top

[B15] 布尔运算与取反
来源：http://qkd.ppjwa.cn

Py:   a and b or not c
来源：http://vyf.ybcxt.top

PHP:  $a && $b || !$c
来源：http://afx.shuidangran.top

JS:   a && b || !c
来源：http://bdn.andypj.xyz

TS:   a && b || !c
来源：http://naw.ppjwa.cn

Java: a && b || !c
来源：http://rqc.hysaishi.cn

Go:   a && b || !c
来源：http://gpg.iojbl.cn

Ruby: a && b || !c
来源：http://xzv.shangyingyoupin.top

C#:   a && b || !c
来源：http://jul.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qup.yj20258.top

Py:   if not data: return
来源：http://xtj.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://kef.sweek.top

JS:   if (!data) return;
来源：http://bgw.yj20258.top

TS:   if (!data) return;
来源：http://kvv.jianghu66.top

Java: if (data == null) return;
来源：http://zxk.cheryme.top

Go:   if data == nil { return }
来源：http://pmo.quarkkingdee.top

Ruby: return if data.nil?
来源：http://jdk.jianghu66.top

C#:   if (data == null) return;
来源：http://dwm.52xcode.cn

================================================================================
来源：http://xua.shzxlz.cn

C. 函数与作用域
来源：http://cnh.fktsv.cn

================================================================================
来源：http://cfd.jyoumei.cn

[C01] 定义函数
来源：http://eyw.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://ggk.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yjv.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://ykb.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jhw.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hdj.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ygq.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://zby.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kuk.tarul.cn

[C02] 默认参数
来源：http://exk.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://dmn.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dlk.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://mpb.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://iwz.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://zbm.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zam.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://vgp.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://ryk.snrcjt.cn

[C03] 可变参数
来源：http://hmj.snrcjt.cn

Py:   def total(*args): return sum(args)
来源：http://jzb.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dwt.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://seu.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nim.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xcs.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gvq.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qvz.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ehm.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://vbu.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gyh.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://osk.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cxr.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fhp.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://qpg.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://qoe.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://qjc.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://gzf.pengpengdd.cyou

[C05] 返回多个值
来源：http://pnt.zdbjq.cn

Py:   return a, b
来源：http://qjr.xziqi.cn

PHP:  return [$a, $b];
来源：http://qti.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ccv.jinghuilouyu.cn

TS:   return { a, b };
来源：http://whh.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tsg.jinqigfzy.top

Go:   return a, b
来源：http://qwb.jianghu66.top

Ruby: return a, b
来源：http://jyl.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://jpw.jinyuanbaomall.cn


<!-- 参考信息 -->