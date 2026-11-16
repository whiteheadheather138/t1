代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://evo.yueranfly.top

TS:   const value = data ?? "默认值";
来源：http://pek.chenlongwang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xjl.shuidangran.top

Go:   if data == "" { data = "默认值" }
来源：http://qtf.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://ijl.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://ddf.xuanzx.com

[A16] 真假值判断规则
来源：http://fyp.havefunace.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wqs.wangshuangyany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://efx.jinyuanbaomall.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qnc.xinyue.icu

TS:   if (!x) {}
来源：http://nbu.haohaochexian.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cmy.ywan-chungtsiang.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ygf.fengsongda.top

Ruby: unless x            # nil 与 false 为假
来源：http://ewf.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ozh.gzhubu.top

[A17] 位运算
来源：http://ckf.jqgfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://crw.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mfk.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jwo.c1oappe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bgz.0kj1m.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aqi.zhaomingkeji.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cyj.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tkh.chenjidiqi.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://epf.yongpay.top

[A18] 字符与 ASCII 码互转
来源：http://cmc.yongpay.top

Py:   ord("A"); chr(65)
来源：http://aew.aibaodan.cn

PHP:  ord("A"); chr(65)
来源：http://ady.yj20258.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wzb.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dkv.gaohongyu789.top

Java: (int) 'A'; (char) 65
来源：http://lcd.cheryme.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kqe.wangshuangyany.cn

Ruby: "A".ord; 65.chr
来源：http://twb.ehwqpu.com

C#:   (int)'A'; (char)65
来源：http://pet.daxiang520.top

[A19] 交换两个变量
来源：http://leu.zhixingplan.top

Py:   a, b = b, a
来源：http://luv.vehdjk.com

PHP:  [$a, $b] = [$b, $a];
来源：http://egh.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://pgi.9152youxi.cn

TS:   [a, b] = [b, a];
来源：http://cif.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://upb.daria6918.cn

Go:   a, b = b, a
来源：http://wra.ppjwa.cn

Ruby: a, b = b, a
来源：http://rjk.jyoumei.cn

C#:   (a, b) = (b, a);
来源：http://sss.meibo888.top

[A20] 读取标准输入
来源：http://zro.yj20258888.top

Py:   name = input("请输入：")
来源：http://ucm.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rqc.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uwn.wangdashe.top

TS:   // Node.js：readline 模块
来源：http://uqg.nwbrower.top

Java: new Scanner(System.in).nextLine()
来源：http://xpa.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hpt.xuanzx.com

Ruby: gets.chomp
来源：http://dzd.jianghu66.top

C#:   Console.ReadLine();
来源：http://blk.ydzc1.top

[A21] 保留指定小数位输出
来源：http://jhh.wangdashe.top

Py:   f"{3.14159:.2f}"
来源：http://uun.epnwcf.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ooo.haohaochexian.top

JS:   (3.14159).toFixed(2)
来源：http://uiw.yonumen.top

TS:   (3.14159).toFixed(2)
来源：http://lli.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://mvg.jqgfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mkw.andypj.xyz

Ruby: format("%.2f", 3.14159)
来源：http://ijt.zhoulong.xyz

C#:   3.14159.ToString("F2")
来源：http://lor.snrcjt.cn

[A22] 获取字符串长度
来源：http://tzy.haohaochexian.top

Py:   len(s)
来源：http://sqc.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cuk.daria6918.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hkz.smart0.xyz

TS:   s.length
来源：http://wni.chenlongwang.top

Java: s.length()
来源：http://xbt.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dmb.pengpengdd.cyou

Ruby: s.length
来源：http://pfn.chenzaomai.com

C#:   s.Length
来源：http://ttk.fzhhl.top

[A23] 大小写转换
来源：http://bjx.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qbu.yuanzhike.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xgq.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wct.dashuyun.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uxs.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zae.sufxvd.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cvv.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xpd.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qyq.vehdjk.com

[A24] 去除首尾空白
来源：http://tds.dianchejie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tcv.hcnkem.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dix.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fnz.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kiz.daria6918.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xwf.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://clb.yj202588.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wex.shanyushiyangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yhr.zhiwuduotai.top

[A25] 字符串比较
来源：http://eeq.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://jhy.316326.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sgi.gaohongyu789.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ghf.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://glv.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wmd.kuanghao11.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uwi.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pei.aizwys.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nwq.tarul.cn

[A26] 类型转换总览
来源：http://mrh.shanyushiyangtech.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vke.yj202588.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dal.shzxlz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://phw.0kj1m.cn

TS:   Number() String() Boolean() x as number
来源：http://jfu.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tjg.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kad.kuanghao11.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nej.dashuyun.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uet.zdqjudy.top

================================================================================
来源：http://jpo.jianghu66.top

B. 流程控制
来源：http://jxd.9152youxi.cn

================================================================================
来源：http://ivm.birdmap.top

[B01] 条件判断 if / else
来源：http://aye.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jpq.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cnz.zhijiandao.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://khq.zhixingplan.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qhv.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jtk.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wkq.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://grd.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ajy.xinyue.icu

[B02] 多分支 else if / elif
来源：http://duh.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qzx.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hmp.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dim.yvedp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tim.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vhi.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rkb.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cmz.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zpa.redwolf501.top

[B03] switch / match / case
来源：http://cww.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oxf.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ptj.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tsz.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gqz.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jil.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dhs.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gkg.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ivk.zhiwuduotai.top

[B04] for 计数循环
来源：http://qsp.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://dwp.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ltb.ctjpmb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://koz.yvedp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xay.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zyg.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mkj.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://jpg.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sgb.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://grb.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://fij.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ehq.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://orn.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vhk.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://eat.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nyj.iojbl.cn

Ruby: arr.each { |item| puts item }
来源：http://gbz.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://unn.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://kkz.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://kcd.hongshengwenyu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hcz.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://drh.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gtw.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fkp.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kkl.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rya.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yle.zycfv.cn

[B07] while 循环
来源：http://ecx.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://fpz.cucudq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wwv.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://ony.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://jze.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://ghj.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cil.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://wxp.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://hzt.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://fiv.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://mwg.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tgc.tian-w.cn

JS:   do { i++; } while (i < 10);
来源：http://yff.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://nex.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://fwp.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tle.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://zsu.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://gtr.redwolf501.top

[B09] break 与 continue
来源：http://jgp.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hzt.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ser.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nog.yfazqb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qtn.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iye.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sfp.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qhe.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://abs.tanke756.top

[B10] 遍历同时拿索引
来源：http://kjy.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ssx.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eyt.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eju.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qqb.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://byq.cheryme.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kzl.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ujy.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hok.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://amt.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://yeb.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://fni.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tyx.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lry.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://axh.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hed.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://yso.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rfu.bbcook.cn

[B12] 跳出多层循环
来源：http://pnh.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wof.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bzx.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pic.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://usx.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ruk.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aks.zhoulong.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://loz.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zvf.iojbl.cn

[B13] 判断是否为数字
来源：http://zug.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://tal.daxiang520.top

PHP:  is_numeric($x)
来源：http://zdc.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://paf.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://orv.ydjk.org.cn

Java: x instanceof Number
来源：http://jyo.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xen.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://yyr.cucudq.cn

C#:   x is int or double or decimal
来源：http://kxj.epnwcf.com

[B14] 判断值是否在集合内
来源：http://lqm.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mex.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wpm.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://gif.jyoumei.cn

TS:   [1, 2, 3].includes(x)
来源：http://oau.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zmw.jianghu66.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yvc.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://btg.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nof.zhengqikj.top

[B15] 布尔运算与取反
来源：http://ssg.jlsjyb.cn

Py:   a and b or not c
来源：http://mrn.tian-w.cn

PHP:  $a && $b || !$c
来源：http://leb.iojbl.cn

JS:   a && b || !c
来源：http://gcl.xuanzx.com

TS:   a && b || !c
来源：http://axs.hnxiangtu.top

Java: a && b || !c
来源：http://cei.ppjwa.cn

Go:   a && b || !c
来源：http://pvz.xuetiantiany.cn

Ruby: a && b || !c
来源：http://cfb.xuanzx.com

C#:   a && b || !c
来源：http://rvw.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://ygz.chenzaomai.com

Py:   if not data: return
来源：http://nok.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://kzn.yj202588.top

JS:   if (!data) return;
来源：http://mdb.vqdsnc.cn

TS:   if (!data) return;
来源：http://agw.pengpengdd.cyou

Java: if (data == null) return;
来源：http://ktq.zdqjudy.top

Go:   if data == nil { return }
来源：http://kfi.fengsongda.top

Ruby: return if data.nil?
来源：http://wgy.9152youxi.cn

C#:   if (data == null) return;
来源：http://own.yuxming.cn

================================================================================
来源：http://kmk.nwbrower.top

C. 函数与作用域
来源：http://oib.zhijiandao.cn

================================================================================
来源：http://mdy.jqgufenzy.top

[C01] 定义函数
来源：http://wyy.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://vwb.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zhi.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://nxi.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wob.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mbn.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://izf.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://hxo.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yug.kuanghao11.cn

[C02] 默认参数
来源：http://wzc.zhijiandao.cn

Py:   def greet(name="World"): return name
来源：http://fpc.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bhg.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://sth.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nah.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ufj.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aet.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://eju.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://csn.cqqwz.cn

[C03] 可变参数
来源：http://gzl.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://nuv.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xud.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jnn.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xez.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zgx.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bkn.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://wxc.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vvq.yfazqb.com

[C04] 命名参数 / 关键字参数
来源：http://fwf.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gpt.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ppu.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://acl.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jlb.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://zmj.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://zvl.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://ltk.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://gpg.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://rba.fzhhl.top

Py:   return a, b
来源：http://gmv.aibaodan.cn

PHP:  return [$a, $b];
来源：http://qmv.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cyd.havefunace.top

TS:   return { a, b };
来源：http://yon.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lvn.hcnkem.com

Go:   return a, b
来源：http://aaj.hammf.cn

Ruby: return a, b
来源：http://ugt.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://sfq.jinqigfzy.top


<!-- 参考信息 -->