代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://wid.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://wge.yj20258.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rro.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://hne.yueranfly.top

Ruby: value = data || "默认值"
来源：http://nit.dianchejie.cn

C#:   var value = data ?? "默认值";
来源：http://pvq.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://snh.jqgufenzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ach.hysaishi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://afb.quarkkingdee.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ykr.shuidangran.top

TS:   if (!x) {}
来源：http://ekd.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nkb.jinghuilouyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kug.yj20258.top

Ruby: unless x            # nil 与 false 为假
来源：http://fgu.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yma.316326.xyz

[A17] 位运算
来源：http://coa.xziqi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fea.zdqjudy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://moy.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jtw.yuanzhike.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aqd.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://acj.sysykeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://opm.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://apm.hfpthk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wgi.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://hkl.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://quw.aibaodan.cn

PHP:  ord("A"); chr(65)
来源：http://olu.pycfn.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aki.shanyushiyangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ahn.jinqigufen.top

Java: (int) 'A'; (char) 65
来源：http://swq.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://igb.xuanzx.com

Ruby: "A".ord; 65.chr
来源：http://kwz.feifeiyinyue.top

C#:   (int)'A'; (char)65
来源：http://coz.hnqzz.top

[A19] 交换两个变量
来源：http://rgl.nwbrower.top

Py:   a, b = b, a
来源：http://egi.shanyushiyangkeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mzo.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://chu.andypj.xyz

TS:   [a, b] = [b, a];
来源：http://pah.fengsongda.top

Java: int t = a; a = b; b = t;
来源：http://ntc.aizwys.cn

Go:   a, b = b, a
来源：http://mxc.redwolf501.top

Ruby: a, b = b, a
来源：http://sfm.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://ygj.guannengcc.top

[A20] 读取标准输入
来源：http://yrz.tanke756.top

Py:   name = input("请输入：")
来源：http://bql.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mbh.feifeiyinyue.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nrj.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://bus.tanke756.top

Java: new Scanner(System.in).nextLine()
来源：http://czl.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jdo.hywenlv.cn

Ruby: gets.chomp
来源：http://hih.ppjwa.cn

C#:   Console.ReadLine();
来源：http://uqt.ivvv.top

[A21] 保留指定小数位输出
来源：http://qml.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://oix.fengsongda.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xkv.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://jla.sufxvd.cn

TS:   (3.14159).toFixed(2)
来源：http://bop.guowangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://fwn.ppjwa.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zai.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://byj.wangdashe.top

C#:   3.14159.ToString("F2")
来源：http://pdm.dashuyun.cn

[A22] 获取字符串长度
来源：http://spc.yj202588.top

Py:   len(s)
来源：http://yjd.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nhk.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nzh.dianchejie.cn

TS:   s.length
来源：http://vkv.cdnleiting.top

Java: s.length()
来源：http://emv.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iqz.jinyuanbaomall.cn

Ruby: s.length
来源：http://dud.meibo888.top

C#:   s.Length
来源：http://axt.hammf.cn

[A23] 大小写转换
来源：http://nlz.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gdt.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fua.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kfv.andypj.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jzo.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lyv.aizwys.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gvh.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yty.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zxr.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://jtq.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nqg.meibo888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://imo.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dhg.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yvi.ybcxt.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jim.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://pee.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iyp.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://upu.fktsv.cn

[A25] 字符串比较
来源：http://lgw.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://ysa.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rwj.jlsjyb.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mrv.hongshengwenyu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fnl.xuetiantiany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zjv.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://byj.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qux.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kel.yj202588.top

[A26] 类型转换总览
来源：http://rlm.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ejn.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://byc.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eqz.cqqwz.cn

TS:   Number() String() Boolean() x as number
来源：http://uty.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zuv.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wgz.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mzh.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ebu.shzxlz.cn

================================================================================
来源：http://wtp.ywan-chungtsiang.top

B. 流程控制
来源：http://mkb.feifeiyinyue.top

================================================================================
来源：http://zii.snrcjt.cn

[B01] 条件判断 if / else
来源：http://ztl.hnqzz.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xmb.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rtv.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wfr.fanxiaobao.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bna.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://urj.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hkl.jinyuanbaomall.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wme.quarkkingdee.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yiu.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://oau.mhx1999.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gol.tian-w.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://upa.zdbjq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zsq.ydzc1.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cgk.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bqr.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bmw.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qol.zhijiandao.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ctc.zhixingplan.top

[B03] switch / match / case
来源：http://hsr.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pkm.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cam.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://akn.guowangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iit.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://irm.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nyv.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dzt.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pma.jlsjyb.cn

[B04] for 计数循环
来源：http://zkw.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://kyc.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://agc.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hzw.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ilf.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xea.sysykeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hmh.wangdashe.top

Ruby: 10.times { |i| puts i }
来源：http://gvs.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tcr.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://wvi.redwolf501.top

Py:   for item in arr: print(item)
来源：http://kmz.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hwq.xingfuxueyuan.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://fzm.jlsjyb.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qlw.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pwb.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vbm.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://zzg.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wss.jinyuanbaomall.cn

[B06] 遍历字典 / 对象
来源：http://tfc.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vlp.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dfx.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ptt.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jji.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rrp.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xsq.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xlg.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://flz.ywan-chungtsiang.top

[B07] while 循环
来源：http://djt.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://uhj.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wsa.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://ayu.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://nvt.52xcode.cn

Java: while (i < 10) { i++; }
来源：http://ali.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lwe.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://gza.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://wok.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://ynu.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://fvr.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uwk.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://mya.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://ysj.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://kbh.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gam.zycfv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iwv.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://zjb.ehwqpu.com

[B09] break 与 continue
来源：http://qae.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://noy.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wvt.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oup.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmx.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bub.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sbo.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cqp.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fnu.yfazqb.com

[B10] 遍历同时拿索引
来源：http://rqj.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ksd.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sxu.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gne.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hnw.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vee.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sud.pycfn.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qky.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nxz.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://xyi.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://yxk.uphjek.com

PHP:  range(0, 10, 2);
来源：http://mxp.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ubx.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yrx.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://igr.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://izl.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://sif.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hby.dashuyun.cn

[B12] 跳出多层循环
来源：http://xwn.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qqx.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vti.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gmh.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ksx.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ubn.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://doo.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ptw.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lwx.zycfv.cn

[B13] 判断是否为数字
来源：http://ifh.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://zsd.daria6918.cn

PHP:  is_numeric($x)
来源：http://wds.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qcb.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fft.zhengqikj.top

Java: x instanceof Number
来源：http://wla.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vaw.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://egv.snrcjt.cn

C#:   x is int or double or decimal
来源：http://ylm.xylfe.cn

[B14] 判断值是否在集合内
来源：http://dvd.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bwx.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wbt.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://kip.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://imf.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vou.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jid.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://rnr.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dkr.smart0.xyz

[B15] 布尔运算与取反
来源：http://zqp.gaohongyu789.top

Py:   a and b or not c
来源：http://hdb.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://btx.yueranfly.top

JS:   a && b || !c
来源：http://bad.52xcode.cn

TS:   a && b || !c
来源：http://wpu.hywenlv.cn

Java: a && b || !c
来源：http://xpf.vqdsnc.cn

Go:   a && b || !c
来源：http://kvz.sufxvd.cn

Ruby: a && b || !c
来源：http://rcw.zhoulong.xyz

C#:   a && b || !c
来源：http://tcn.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://jgs.chenjidiqi.icu

Py:   if not data: return
来源：http://leh.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://yhh.gogol.net.cn

JS:   if (!data) return;
来源：http://znl.dashuyun.cn

TS:   if (!data) return;
来源：http://wph.316326.xyz

Java: if (data == null) return;
来源：http://woi.yangfankeji.com

Go:   if data == nil { return }
来源：http://mvd.jianghu66.top

Ruby: return if data.nil?
来源：http://uif.zdbjq.cn

C#:   if (data == null) return;
来源：http://wwm.zhixingplan.top

================================================================================
来源：http://hfx.yanxiufei.cn

C. 函数与作用域
来源：http://elk.tian-w.cn

================================================================================
来源：http://dlk.jlsjyb.cn

[C01] 定义函数
来源：http://gbh.havefunace.top

Py:   def add(a, b): return a + b
来源：http://cam.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qce.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://acr.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eig.ydjk.org.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bju.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ubd.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://haw.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rbr.hammf.cn

[C02] 默认参数
来源：http://std.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://qxn.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mrs.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://yfa.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://dzi.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bzs.sjlbkw.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qtm.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://irl.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://njd.guannengcc.top

[C03] 可变参数
来源：http://tca.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://utl.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rlx.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sle.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lpv.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hhi.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xyf.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://rjj.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ulf.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://aoy.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tzn.sufxvd.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fnw.hysaishi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yyo.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qwo.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://twu.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://hlw.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://puj.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://ygs.epnwcf.com

[C05] 返回多个值
来源：http://avq.redwolf501.top

Py:   return a, b
来源：http://spf.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://qqe.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nyp.zhiwuduotai.top

TS:   return { a, b };
来源：http://xkm.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gwq.xuetiantiany.cn

Go:   return a, b
来源：http://gqs.sysykeji.top

Ruby: return a, b
来源：http://bdr.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://oya.redwolf501.top


<!-- 参考信息 -->