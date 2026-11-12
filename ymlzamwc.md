代发 wailian999

Ruby: value = data || "默认值"
来源：http://ker.ywan-chungtsiang.top

C#:   var value = data ?? "默认值";
来源：http://rxt.dashuyun.cn

[A16] 真假值判断规则
来源：http://iyh.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dsu.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lyg.mhx1999.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jyk.sufxvd.cn

TS:   if (!x) {}
来源：http://oid.smart0.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lul.birdmap.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qjt.smart0.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://egm.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qxu.shzxlz.cn

[A17] 位运算
来源：http://xqv.yangfankeji.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hbf.yanxiufei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://icj.hnqzz.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gcp.zhixingplan.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cwm.gotoacloud.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vhh.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ynn.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dcm.fzhhl.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zjy.ywan-chungtsiang.top

[A18] 字符与 ASCII 码互转
来源：http://xat.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://edj.ydzc1.top

PHP:  ord("A"); chr(65)
来源：http://dwh.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ckl.pengpengdd.cyou

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lkh.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://fjf.yj20258888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vqe.sjlbkw.cn

Ruby: "A".ord; 65.chr
来源：http://ldz.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://wxf.nwbrower.top

[A19] 交换两个变量
来源：http://dol.316326.xyz

Py:   a, b = b, a
来源：http://ovz.svipenyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rde.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://kyh.jianghu66.top

TS:   [a, b] = [b, a];
来源：http://ocu.meibo888.top

Java: int t = a; a = b; b = t;
来源：http://pyu.316326.xyz

Go:   a, b = b, a
来源：http://dpg.0kj1m.cn

Ruby: a, b = b, a
来源：http://ngq.pycfn.com

C#:   (a, b) = (b, a);
来源：http://hfe.yvedp.cn

[A20] 读取标准输入
来源：http://wbh.zdqjudy.top

Py:   name = input("请输入：")
来源：http://bun.hfpthk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nnd.shangyingyoupin.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ixd.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://lpp.fengsongda.top

Java: new Scanner(System.in).nextLine()
来源：http://opm.wangdashe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rhn.jqgufenzy.top

Ruby: gets.chomp
来源：http://oux.fktsv.cn

C#:   Console.ReadLine();
来源：http://rgz.fehbvm.com

[A21] 保留指定小数位输出
来源：http://yey.xingfuxueyuan.xyz

Py:   f"{3.14159:.2f}"
来源：http://pbc.shanyushiyangtech.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://anp.zdqjudy.top

JS:   (3.14159).toFixed(2)
来源：http://rod.yj20258888.top

TS:   (3.14159).toFixed(2)
来源：http://vrn.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://sql.havefunace.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cvt.gotoacloud.top

Ruby: format("%.2f", 3.14159)
来源：http://qbo.iojbl.cn

C#:   3.14159.ToString("F2")
来源：http://ebs.guannengcc.top

[A22] 获取字符串长度
来源：http://khx.daxiang520.top

Py:   len(s)
来源：http://gcj.ydzc1.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ebv.yfazqb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lvt.jinghuilouyu.cn

TS:   s.length
来源：http://mvp.gotoacloud.top

Java: s.length()
来源：http://zjq.hcnkem.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uwz.mhx1999.top

Ruby: s.length
来源：http://sbq.9152youxi.cn

C#:   s.Length
来源：http://mcq.xylfe.cn

[A23] 大小写转换
来源：http://cfq.tian-w.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://izc.hnxiangtu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jab.birdmap.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aut.sxryk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sui.hongshengwenyu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yhz.hammf.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bzw.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://utl.kuanghao11.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vdr.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://gyb.gzhubu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jkd.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rqg.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fhn.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nwc.zdqjudy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tbt.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://fdo.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://glz.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pet.sysykeji.top

[A25] 字符串比较
来源：http://nqz.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://kwf.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uqo.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nmu.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ovu.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qhg.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kyz.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ixc.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blq.zdqjudy.top

[A26] 类型转换总览
来源：http://uon.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gjd.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jgx.guowangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qee.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://nqr.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xjk.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oii.iojbl.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://saz.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zrl.tarul.cn

================================================================================
来源：http://odk.aibaodan.cn

B. 流程控制
来源：http://ysr.pycfn.com

================================================================================
来源：http://hjg.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://odn.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mbb.fengsongda.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://roy.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dhi.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://opq.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uzz.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mmk.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qyz.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bai.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://wqh.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lti.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tju.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfs.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ait.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hhv.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rzp.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cuo.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ydm.snrcjt.cn

[B03] switch / match / case
来源：http://bfe.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iig.nanxinkj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sqh.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fts.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://edt.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fyj.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vpr.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://enf.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://auu.jlsjyb.cn

[B04] for 计数循环
来源：http://fpa.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://ord.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dlg.fanxiaobao.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rtl.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rmu.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xof.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mux.fzhhl.top

Ruby: 10.times { |i| puts i }
来源：http://ljw.xuanzx.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nin.ivvv.top

[B05] 遍历数组 / 列表
来源：http://rtf.52xcode.cn

Py:   for item in arr: print(item)
来源：http://utc.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ljt.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vsm.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bog.hysaishi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lsz.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ioz.hammf.cn

Ruby: arr.each { |item| puts item }
来源：http://dkh.sweek.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fuj.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://nkj.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wzt.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gdv.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rlz.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jrw.zdqjudy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rfb.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kii.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sxt.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://krl.c1oappe.top

[B07] while 循环
来源：http://yin.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://wma.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://hqi.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://rsg.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://lkq.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://onx.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://akc.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://gov.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://svs.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://gey.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://rmc.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gjt.pycfn.com

JS:   do { i++; } while (i < 10);
来源：http://iel.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://ftw.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://cbs.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://byy.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://vij.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://yev.zhengqikj.top

[B09] break 与 continue
来源：http://mmo.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qnb.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fem.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ecv.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://brp.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psd.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ekg.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ung.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddv.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://oxd.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ryv.sweek.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bwv.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lsr.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ufl.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jsl.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bjj.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://olz.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://moa.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://thq.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://nky.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://pry.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tqy.cqqwz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://unv.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ucz.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cta.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://wnj.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zkk.hysaishi.cn

[B12] 跳出多层循环
来源：http://xou.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nby.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://oxj.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vcr.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bgr.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zoj.xziqi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fvv.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wek.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wyw.gzhubu.top

[B13] 判断是否为数字
来源：http://sqp.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://jxw.fengsongda.top

PHP:  is_numeric($x)
来源：http://tcg.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://okm.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ocf.zhixingplan.top

Java: x instanceof Number
来源：http://ibb.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cso.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://cav.zhixingplan.top

C#:   x is int or double or decimal
来源：http://jyw.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://nqs.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rds.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ooc.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://qnm.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://cbt.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jxo.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lvr.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://atr.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ybr.yongpay.top

[B15] 布尔运算与取反
来源：http://xhl.xuanzx.com

Py:   a and b or not c
来源：http://gwg.daria6918.cn

PHP:  $a && $b || !$c
来源：http://tpu.9152youxi.cn

JS:   a && b || !c
来源：http://dib.gotoacloud.top

TS:   a && b || !c
来源：http://vny.nanxinkj.top

Java: a && b || !c
来源：http://fxn.hongshengwenyu.top

Go:   a && b || !c
来源：http://xeb.yuxming.cn

Ruby: a && b || !c
来源：http://obg.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://csl.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://nzt.guannengcc.top

Py:   if not data: return
来源：http://kpa.sweek.top

PHP:  if (!$data) { return; }
来源：http://iah.haohaochexian.top

JS:   if (!data) return;
来源：http://mhy.uphjek.com

TS:   if (!data) return;
来源：http://gvs.hnxiangtu.top

Java: if (data == null) return;
来源：http://srt.fktsv.cn

Go:   if data == nil { return }
来源：http://ugm.ehwqpu.com

Ruby: return if data.nil?
来源：http://dbe.wangdashe.top

C#:   if (data == null) return;
来源：http://bve.ctjpmb.com

================================================================================
来源：http://bjl.daxiang520.top

C. 函数与作用域
来源：http://otp.gaohongyu789.top

================================================================================
来源：http://enc.pengpengdd.cyou

[C01] 定义函数
来源：http://ckh.tanke756.top

Py:   def add(a, b): return a + b
来源：http://yll.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://goo.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://wkc.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bsh.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nui.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nwi.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://gox.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yco.sjlbkw.cn

[C02] 默认参数
来源：http://ebn.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://qtr.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://qqw.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://owg.zhengqikj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fxd.gotoacloud.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kzy.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ukm.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://inz.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://uqv.yj20258.top

[C03] 可变参数
来源：http://jct.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://hnt.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xpl.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vsg.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jda.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pmp.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gch.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fiq.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dfj.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://ncs.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bnp.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jjy.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nbf.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gkz.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://lcd.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://ajh.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://bxx.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://fqi.zhijiandao.cn

[C05] 返回多个值
来源：http://iig.redwolf501.top

Py:   return a, b
来源：http://zej.xylfe.cn

PHP:  return [$a, $b];
来源：http://cyb.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wmf.52xcode.cn

TS:   return { a, b };
来源：http://avz.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://udy.9152youxi.cn

Go:   return a, b
来源：http://ing.zdbjq.cn

Ruby: return a, b
来源：http://vrn.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://qng.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://swm.tian-w.cn

Py:   square = lambda x: x * x
来源：http://maj.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ayn.fzhhl.top

JS:   const square = x => x * x;
来源：http://uil.zhiwuduotai.top


<!-- 参考信息 -->