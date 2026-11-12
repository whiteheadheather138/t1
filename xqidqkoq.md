代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://ibf.zdbjq.cn

TS:   const value = data ?? "默认值";
来源：http://gzt.gaohongyu789.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dwx.gaohongyu789.top

Go:   if data == "" { data = "默认值" }
来源：http://zdx.wangdashe.top

Ruby: value = data || "默认值"
来源：http://gsm.yueranfly.top

C#:   var value = data ?? "默认值";
来源：http://tin.shangyingyoupin.top

[A16] 真假值判断规则
来源：http://yfs.zdqjudy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wxh.zhijiandao.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dwx.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uzz.cqqwz.cn

TS:   if (!x) {}
来源：http://fes.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ynl.guowangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ksy.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mpu.shzxlz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tur.jyoumei.cn

[A17] 位运算
来源：http://fyj.pengpengdd.cyou

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://avb.sufxvd.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mkx.epnwcf.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oug.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dfe.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cve.yfazqb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ddz.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ycx.fengsongda.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hle.andypj.xyz

[A18] 字符与 ASCII 码互转
来源：http://gfh.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://cjo.jqgufenzy.top

PHP:  ord("A"); chr(65)
来源：http://ayt.hnxiangtu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://stj.wangshuangyany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zmk.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://gut.sufxvd.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uke.jinqigufen.top

Ruby: "A".ord; 65.chr
来源：http://dun.sweek.top

C#:   (int)'A'; (char)65
来源：http://jqa.yuanzhike.top

[A19] 交换两个变量
来源：http://spz.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://xig.wangshuangyany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vmk.nwbrower.top

JS:   [a, b] = [b, a];
来源：http://ydm.ywan-chungtsiang.top

TS:   [a, b] = [b, a];
来源：http://jna.daria6918.cn

Java: int t = a; a = b; b = t;
来源：http://dfa.yueranfly.top

Go:   a, b = b, a
来源：http://qbb.cucudq.cn

Ruby: a, b = b, a
来源：http://xnp.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://sqj.hesvh.cn

[A20] 读取标准输入
来源：http://oln.zhoulong.xyz

Py:   name = input("请输入：")
来源：http://ylb.zhaomingkeji.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://slc.mhx1999.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cvq.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://svm.bjfxy.top

Java: new Scanner(System.in).nextLine()
来源：http://znt.gaohongyu789.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yca.guannengcc.top

Ruby: gets.chomp
来源：http://xqb.sufxvd.cn

C#:   Console.ReadLine();
来源：http://jbi.tarul.cn

[A21] 保留指定小数位输出
来源：http://obz.zhaomingkeji.xyz

Py:   f"{3.14159:.2f}"
来源：http://lnt.sjlbkw.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xjt.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://fhu.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://iqe.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://xcz.zdbjq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oat.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://tws.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://qpg.vqdsnc.cn

[A22] 获取字符串长度
来源：http://ouh.yuanzhike.top

Py:   len(s)
来源：http://ncp.zhiwuduotai.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oxv.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vhe.ydzc1.top

TS:   s.length
来源：http://sxg.xylfe.cn

Java: s.length()
来源：http://rby.yangfankeji.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mae.andypj.xyz

Ruby: s.length
来源：http://vns.0kj1m.cn

C#:   s.Length
来源：http://gvc.yuanzhike.top

[A23] 大小写转换
来源：http://hti.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hmv.jinqigufen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wag.xziqi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hos.gaohongyu789.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hbk.yanxiufei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://arl.jianghu66.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qxs.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ctc.hammf.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kwj.sxryk.cn

[A24] 去除首尾空白
来源：http://pan.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qej.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://axl.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wcf.jiagoushi.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fyx.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qjv.nanxuanxn.top

Go:   strings.TrimSpace(s)
来源：http://ulh.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eoe.ydzc1.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eyc.jqgufenzy.top

[A25] 字符串比较
来源：http://rhb.shanyushiyangtech.top

Py:   s1 == s2; s1 != s2
来源：http://wus.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nab.andypj.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eqs.jianghu66.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tux.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rxa.9152youxi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rst.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vth.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hsj.haohaochexian.top

[A26] 类型转换总览
来源：http://oyw.snrcjt.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oux.sxryk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uep.gaohongyu789.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lys.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://aez.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gme.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://khb.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pog.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uoo.jinyuanbaomall.cn

================================================================================
来源：http://cxm.sufxvd.cn

B. 流程控制
来源：http://sih.hcnkem.com

================================================================================
来源：http://qsh.ivvv.top

[B01] 条件判断 if / else
来源：http://hgg.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ocd.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zqq.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yzk.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cas.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://agn.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ngn.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bmr.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kky.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://raj.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wth.cdnleiting.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rdb.vehdjk.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slo.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nmn.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jof.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wxs.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jjh.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwt.jiagoushi.top

[B03] switch / match / case
来源：http://lut.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xvd.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gxs.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gmy.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dss.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kze.chenjidiqi.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nvb.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lgr.shanyushiyangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ucc.fktsv.cn

[B04] for 计数循环
来源：http://tky.hammf.cn

Py:   for i in range(10): print(i)
来源：http://ixm.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hbr.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qgf.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://plx.yj20258.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tll.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wof.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://ghe.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dpl.andypj.xyz

[B05] 遍历数组 / 列表
来源：http://hab.yueranfly.top

Py:   for item in arr: print(item)
来源：http://hzb.shanyushiyangtech.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wnj.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://zmu.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kit.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wyi.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nij.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://wsf.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sej.jinghuilouyu.cn

[B06] 遍历字典 / 对象
来源：http://bbi.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://urj.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rfa.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zrb.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://thk.zdqjudy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fko.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uyp.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nec.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hjr.shzxlz.cn

[B07] while 循环
来源：http://urs.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://mbb.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://lhq.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://qnp.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://tbk.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://cva.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ojn.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://zkm.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://zta.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://mpl.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://uzj.hysaishi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mdy.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://xga.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://qrm.shuidangran.top

Java: do { i++; } while (i < 10);
来源：http://bvz.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://fyf.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://jdq.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://ldt.fengsongda.top

[B09] break 与 continue
来源：http://qzq.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vec.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uat.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://otk.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tve.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzh.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ojd.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dop.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jeu.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://wsm.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nyr.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tvv.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wxk.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xcj.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aqm.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yyp.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nsr.tanke756.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://exi.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://rkj.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://edi.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://ein.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://brh.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aex.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uql.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gfw.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://yrk.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lqf.jinqigufen.top

[B12] 跳出多层循环
来源：http://csq.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eyu.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pyy.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cjk.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ksm.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://djm.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ucs.zhengqikj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cpy.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fpr.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://ygo.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://cmw.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://tug.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fre.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zzv.hywenlv.cn

Java: x instanceof Number
来源：http://ari.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qgj.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://vgp.jqgfzy.top

C#:   x is int or double or decimal
来源：http://xig.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://ejh.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bxr.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lxv.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ehk.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://hhu.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ojb.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mds.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cjm.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yqa.ivvv.top

[B15] 布尔运算与取反
来源：http://rbv.guannengcc.top

Py:   a and b or not c
来源：http://dqe.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://iad.yj202588.top

JS:   a && b || !c
来源：http://prg.haohaochexian.top

TS:   a && b || !c
来源：http://uwu.tarul.cn

Java: a && b || !c
来源：http://sms.bbcook.cn

Go:   a && b || !c
来源：http://tmh.daria6918.cn

Ruby: a && b || !c
来源：http://rlg.fktsv.cn

C#:   a && b || !c
来源：http://phh.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://evy.jinqigfzy.top

Py:   if not data: return
来源：http://xch.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://ksc.tarul.cn

JS:   if (!data) return;
来源：http://pgz.yongpay.top

TS:   if (!data) return;
来源：http://hna.shuidangran.top

Java: if (data == null) return;
来源：http://vwa.xziqi.cn

Go:   if data == nil { return }
来源：http://avv.ppjwa.cn

Ruby: return if data.nil?
来源：http://wlt.bjfxy.top

C#:   if (data == null) return;
来源：http://gqb.kuanghao11.cn

================================================================================
来源：http://bku.yfazqb.com

C. 函数与作用域
来源：http://mja.sysykeji.top

================================================================================
来源：http://edb.ehwqpu.com

[C01] 定义函数
来源：http://xlp.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://cio.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yuq.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://qjx.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fdp.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ejx.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ksg.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://qmj.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://igd.fengsongda.top

[C02] 默认参数
来源：http://hvn.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://ebk.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dpy.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://jfj.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ifm.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ccq.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hsf.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://flv.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://nsi.yangfankeji.com

[C03] 可变参数
来源：http://gqi.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://jef.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://knv.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uhw.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rjk.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mfj.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://edr.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dkh.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://his.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://pem.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ydc.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xqr.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nsp.ehwqpu.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vdb.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://znd.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://xcv.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://xbe.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://tfp.feifeiyinyue.top

[C05] 返回多个值
来源：http://pah.guannengcc.top

Py:   return a, b
来源：http://mdj.vqdsnc.cn

PHP:  return [$a, $b];
来源：http://pwc.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://spb.jianghu66.top

TS:   return { a, b };
来源：http://oae.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tkf.ehwqpu.com

Go:   return a, b
来源：http://ubm.yuxming.cn

Ruby: return a, b
来源：http://zge.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://rku.tanke756.top


<!-- 参考信息 -->