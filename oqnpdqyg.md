代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://wvx.nwbrower.top

TS:   const value = data ?? "默认值";
来源：http://zsr.chenlongwang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://foj.sjlbkw.cn

Go:   if data == "" { data = "默认值" }
来源：http://niq.iojbl.cn

Ruby: value = data || "默认值"
来源：http://qxt.chenlongwang.top

C#:   var value = data ?? "默认值";
来源：http://ilc.shangyingyoupin.top

[A16] 真假值判断规则
来源：http://jff.wangdashe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xhf.uphjek.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://glz.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kmb.sufxvd.cn

TS:   if (!x) {}
来源：http://dsn.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ror.kuanghao11.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eyr.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wap.xziqi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ulj.hnxiangtu.top

[A17] 位运算
来源：http://gmg.hongshengwenyu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zom.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mrx.cheryme.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ddo.daxiang520.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nxh.52xcode.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mmh.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vma.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrm.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lgt.jyoumei.cn

[A18] 字符与 ASCII 码互转
来源：http://bwe.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://fni.nwbrower.top

PHP:  ord("A"); chr(65)
来源：http://tzc.tian-w.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bzz.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lhf.ctjpmb.com

Java: (int) 'A'; (char) 65
来源：http://zyk.zhijiandao.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://odr.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://jgp.ivvv.top

C#:   (int)'A'; (char)65
来源：http://sli.haohaochexian.top

[A19] 交换两个变量
来源：http://dks.zhengqikj.top

Py:   a, b = b, a
来源：http://rjb.mhx1999.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xoo.shuidangran.top

JS:   [a, b] = [b, a];
来源：http://kyh.ywan-chungtsiang.top

TS:   [a, b] = [b, a];
来源：http://vay.hesvh.cn

Java: int t = a; a = b; b = t;
来源：http://fyp.pengpengdd.cyou

Go:   a, b = b, a
来源：http://kqb.vehdjk.com

Ruby: a, b = b, a
来源：http://gmj.ybcxt.top

C#:   (a, b) = (b, a);
来源：http://xbv.c1oappe.top

[A20] 读取标准输入
来源：http://rkj.ydzc1.top

Py:   name = input("请输入：")
来源：http://pus.jqgufenzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bvr.yanxiufei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jbo.fktsv.cn

TS:   // Node.js：readline 模块
来源：http://vnq.bjfxy.top

Java: new Scanner(System.in).nextLine()
来源：http://skk.daxiang520.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zxw.fktsv.cn

Ruby: gets.chomp
来源：http://jto.cashguo.top

C#:   Console.ReadLine();
来源：http://gcu.hnqzz.top

[A21] 保留指定小数位输出
来源：http://vrg.gogol.net.cn

Py:   f"{3.14159:.2f}"
来源：http://umx.jinghuilouyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ckd.vehdjk.com

JS:   (3.14159).toFixed(2)
来源：http://yol.hywenlv.cn

TS:   (3.14159).toFixed(2)
来源：http://zjb.smart0.xyz

Java: String.format("%.2f", 3.14159)
来源：http://orz.zhaomingkeji.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://okn.redwolf501.top

Ruby: format("%.2f", 3.14159)
来源：http://uch.andypj.xyz

C#:   3.14159.ToString("F2")
来源：http://mgs.zhongyouzk.top

[A22] 获取字符串长度
来源：http://rze.jiagoushi.top

Py:   len(s)
来源：http://xaw.tarul.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uuz.hammf.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yud.yfazqb.com

TS:   s.length
来源：http://jyj.yonumen.top

Java: s.length()
来源：http://esf.hnqzz.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iyb.zhiwuduotai.top

Ruby: s.length
来源：http://lxx.sxryk.cn

C#:   s.Length
来源：http://zed.fktsv.cn

[A23] 大小写转换
来源：http://wqw.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://amk.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fip.shanyushiyangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sro.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nwa.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ene.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mqc.xuetiantiany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uyv.yangfankeji.com

C#:   s.ToUpper(); s.ToLower()
来源：http://rxj.ybcxt.top

[A24] 去除首尾空白
来源：http://kmz.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vrj.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vdt.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jgv.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uxy.tian-w.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://umt.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://kbi.yonumen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mjl.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://woi.aizwys.cn

[A25] 字符串比较
来源：http://usn.shzxlz.cn

Py:   s1 == s2; s1 != s2
来源：http://gme.vehdjk.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tzv.hammf.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vvp.tianlin.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xld.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://waf.tarul.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://maj.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ast.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wlx.hcnkem.com

[A26] 类型转换总览
来源：http://itt.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yeg.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vmh.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xsy.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://gpv.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kzv.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aec.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nxk.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rmi.nwbrower.top

================================================================================
来源：http://guv.jinqigufen.top

B. 流程控制
来源：http://lrn.guannengcc.top

================================================================================
来源：http://ahu.zycfv.cn

[B01] 条件判断 if / else
来源：http://aym.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ien.c1oappe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ycq.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rbg.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mqs.xuetiantiany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ola.dashuyun.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jaf.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ymt.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zml.wangdashe.top

[B02] 多分支 else if / elif
来源：http://nvd.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rre.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yec.ppjwa.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xtd.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bok.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gjk.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://por.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wuv.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ibw.fanxiaobao.xyz

[B03] switch / match / case
来源：http://llo.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yab.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kxy.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jco.zhengqikj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://val.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://myp.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mni.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pwj.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://awr.zdbjq.cn

[B04] for 计数循环
来源：http://ovv.cheryme.top

Py:   for i in range(10): print(i)
来源：http://ied.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mlb.ctjpmb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://beg.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://goz.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tiv.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yru.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://coo.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jiz.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://ims.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://crg.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dng.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ulc.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gzg.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://urh.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pao.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://epz.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aaq.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://wwq.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dyq.andypj.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://soq.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dig.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xqs.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hjb.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://czs.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tfw.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yht.bbcook.cn

[B07] while 循环
来源：http://oij.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://iip.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://xyw.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://hij.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://pvw.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://gxv.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xiw.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://mab.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://dwp.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://cdk.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://czu.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ixo.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://sij.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://jmh.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://ssu.ppjwa.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zru.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://bgt.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://sol.zhoulong.xyz

[B09] break 与 continue
来源：http://csu.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ryi.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ehl.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qwj.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozm.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tap.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jhv.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lzi.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yyw.ydzc1.top

[B10] 遍历同时拿索引
来源：http://qxf.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qqw.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://igf.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ynx.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lfc.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lqp.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wum.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vyu.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://grz.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://xut.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://oun.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://yof.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yhq.chenlongwang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jdw.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sij.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lxh.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://rex.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wyp.chenlongwang.top

[B12] 跳出多层循环
来源：http://gbc.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nuc.jyoumei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ycj.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blc.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aej.vqdsnc.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jvj.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://psd.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yke.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kcn.mhx1999.top

[B13] 判断是否为数字
来源：http://fvn.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://qzw.svipenyu.cn

PHP:  is_numeric($x)
来源：http://utd.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mti.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hzt.meibo888.top

Java: x instanceof Number
来源：http://pyb.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gmu.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://qsf.nanxinkj.top

C#:   x is int or double or decimal
来源：http://sae.bjfxy.top

[B14] 判断值是否在集合内
来源：http://azc.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nbd.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mkh.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://egp.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://zvd.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://rpb.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ueu.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://aug.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nng.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://bfs.chenzaomai.com

Py:   a and b or not c
来源：http://hwv.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://xlo.gzhubu.top

JS:   a && b || !c
来源：http://rms.sysykeji.top

TS:   a && b || !c
来源：http://txl.jinqigfzy.top

Java: a && b || !c
来源：http://jvz.ybcxt.top

Go:   a && b || !c
来源：http://udc.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://xxg.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://axg.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://jti.hywenlv.cn

Py:   if not data: return
来源：http://uij.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://bqc.chenzaomai.com

JS:   if (!data) return;
来源：http://fuo.pycfn.com

TS:   if (!data) return;
来源：http://evu.sufxvd.cn

Java: if (data == null) return;
来源：http://khl.fzhhl.top

Go:   if data == nil { return }
来源：http://iha.kuanghao11.cn

Ruby: return if data.nil?
来源：http://hef.gogol.net.cn

C#:   if (data == null) return;
来源：http://cct.epnwcf.com

================================================================================
来源：http://kan.fzhhl.top

C. 函数与作用域
来源：http://yvy.svipenyu.cn

================================================================================
来源：http://opn.nanxinkj.top

[C01] 定义函数
来源：http://mcs.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://uqw.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pko.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://gas.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://arm.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lxj.fehbvm.com

Go:   func add(a, b int) int { return a + b }
来源：http://fux.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://crg.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vaa.andypj.xyz

[C02] 默认参数
来源：http://lcz.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://hmt.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://msm.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://dlx.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vay.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://aet.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jhu.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://bwl.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://ckd.yj20258.top

[C03] 可变参数
来源：http://unm.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://oqh.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rzt.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qus.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://htf.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://znt.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gmp.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rnn.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zih.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://voj.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jgh.tianlin.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vge.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hhj.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wpl.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://lts.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://oxj.feifeiyinyue.top

Ruby: f(a: 1, b: 2)
来源：http://svn.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://uaa.ydjk.org.cn

[C05] 返回多个值
来源：http://hqx.zhengqikj.top

Py:   return a, b
来源：http://obv.gogol.net.cn

PHP:  return [$a, $b];
来源：http://kml.aibaodan.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qrt.aibaodan.cn

TS:   return { a, b };
来源：http://xvt.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aee.quarkkingdee.top

Go:   return a, b
来源：http://rvi.shanyushiyangtech.top

Ruby: return a, b
来源：http://xic.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://uyv.yuanzhike.top


<!-- 参考信息 -->