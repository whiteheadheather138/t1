代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://til.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://lyl.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jqf.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://nyz.meibo888.top

Ruby: value = data || "默认值"
来源：http://chg.yangfankeji.com

C#:   var value = data ?? "默认值";
来源：http://lck.jinghuilouyu.cn

[A16] 真假值判断规则
来源：http://tec.zycfv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ogt.yvedp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kpb.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://itp.zycfv.cn

TS:   if (!x) {}
来源：http://rme.chenjidiqi.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tme.zycfv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yzz.redwolf501.top

Ruby: unless x            # nil 与 false 为假
来源：http://zeh.hfpthk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ofx.ywan-chungtsiang.top

[A17] 位运算
来源：http://jkw.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bvq.jinqigufen.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://igg.tarul.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcp.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bzx.daria6918.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://knb.52xcode.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tgl.jqgufenzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lpb.chenlongwang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kks.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://sdz.yongpay.top

Py:   ord("A"); chr(65)
来源：http://mlr.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://pke.epnwcf.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ckn.kuanghao11.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nto.tian-w.cn

Java: (int) 'A'; (char) 65
来源：http://cxg.zhiwuduotai.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tuk.vqdsnc.cn

Ruby: "A".ord; 65.chr
来源：http://dwu.jiagoushi.top

C#:   (int)'A'; (char)65
来源：http://fhm.jqgfzy.top

[A19] 交换两个变量
来源：http://hsp.zhengqikj.top

Py:   a, b = b, a
来源：http://fij.xuanzx.com

PHP:  [$a, $b] = [$b, $a];
来源：http://wdm.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://fsv.meibo888.top

TS:   [a, b] = [b, a];
来源：http://wrc.gogol.net.cn

Java: int t = a; a = b; b = t;
来源：http://goz.jinqigufen.top

Go:   a, b = b, a
来源：http://mnl.zhongyouzk.top

Ruby: a, b = b, a
来源：http://sos.jiagoushi.top

C#:   (a, b) = (b, a);
来源：http://nzo.xuanzx.com

[A20] 读取标准输入
来源：http://tif.shuidangran.top

Py:   name = input("请输入：")
来源：http://xly.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ksh.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uvf.hfpthk.cn

TS:   // Node.js：readline 模块
来源：http://wqs.pycfn.com

Java: new Scanner(System.in).nextLine()
来源：http://kzt.jlsjyb.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fzl.zhongyouzk.top

Ruby: gets.chomp
来源：http://kjv.haohaochexian.top

C#:   Console.ReadLine();
来源：http://ock.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://akn.jinqigfzy.top

Py:   f"{3.14159:.2f}"
来源：http://bsh.shangyingyoupin.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ieb.sweek.top

JS:   (3.14159).toFixed(2)
来源：http://vte.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://jjz.cucudq.cn

Java: String.format("%.2f", 3.14159)
来源：http://plg.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vnv.jqgufenzy.top

Ruby: format("%.2f", 3.14159)
来源：http://upj.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://bzn.havefunace.top

[A22] 获取字符串长度
来源：http://xuy.dianchejie.cn

Py:   len(s)
来源：http://kiz.shanyushiyangtech.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jkv.hfpthk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mio.ctjpmb.com

TS:   s.length
来源：http://dhy.bjfxy.top

Java: s.length()
来源：http://zmm.fktsv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lbt.tianlin.xyz

Ruby: s.length
来源：http://fio.yonumen.top

C#:   s.Length
来源：http://sbn.haohaochexian.top

[A23] 大小写转换
来源：http://psx.jiagoushi.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nyq.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cqb.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vqh.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xxk.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sbc.dianchejie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eci.bbcook.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fnd.jinqigfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vho.chenlongwang.top

[A24] 去除首尾空白
来源：http://rhz.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jdn.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qjv.sysykeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xji.gaohongyu789.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ygm.aibaodan.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wya.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://yxw.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://izg.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pca.bjfxy.top

[A25] 字符串比较
来源：http://dyw.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://sjn.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://znr.nwbrower.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://slc.zhengqikj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jcm.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fao.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://moi.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ohi.aibaodan.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lrf.shzxlz.cn

[A26] 类型转换总览
来源：http://rxi.bjfxy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://auj.ppjwa.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://use.jyoumei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ndz.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://ymn.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://osy.cheryme.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://drb.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ayi.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fhv.vqdsnc.cn

================================================================================
来源：http://kfm.shangyingyoupin.top

B. 流程控制
来源：http://pnn.gogol.net.cn

================================================================================
来源：http://mwa.fehbvm.com

[B01] 条件判断 if / else
来源：http://fuj.yueranfly.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hsu.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aqt.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cqx.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lrs.gaohongyu789.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://laa.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bxa.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dzo.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dtn.yj202588.top

[B02] 多分支 else if / elif
来源：http://lhq.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://azz.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vhb.zdbjq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aav.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gsy.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jup.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hqv.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://efp.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jry.sxryk.cn

[B03] switch / match / case
来源：http://jxm.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xeo.hcnkem.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mus.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kxr.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hfj.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://edy.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wox.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://msf.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tsd.fzhhl.top

[B04] for 计数循环
来源：http://wat.fktsv.cn

Py:   for i in range(10): print(i)
来源：http://pfl.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hpm.hesvh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://puo.xingfuxueyuan.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tnc.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kdo.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bqo.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://yqf.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uoi.iojbl.cn

[B05] 遍历数组 / 列表
来源：http://uhr.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://owh.zhengqikj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rrx.havefunace.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fyt.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iwu.daxiang520.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ymn.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hzm.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://fyf.svipenyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xsq.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://tgp.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pyw.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sdb.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mpr.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uid.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gvg.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lfw.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cjq.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qme.guannengcc.top

[B07] while 循环
来源：http://wol.xylfe.cn

Py:   while i < 10: i += 1
来源：http://gyy.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qbc.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://wdx.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://prv.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://oso.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://smt.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://jby.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://zpu.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://zjs.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://klv.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://lbw.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://gxc.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://xfu.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://uua.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wyl.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://pau.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://mlp.zdqjudy.top

[B09] break 与 continue
来源：http://ehk.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bba.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nej.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bvy.dashuyun.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sxg.guannengcc.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ckz.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qtd.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://akl.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qui.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://pum.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ggd.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lzc.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oej.0kj1m.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ddf.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cnf.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aco.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kcd.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://giz.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://avz.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://kxx.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://uem.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jto.guannengcc.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nld.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lbj.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://stl.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://vze.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qtv.birdmap.top

[B12] 跳出多层循环
来源：http://qml.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yha.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://vcu.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wco.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tbh.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nbz.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jql.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ktz.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ijm.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://idk.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://poh.wangdashe.top

PHP:  is_numeric($x)
来源：http://hiw.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gio.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ghl.daxiang520.top

Java: x instanceof Number
来源：http://iwz.tianlin.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zuc.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://nbl.smart0.xyz

C#:   x is int or double or decimal
来源：http://trm.jqgfzy.top

[B14] 判断值是否在集合内
来源：http://whc.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xty.cheryme.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://urn.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://rpg.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://kcx.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zak.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wwg.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://ebf.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iry.cqqwz.cn

[B15] 布尔运算与取反
来源：http://dxx.bjfxy.top

Py:   a and b or not c
来源：http://gjv.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://wpr.hammf.cn

JS:   a && b || !c
来源：http://jmv.zycfv.cn

TS:   a && b || !c
来源：http://hjd.jqgfzy.top

Java: a && b || !c
来源：http://was.ybcxt.top

Go:   a && b || !c
来源：http://bzx.andypj.xyz

Ruby: a && b || !c
来源：http://aqj.hcnkem.com

C#:   a && b || !c
来源：http://ikh.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://udi.jinqigufen.top

Py:   if not data: return
来源：http://sie.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://uhb.bbcook.cn

JS:   if (!data) return;
来源：http://srs.yj20258888.top

TS:   if (!data) return;
来源：http://zyy.zhixingplan.top

Java: if (data == null) return;
来源：http://bry.uphjek.com

Go:   if data == nil { return }
来源：http://lsq.bjfxy.top

Ruby: return if data.nil?
来源：http://jqj.zhengqikj.top

C#:   if (data == null) return;
来源：http://spo.feifeiyinyue.top

================================================================================
来源：http://kae.hywenlv.cn

C. 函数与作用域
来源：http://ios.haohaochexian.top

================================================================================
来源：http://aoj.xziqi.cn

[C01] 定义函数
来源：http://exn.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://mrv.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wik.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://viy.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fgw.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zpl.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://gtn.ybcxt.top

Ruby: def add(a, b); a + b; end
来源：http://gmy.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cai.fengsongda.top

[C02] 默认参数
来源：http://rmn.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://aqh.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ipe.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://nbe.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://itq.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xeo.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zsd.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://aii.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://fmb.nanxuanxn.top

[C03] 可变参数
来源：http://kss.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://gkz.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://irx.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ian.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://twu.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wbi.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sqa.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://zka.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://elm.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://jjq.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ohp.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://slc.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vrv.hammf.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://afn.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://odw.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://pdg.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://lqh.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://tja.cheryme.top

[C05] 返回多个值
来源：http://jml.zhongyouzk.top

Py:   return a, b
来源：http://ppk.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://coi.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vuq.yj20258.top

TS:   return { a, b };
来源：http://vdw.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jwj.yj20258.top

Go:   return a, b
来源：http://tro.gaohongyu789.top

Ruby: return a, b
来源：http://pci.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://oiz.xuanzx.com


<!-- 参考信息 -->