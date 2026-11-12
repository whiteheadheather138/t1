代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://gqx.jlsjyb.cn

[A15] 空值判断与默认值
来源：http://ifb.gzhubu.top

Py:   value = data or "默认值"
来源：http://qym.ctjpmb.com

PHP:  $value = $data ?? "默认值";
来源：http://dav.daria6918.cn

JS:   const value = data ?? "默认值";
来源：http://bxz.ybcxt.top

TS:   const value = data ?? "默认值";
来源：http://kqy.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wfa.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://unz.xingfuxueyuan.xyz

Ruby: value = data || "默认值"
来源：http://fvh.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://fjb.gzhubu.top

[A16] 真假值判断规则
来源：http://hho.ybcxt.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hek.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nig.sxryk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bni.jinghuilouyu.cn

TS:   if (!x) {}
来源：http://kla.tianlin.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://svb.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yfz.snrcjt.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lln.sysykeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kse.hfpthk.cn

[A17] 位运算
来源：http://rqb.yueranfly.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bvb.yueranfly.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://unz.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jdc.mhx1999.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lnk.yanxiufei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eyh.chenlongwang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tai.shuidangran.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qml.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oph.ydzc1.top

[A18] 字符与 ASCII 码互转
来源：http://wln.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://aao.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://kiu.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixi.fanxiaobao.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://thm.shzxlz.cn

Java: (int) 'A'; (char) 65
来源：http://nca.yanxiufei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nft.kuanghao11.cn

Ruby: "A".ord; 65.chr
来源：http://ief.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://emq.zhixingplan.top

[A19] 交换两个变量
来源：http://ihb.ppjwa.cn

Py:   a, b = b, a
来源：http://kcs.jlsjyb.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mpx.ydjk.org.cn

JS:   [a, b] = [b, a];
来源：http://rlw.316326.xyz

TS:   [a, b] = [b, a];
来源：http://gtk.quarkkingdee.top

Java: int t = a; a = b; b = t;
来源：http://fam.316326.xyz

Go:   a, b = b, a
来源：http://prw.zycfv.cn

Ruby: a, b = b, a
来源：http://gci.jinqigufen.top

C#:   (a, b) = (b, a);
来源：http://jee.aizwys.cn

[A20] 读取标准输入
来源：http://jpi.0kj1m.cn

Py:   name = input("请输入：")
来源：http://usq.tianlin.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://uqi.zdqjudy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zgu.chenzaomai.com

TS:   // Node.js：readline 模块
来源：http://qqj.smart0.xyz

Java: new Scanner(System.in).nextLine()
来源：http://qhn.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dkz.haohaochexian.top

Ruby: gets.chomp
来源：http://onk.dashuyun.cn

C#:   Console.ReadLine();
来源：http://gnr.nwbrower.top

[A21] 保留指定小数位输出
来源：http://qnj.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://hfa.daxiang520.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cdd.aizwys.cn

JS:   (3.14159).toFixed(2)
来源：http://rox.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://gnj.hysaishi.cn

Java: String.format("%.2f", 3.14159)
来源：http://alg.zdbjq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qvk.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://ptz.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://muo.ybcxt.top

[A22] 获取字符串长度
来源：http://wea.svipenyu.cn

Py:   len(s)
来源：http://aso.jlsjyb.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cha.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://awt.52xcode.cn

TS:   s.length
来源：http://get.xinyue.icu

Java: s.length()
来源：http://iio.316326.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pel.hammf.cn

Ruby: s.length
来源：http://tct.hysaishi.cn

C#:   s.Length
来源：http://zou.shzxlz.cn

[A23] 大小写转换
来源：http://jqa.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bqj.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qjr.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mlz.shuidangran.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://csw.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xjl.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gwq.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kmz.zhaomingkeji.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://qyo.jqgfzy.top

[A24] 去除首尾空白
来源：http://rtp.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://awk.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hwl.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://woz.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lza.aibaodan.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lyl.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://jbd.vehdjk.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://got.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bqh.zdbjq.cn

[A25] 字符串比较
来源：http://fsr.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://vjm.chenjidiqi.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://prd.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yoy.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uep.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rjb.jiagoushi.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wvq.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pqr.tian-w.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zuq.ydzc1.top

[A26] 类型转换总览
来源：http://ujk.hammf.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://koe.52xcode.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bnn.feifeiyinyue.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vuz.hongshengwenyu.top

TS:   Number() String() Boolean() x as number
来源：http://blf.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eky.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fgq.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://dha.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ppy.mhx1999.top

================================================================================
来源：http://obs.haohaochexian.top

B. 流程控制
来源：http://fuw.yfazqb.com

================================================================================
来源：http://hpo.yfazqb.com

[B01] 条件判断 if / else
来源：http://eve.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bqj.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lhk.jqgufenzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uiq.zhixingplan.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dif.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cmi.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qnh.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://stm.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oqz.xuanzx.com

[B02] 多分支 else if / elif
来源：http://qwt.tian-w.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wbz.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lue.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mte.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fzr.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://civ.tian-w.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qsz.yj20258888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wbk.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzv.nanxuanxn.top

[B03] switch / match / case
来源：http://qna.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jdh.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rrd.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mef.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sje.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tkv.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dga.zhixingplan.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qmi.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cbn.sysykeji.top

[B04] for 计数循环
来源：http://zmf.yj20258.top

Py:   for i in range(10): print(i)
来源：http://qif.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jer.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yxi.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yfw.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gut.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kdz.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://tvp.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bxq.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://war.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://pty.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gey.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fjj.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://gao.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://anf.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dep.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://nag.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ktt.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://pox.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mcs.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cai.sweek.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wko.meibo888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xmq.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xjm.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ydh.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qmn.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zmb.vehdjk.com

[B07] while 循环
来源：http://qwz.fktsv.cn

Py:   while i < 10: i += 1
来源：http://cmm.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://nwt.hnxiangtu.top

JS:   while (i < 10) { i++; }
来源：http://ibo.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://jig.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://pxo.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pas.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://llr.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://xll.sweek.top

[B08] do-while（至少执行一次）
来源：http://ski.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://hpi.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ppu.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://djj.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://qfy.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://hki.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://txb.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://awy.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://mov.jlsjyb.cn

[B09] break 与 continue
来源：http://tsg.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ohy.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://exz.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyy.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zeh.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tgl.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bvx.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kra.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzv.daxiang520.top

[B10] 遍历同时拿索引
来源：http://oki.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uwi.hongshengwenyu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qui.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dub.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ggq.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://svc.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pxa.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ryk.hnxiangtu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xfl.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://oli.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://gzt.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://jwo.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lek.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://shx.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fhb.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mxq.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://xyn.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bgi.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://ibx.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://oeq.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ysp.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yrs.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tlx.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ndp.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ywd.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rmu.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xps.dashuyun.cn

[B13] 判断是否为数字
来源：http://dlp.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://ync.jiagoushi.top

PHP:  is_numeric($x)
来源：http://xap.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lpa.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mal.jinqigfzy.top

Java: x instanceof Number
来源：http://foy.jinqigufen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bal.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://hbb.yuanzhike.top

C#:   x is int or double or decimal
来源：http://wsj.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://wvm.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vno.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://chr.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://hsb.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://ckh.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://kll.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fxw.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://iir.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bgg.yfazqb.com

[B15] 布尔运算与取反
来源：http://ivv.hesvh.cn

Py:   a and b or not c
来源：http://art.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://sqr.c1oappe.top

JS:   a && b || !c
来源：http://dtz.hysaishi.cn

TS:   a && b || !c
来源：http://xnx.c1oappe.top

Java: a && b || !c
来源：http://mam.ivvv.top

Go:   a && b || !c
来源：http://vzl.cheryme.top

Ruby: a && b || !c
来源：http://ocv.dashuyun.cn

C#:   a && b || !c
来源：http://gcq.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://pja.nanxuanxn.top

Py:   if not data: return
来源：http://xts.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://hgi.kuanghao11.cn

JS:   if (!data) return;
来源：http://zyd.cdnleiting.top

TS:   if (!data) return;
来源：http://buw.hesvh.cn

Java: if (data == null) return;
来源：http://gos.316326.xyz

Go:   if data == nil { return }
来源：http://wsk.jyoumei.cn

Ruby: return if data.nil?
来源：http://dwx.nanxuanxn.top

C#:   if (data == null) return;
来源：http://xmk.vqdsnc.cn

================================================================================
来源：http://wtf.quarkkingdee.top

C. 函数与作用域
来源：http://ake.zdbjq.cn

================================================================================
来源：http://qxo.yangfankeji.com

[C01] 定义函数
来源：http://psv.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://ppu.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ekk.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://flh.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://laq.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dtx.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://shd.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://dml.uphjek.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://soz.ywan-chungtsiang.top

[C02] 默认参数
来源：http://jrj.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://hjf.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oyl.fktsv.cn

JS:   function greet(name = "World") { return name; }
来源：http://wau.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jhn.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pzv.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ozc.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://vpy.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://yqk.xuanzx.com

[C03] 可变参数
来源：http://hob.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://ubi.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qrm.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qpj.ctjpmb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://upx.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tdq.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rvx.meibo888.top

Ruby: def total(*nums); nums.sum; end
来源：http://yxu.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://amr.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://kiq.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bra.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mbl.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kqs.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kpd.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://oze.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://ahq.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://lik.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://tuy.gaohongyu789.top

[C05] 返回多个值
来源：http://usq.vehdjk.com

Py:   return a, b
来源：http://lok.sweek.top

PHP:  return [$a, $b];
来源：http://hfl.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://vhl.hammf.cn

TS:   return { a, b };
来源：http://eqi.hnxiangtu.top


<!-- 参考信息 -->