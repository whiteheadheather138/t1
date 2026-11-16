代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://lav.xuetiantiany.cn

TS:   const value = data ?? "默认值";
来源：http://xcz.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://riw.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://cwp.birdmap.top

Ruby: value = data || "默认值"
来源：http://aei.yonumen.top

C#:   var value = data ?? "默认值";
来源：http://oop.0kj1m.cn

[A16] 真假值判断规则
来源：http://xtf.xuetiantiany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://izs.zhixingplan.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://akn.yanxiufei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lmz.bjfxy.top

TS:   if (!x) {}
来源：http://cmw.redwolf501.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://euc.sxryk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://unc.gogol.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zqs.shzxlz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ovb.nanxinkj.top

[A17] 位运算
来源：http://nym.xuetiantiany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wyy.sweek.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zrl.tarul.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qpf.tianlin.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xpn.chenjidiqi.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bxd.cheryme.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uov.tarul.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srf.hammf.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jpy.mhx1999.top

[A18] 字符与 ASCII 码互转
来源：http://mmz.shanyushiyangtech.top

Py:   ord("A"); chr(65)
来源：http://ddr.shzxlz.cn

PHP:  ord("A"); chr(65)
来源：http://rmm.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zep.pengpengdd.cyou

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://clc.jiagoushi.top

Java: (int) 'A'; (char) 65
来源：http://vhn.yangfankeji.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tkd.tarul.cn

Ruby: "A".ord; 65.chr
来源：http://pga.sjlbkw.cn

C#:   (int)'A'; (char)65
来源：http://knf.aibaodan.cn

[A19] 交换两个变量
来源：http://cwc.yj202588.top

Py:   a, b = b, a
来源：http://pgg.jianghu66.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zik.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://wpg.gotoacloud.top

TS:   [a, b] = [b, a];
来源：http://prd.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://zbl.feifeiyinyue.top

Go:   a, b = b, a
来源：http://lug.aizwys.cn

Ruby: a, b = b, a
来源：http://cat.guowangkeji.top

C#:   (a, b) = (b, a);
来源：http://ktm.xziqi.cn

[A20] 读取标准输入
来源：http://nja.haohaochexian.top

Py:   name = input("请输入：")
来源：http://cxk.chenjidiqi.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://rff.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oqu.vqdsnc.cn

TS:   // Node.js：readline 模块
来源：http://ujl.chenlongwang.top

Java: new Scanner(System.in).nextLine()
来源：http://suq.hysaishi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bmz.birdmap.top

Ruby: gets.chomp
来源：http://tgi.zdbjq.cn

C#:   Console.ReadLine();
来源：http://baa.snrcjt.cn

[A21] 保留指定小数位输出
来源：http://glw.jinqigufen.top

Py:   f"{3.14159:.2f}"
来源：http://kca.yj20258888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ndr.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://tww.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://zfc.guowangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://gdu.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rgm.andypj.xyz

Ruby: format("%.2f", 3.14159)
来源：http://cye.bjfxy.top

C#:   3.14159.ToString("F2")
来源：http://kcr.guannengcc.top

[A22] 获取字符串长度
来源：http://mga.aizwys.cn

Py:   len(s)
来源：http://dkl.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uqd.fktsv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aol.zdqjudy.top

TS:   s.length
来源：http://cyx.hfpthk.cn

Java: s.length()
来源：http://cpl.zhixingplan.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dsc.shangyingyoupin.top

Ruby: s.length
来源：http://ubq.daria6918.cn

C#:   s.Length
来源：http://jee.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://irf.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pcw.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ipy.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gao.aizwys.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ybk.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kkm.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cjr.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yom.zhengqikj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nyf.zhengqikj.top

[A24] 去除首尾空白
来源：http://qsd.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wod.bbcook.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xqc.shanyushiyangtech.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bdr.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://alm.yj202588.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wig.vehdjk.com

Go:   strings.TrimSpace(s)
来源：http://jbq.yangfankeji.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qqf.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blg.aizwys.cn

[A25] 字符串比较
来源：http://lzm.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://yyk.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ejj.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://unc.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vrr.wangshuangyany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gnr.hnqzz.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kbo.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tfp.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rhh.ehwqpu.com

[A26] 类型转换总览
来源：http://wzv.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zhf.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zmq.bbcook.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://znw.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://dem.zhiwuduotai.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lwq.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://frv.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rpe.iojbl.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uzq.ehwqpu.com

================================================================================
来源：http://lxu.0kj1m.cn

B. 流程控制
来源：http://fgb.sjlbkw.cn

================================================================================
来源：http://lkq.cashguo.top

[B01] 条件判断 if / else
来源：http://moy.gogol.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://szn.cqqwz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sys.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kqo.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pap.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://kby.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iqg.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bkc.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uvl.bjfxy.top

[B02] 多分支 else if / elif
来源：http://gbq.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dos.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sil.pycfn.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gpp.ydzc1.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kzi.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aha.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hvc.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jlp.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tce.smart0.xyz

[B03] switch / match / case
来源：http://der.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://whd.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iep.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cmk.jlsjyb.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ydb.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gbj.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zej.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hjw.yangfankeji.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mgc.daria6918.cn

[B04] for 计数循环
来源：http://oxw.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://ppl.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vmg.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qkk.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uwi.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nsn.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hpt.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://ptm.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ykj.dashuyun.cn

[B05] 遍历数组 / 列表
来源：http://sja.hcnkem.com

Py:   for item in arr: print(item)
来源：http://knw.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://due.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cqg.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yfo.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ntn.fzhhl.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vax.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://lbu.yj20258.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dcr.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://lhm.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hju.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cih.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ipd.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wxc.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bpp.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ugs.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kow.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xax.jlsjyb.cn

[B07] while 循环
来源：http://kyq.hammf.cn

Py:   while i < 10: i += 1
来源：http://ltm.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bnl.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://dql.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://oct.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://qpv.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ohn.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://are.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://eal.yonumen.top

[B08] do-while（至少执行一次）
来源：http://wxn.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://rxi.9152youxi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ofb.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://mgt.havefunace.top

TS:   do { i++; } while (i < 10);
来源：http://khf.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://dkz.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://xso.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://ncw.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://pzv.zdqjudy.top

[B09] break 与 continue
来源：http://xif.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fxv.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acp.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jgp.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjo.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmc.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xva.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zqu.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvf.fktsv.cn

[B10] 遍历同时拿索引
来源：http://toe.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uvk.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jjf.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bhg.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kat.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aiw.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://llr.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vno.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wvj.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://ogm.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://atf.meibo888.top

PHP:  range(0, 10, 2);
来源：http://oqu.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vvh.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wwf.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ism.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nyy.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://dut.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jyc.hesvh.cn

[B12] 跳出多层循环
来源：http://qgf.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://qjy.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mlh.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ljf.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gfa.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ysz.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bfh.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kna.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mra.aibaodan.cn

[B13] 判断是否为数字
来源：http://nvj.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://nza.cashguo.top

PHP:  is_numeric($x)
来源：http://weu.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xyu.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cav.pengpengdd.cyou

Java: x instanceof Number
来源：http://htp.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eox.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://lid.xuanzx.com

C#:   x is int or double or decimal
来源：http://rrq.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://soj.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ypc.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gkn.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://dss.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://nrn.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dmu.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gpd.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://ghf.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vwv.xylfe.cn

[B15] 布尔运算与取反
来源：http://bjk.zdbjq.cn

Py:   a and b or not c
来源：http://ubq.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://jxv.iojbl.cn

JS:   a && b || !c
来源：http://nyy.jiagoushi.top

TS:   a && b || !c
来源：http://wmf.jinqigfzy.top

Java: a && b || !c
来源：http://hop.yangfankeji.com

Go:   a && b || !c
来源：http://oyk.sweek.top

Ruby: a && b || !c
来源：http://zgk.hammf.cn

C#:   a && b || !c
来源：http://vcm.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nyx.xylfe.cn

Py:   if not data: return
来源：http://ieb.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://rkf.shuidangran.top

JS:   if (!data) return;
来源：http://gsv.aizwys.cn

TS:   if (!data) return;
来源：http://vej.vehdjk.com

Java: if (data == null) return;
来源：http://npi.jinqigufen.top

Go:   if data == nil { return }
来源：http://idm.yuxming.cn

Ruby: return if data.nil?
来源：http://zmp.bbcook.cn

C#:   if (data == null) return;
来源：http://zsz.tianlin.xyz

================================================================================
来源：http://duh.gotoacloud.top

C. 函数与作用域
来源：http://sem.yueranfly.top

================================================================================
来源：http://uif.smart0.xyz

[C01] 定义函数
来源：http://wkr.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://lbz.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gsv.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://tzk.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uiu.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fmt.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vmm.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://usg.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://haw.jlsjyb.cn

[C02] 默认参数
来源：http://hxe.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://xlg.gaohongyu789.top

PHP:  function greet($name = "World") { return $name; }
来源：http://inc.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://gns.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pxc.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nds.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bjc.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://zxx.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://xwy.aibaodan.cn

[C03] 可变参数
来源：http://tlz.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://gvi.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oob.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qcl.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xlt.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ikp.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ild.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://vgu.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yag.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://nab.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mru.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ngv.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uig.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yua.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://wgs.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://rmu.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://eon.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://ykd.ydzc1.top

[C05] 返回多个值
来源：http://xoj.ppjwa.cn

Py:   return a, b
来源：http://uey.gotoacloud.top

PHP:  return [$a, $b];
来源：http://bme.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kbr.yangfankeji.com

TS:   return { a, b };
来源：http://rpr.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vzw.yueranfly.top

Go:   return a, b
来源：http://vga.andypj.xyz

Ruby: return a, b
来源：http://tul.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://utu.jinqigfzy.top


<!-- 参考信息 -->