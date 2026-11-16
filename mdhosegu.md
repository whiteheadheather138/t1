代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://rkn.kuanghao11.cn

[A15] 空值判断与默认值
来源：http://oqk.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://wms.sysykeji.top

PHP:  $value = $data ?? "默认值";
来源：http://qjt.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://jeh.wangdashe.top

TS:   const value = data ?? "默认值";
来源：http://exy.wangshuangyany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nbm.guannengcc.top

Go:   if data == "" { data = "默认值" }
来源：http://dwv.cqqwz.cn

Ruby: value = data || "默认值"
来源：http://vek.jianghu66.top

C#:   var value = data ?? "默认值";
来源：http://kdd.yj20258888.top

[A16] 真假值判断规则
来源：http://ses.tanke756.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iiu.yangfankeji.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://whj.hesvh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pgq.meibo888.top

TS:   if (!x) {}
来源：http://slb.uphjek.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://flx.bbcook.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://azy.jinghuilouyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yel.tian-w.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wuh.sufxvd.cn

[A17] 位运算
来源：http://hnf.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vta.andypj.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rfb.ctjpmb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wwv.zhongyouzk.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gpm.zhixingplan.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jdq.sysykeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bgn.zhongyouzk.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kyr.pycfn.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tyf.nanxinkj.top

[A18] 字符与 ASCII 码互转
来源：http://qer.meibo888.top

Py:   ord("A"); chr(65)
来源：http://sqc.nanxinkj.top

PHP:  ord("A"); chr(65)
来源：http://fms.gotoacloud.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jty.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uor.aizwys.cn

Java: (int) 'A'; (char) 65
来源：http://doa.iojbl.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bon.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://ouq.sufxvd.cn

C#:   (int)'A'; (char)65
来源：http://haa.aibaodan.cn

[A19] 交换两个变量
来源：http://ixz.wangshuangyany.cn

Py:   a, b = b, a
来源：http://uxc.c1oappe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tch.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://zqo.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://npv.bjfxy.top

Java: int t = a; a = b; b = t;
来源：http://jrw.chenjidiqi.icu

Go:   a, b = b, a
来源：http://vvi.jiagoushi.top

Ruby: a, b = b, a
来源：http://ubg.sufxvd.cn

C#:   (a, b) = (b, a);
来源：http://waa.sysykeji.top

[A20] 读取标准输入
来源：http://fhz.cqqwz.cn

Py:   name = input("请输入：")
来源：http://psk.xziqi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mmq.hfpthk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gah.hnqzz.top

TS:   // Node.js：readline 模块
来源：http://zpq.mhx1999.top

Java: new Scanner(System.in).nextLine()
来源：http://mky.sjlbkw.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://maz.zhixingplan.top

Ruby: gets.chomp
来源：http://obj.meibo888.top

C#:   Console.ReadLine();
来源：http://ysr.52xcode.cn

[A21] 保留指定小数位输出
来源：http://gum.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://til.sysykeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pha.nanxuanxn.top

JS:   (3.14159).toFixed(2)
来源：http://zwy.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://emy.sxryk.cn

Java: String.format("%.2f", 3.14159)
来源：http://hut.yueranfly.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tvm.havefunace.top

Ruby: format("%.2f", 3.14159)
来源：http://dsx.hfpthk.cn

C#:   3.14159.ToString("F2")
来源：http://yqj.shanyushiyangtech.top

[A22] 获取字符串长度
来源：http://udz.mhx1999.top

Py:   len(s)
来源：http://uzw.jianghu66.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xpa.zhijiandao.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wky.tianlin.xyz

TS:   s.length
来源：http://por.pengpengdd.cyou

Java: s.length()
来源：http://ufn.birdmap.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zoj.yj20258.top

Ruby: s.length
来源：http://jqv.9152youxi.cn

C#:   s.Length
来源：http://xhq.nanxinkj.top

[A23] 大小写转换
来源：http://gkr.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cfc.vehdjk.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jud.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vwy.shanyushiyangtech.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hio.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hte.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fud.havefunace.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sbw.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://hte.cucudq.cn

[A24] 去除首尾空白
来源：http://bwf.ctjpmb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rav.nwbrower.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tyb.jiagoushi.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xum.vqdsnc.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qzx.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kno.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://cse.ctjpmb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oqs.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fzh.pycfn.com

[A25] 字符串比较
来源：http://odj.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://krq.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rxq.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://crc.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://twl.jianghu66.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gqm.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://flc.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fyi.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yen.xinyue.icu

[A26] 类型转换总览
来源：http://omz.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gnp.vqdsnc.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ynq.yuxming.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sgu.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://vyv.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://npd.fehbvm.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mqw.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://zgh.tianlin.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jpr.dianchejie.cn

================================================================================
来源：http://onr.chenjidiqi.icu

B. 流程控制
来源：http://bxc.sysykeji.top

================================================================================
来源：http://fks.ctjpmb.com

[B01] 条件判断 if / else
来源：http://hnk.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bfw.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tot.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hjn.ydjk.org.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bhk.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dyr.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sga.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wou.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tsv.tanke756.top

[B02] 多分支 else if / elif
来源：http://rbk.iojbl.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://igp.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mzg.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ksg.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sud.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lsn.birdmap.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mlb.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jmb.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wru.ybcxt.top

[B03] switch / match / case
来源：http://flv.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ary.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://atk.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://epn.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ugf.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ojs.yj20258888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://amw.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lzh.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iff.ydzc1.top

[B04] for 计数循环
来源：http://ewu.haohaochexian.top

Py:   for i in range(10): print(i)
来源：http://jhd.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kfb.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lzt.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iei.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qax.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fsp.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://ggo.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://daa.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://nqa.chenlongwang.top

Py:   for item in arr: print(item)
来源：http://jhg.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://abu.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aef.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://aum.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gwa.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ijd.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://qbs.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oef.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://mxy.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kbc.cucudq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vfp.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xxn.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kah.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xdh.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eqk.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uaq.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jru.tian-w.cn

[B07] while 循环
来源：http://eze.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://gnx.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://mqb.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://der.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://erh.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://gos.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bbt.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://xsm.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://wve.xziqi.cn

[B08] do-while（至少执行一次）
来源：http://amg.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://jkq.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ddj.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://mnt.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://lmv.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://pgl.cheryme.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ayz.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ftn.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://ssn.gzhubu.top

[B09] break 与 continue
来源：http://yrx.ppjwa.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://meb.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tcf.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kux.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xot.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kff.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://htt.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jzl.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mjy.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://bur.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bfk.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jvi.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pto.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nxo.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://soh.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hnp.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mcd.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://adx.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://vwn.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://cuk.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://ypt.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kuf.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ega.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://obf.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zoj.sxryk.cn

Ruby: (0...10).step(2).to_a
来源：http://ofh.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dha.guowangkeji.top

[B12] 跳出多层循环
来源：http://izz.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tzb.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uki.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vep.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://snc.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sir.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ssp.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ymb.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://opf.cucudq.cn

[B13] 判断是否为数字
来源：http://zjb.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://jum.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://zkm.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fij.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://taz.hongshengwenyu.top

Java: x instanceof Number
来源：http://fum.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://far.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://muk.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://jpd.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://uwq.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jia.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://itp.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://pwg.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://ram.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://iza.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tvj.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://wsq.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cer.yfazqb.com

[B15] 布尔运算与取反
来源：http://ikp.cdnleiting.top

Py:   a and b or not c
来源：http://may.cashguo.top

PHP:  $a && $b || !$c
来源：http://goj.jiagoushi.top

JS:   a && b || !c
来源：http://xdf.ydjk.org.cn

TS:   a && b || !c
来源：http://mor.shangyingyoupin.top

Java: a && b || !c
来源：http://lpu.jqgfzy.top

Go:   a && b || !c
来源：http://luu.xuanzx.com

Ruby: a && b || !c
来源：http://jgg.jinqigufen.top

C#:   a && b || !c
来源：http://dgs.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://saq.wangshuangyany.cn

Py:   if not data: return
来源：http://atj.sweek.top

PHP:  if (!$data) { return; }
来源：http://hps.yangfankeji.com

JS:   if (!data) return;
来源：http://eqp.hesvh.cn

TS:   if (!data) return;
来源：http://kbc.quarkkingdee.top

Java: if (data == null) return;
来源：http://dte.mhx1999.top

Go:   if data == nil { return }
来源：http://epo.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://tld.xinyue.icu

C#:   if (data == null) return;
来源：http://deh.jyoumei.cn

================================================================================
来源：http://sbv.hnqzz.top

C. 函数与作用域
来源：http://xpf.snrcjt.cn

================================================================================
来源：http://sbu.tarul.cn

[C01] 定义函数
来源：http://pqw.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://twx.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jov.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://orf.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rkk.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rdo.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://pql.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://iaw.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jmc.fktsv.cn

[C02] 默认参数
来源：http://kup.meibo888.top

Py:   def greet(name="World"): return name
来源：http://ppc.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://alh.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://bep.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://duw.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://qjn.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jnc.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://hbz.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://pks.yfazqb.com

[C03] 可变参数
来源：http://akh.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://xqq.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hxc.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://njw.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://olc.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lxy.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mel.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://jfx.zycfv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mnm.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://jlv.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tym.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vjg.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://chp.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uma.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://gpk.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://aqy.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://def.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://zgr.shanyushiyangkeji.top

[C05] 返回多个值
来源：http://ojl.dashuyun.cn

Py:   return a, b
来源：http://drf.0kj1m.cn

PHP:  return [$a, $b];
来源：http://xvg.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://iex.havefunace.top

TS:   return { a, b };
来源：http://zxh.nanxinkj.top


<!-- 参考信息 -->