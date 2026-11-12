代发 wailian999

[A14] 注释写法
来源：http://fia.cucudq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lni.smart0.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://jka.zhixingplan.top

JS:   // 单行；/* 多行 */
来源：http://pka.chenjidiqi.icu

TS:   // 单行；/* 多行 */
来源：http://szc.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://umj.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://ypn.sjlbkw.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qzv.jqgufenzy.top

C#:   // 单行；/* 多行 */
来源：http://zzf.mhx1999.top

[A15] 空值判断与默认值
来源：http://dii.jiagoushi.top

Py:   value = data or "默认值"
来源：http://ely.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://wmp.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://frf.hongshengwenyu.top

TS:   const value = data ?? "默认值";
来源：http://thb.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tnb.zdbjq.cn

Go:   if data == "" { data = "默认值" }
来源：http://kge.gzhubu.top

Ruby: value = data || "默认值"
来源：http://fzy.ehwqpu.com

C#:   var value = data ?? "默认值";
来源：http://ysj.daria6918.cn

[A16] 真假值判断规则
来源：http://pat.sxryk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://myj.pycfn.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yxo.zycfv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bvx.jiagoushi.top

TS:   if (!x) {}
来源：http://dnc.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oxl.zhaomingkeji.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://edl.ctjpmb.com

Ruby: unless x            # nil 与 false 为假
来源：http://wzr.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://igc.ybcxt.top

[A17] 位运算
来源：http://kpz.jlsjyb.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iyn.ydzc1.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uvj.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yxm.0kj1m.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zwk.hnqzz.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hzu.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wov.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bre.zdbjq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xgp.yj20258888.top

[A18] 字符与 ASCII 码互转
来源：http://dyb.hnxiangtu.top

Py:   ord("A"); chr(65)
来源：http://zhm.meibo888.top

PHP:  ord("A"); chr(65)
来源：http://vmq.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://alc.jqgufenzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tvi.meibo888.top

Java: (int) 'A'; (char) 65
来源：http://avp.sysykeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lpc.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://xwj.fehbvm.com

C#:   (int)'A'; (char)65
来源：http://kmi.fktsv.cn

[A19] 交换两个变量
来源：http://aea.yj20258888.top

Py:   a, b = b, a
来源：http://exj.snrcjt.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uur.tian-w.cn

JS:   [a, b] = [b, a];
来源：http://lui.feifeiyinyue.top

TS:   [a, b] = [b, a];
来源：http://udc.havefunace.top

Java: int t = a; a = b; b = t;
来源：http://iyg.havefunace.top

Go:   a, b = b, a
来源：http://ldd.hesvh.cn

Ruby: a, b = b, a
来源：http://sea.xinyue.icu

C#:   (a, b) = (b, a);
来源：http://xvl.gotoacloud.top

[A20] 读取标准输入
来源：http://tnt.yj20258888.top

Py:   name = input("请输入：")
来源：http://qtp.yanxiufei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fqf.hysaishi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hft.andypj.xyz

TS:   // Node.js：readline 模块
来源：http://lup.gotoacloud.top

Java: new Scanner(System.in).nextLine()
来源：http://fau.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iig.nwbrower.top

Ruby: gets.chomp
来源：http://iua.zhengqikj.top

C#:   Console.ReadLine();
来源：http://nic.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://qtx.bbcook.cn

Py:   f"{3.14159:.2f}"
来源：http://cfr.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://stt.aizwys.cn

JS:   (3.14159).toFixed(2)
来源：http://coe.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://hdf.xuanzx.com

Java: String.format("%.2f", 3.14159)
来源：http://kuk.tarul.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://khg.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://bnl.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://qnr.sweek.top

[A22] 获取字符串长度
来源：http://ngy.nanxuanxn.top

Py:   len(s)
来源：http://fmg.nwbrower.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vyk.guowangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ilm.yj20258.top

TS:   s.length
来源：http://jwk.svipenyu.cn

Java: s.length()
来源：http://fmu.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gpt.shangyingyoupin.top

Ruby: s.length
来源：http://knp.gotoacloud.top

C#:   s.Length
来源：http://ifd.sysykeji.top

[A23] 大小写转换
来源：http://aim.jqgfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gwf.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bpp.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kwl.mhx1999.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rnt.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://osj.kuanghao11.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ghx.tian-w.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://osl.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eok.hammf.cn

[A24] 去除首尾空白
来源：http://zbt.ctjpmb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ujz.xinyue.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qdq.ywan-chungtsiang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://izz.zhoulong.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lji.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sfx.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://gvl.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tqr.yj20258.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wqu.xuanzx.com

[A25] 字符串比较
来源：http://ajk.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://dik.316326.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bpb.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jep.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zxt.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://exk.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tdc.chenlongwang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wzg.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kqe.nwbrower.top

[A26] 类型转换总览
来源：http://mpa.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mfg.hammf.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://chd.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://del.yonumen.top

TS:   Number() String() Boolean() x as number
来源：http://ftt.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gfk.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ohd.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rpw.vqdsnc.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yci.meibo888.top

================================================================================
来源：http://jxa.jqgfzy.top

B. 流程控制
来源：http://gjn.epnwcf.com

================================================================================
来源：http://ign.dianchejie.cn

[B01] 条件判断 if / else
来源：http://mqe.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fes.hammf.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hmq.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://keu.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kkw.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pte.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zgb.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://egm.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://csv.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://mny.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dly.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://npt.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqf.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cod.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ojb.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zkc.sxryk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wzt.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lne.shuidangran.top

[B03] switch / match / case
来源：http://eyy.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vbc.gzhubu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nbd.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qpa.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lpi.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vun.cucudq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jbb.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tzi.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oup.yfazqb.com

[B04] for 计数循环
来源：http://pqa.andypj.xyz

Py:   for i in range(10): print(i)
来源：http://qvq.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ybm.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wgw.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swl.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kiz.fehbvm.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qvk.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://gvf.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wnv.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://dhh.sxryk.cn

Py:   for item in arr: print(item)
来源：http://ceh.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ysz.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://owi.jinqigfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lec.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://hfw.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nmg.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://zui.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lwp.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://jcc.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mxp.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yms.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hfw.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iyt.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ifc.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ekk.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://izd.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xuw.pengpengdd.cyou

[B07] while 循环
来源：http://tzz.daria6918.cn

Py:   while i < 10: i += 1
来源：http://ihz.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://hci.jqgufenzy.top

JS:   while (i < 10) { i++; }
来源：http://vqr.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://hhl.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://vvr.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lmi.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://dzc.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://xrr.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://hmx.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://syy.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://qom.aibaodan.cn

JS:   do { i++; } while (i < 10);
来源：http://bcg.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://zkg.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://lww.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://spx.shanyushiyangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://awl.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://tfy.ppjwa.cn

[B09] break 与 continue
来源：http://jjn.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tbz.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jyk.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvz.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hje.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dai.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zbf.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eem.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gdn.daxiang520.top

[B10] 遍历同时拿索引
来源：http://mxv.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kfp.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tvx.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pvl.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gje.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ioe.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oyb.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pii.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kvl.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://mvv.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://mmu.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://skt.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qza.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://azn.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://liq.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iwf.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://bic.fehbvm.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wid.yvedp.cn

[B12] 跳出多层循环
来源：http://lht.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://whd.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://epo.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://app.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gzl.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dfe.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hzz.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cmu.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aqv.hfpthk.cn

[B13] 判断是否为数字
来源：http://cfy.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://aqq.hesvh.cn

PHP:  is_numeric($x)
来源：http://npb.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://asw.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zav.cashguo.top

Java: x instanceof Number
来源：http://trh.jqgfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ksb.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://zms.xuanzx.com

C#:   x is int or double or decimal
来源：http://prm.c1oappe.top

[B14] 判断值是否在集合内
来源：http://prn.jinghuilouyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yxe.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zni.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://brw.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://ceq.yueranfly.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tzr.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iib.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://ozk.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lsk.jyoumei.cn

[B15] 布尔运算与取反
来源：http://pen.fktsv.cn

Py:   a and b or not c
来源：http://nwd.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://pzf.sxryk.cn

JS:   a && b || !c
来源：http://ipa.svipenyu.cn

TS:   a && b || !c
来源：http://zou.cucudq.cn

Java: a && b || !c
来源：http://zae.yonumen.top

Go:   a && b || !c
来源：http://afp.daxiang520.top

Ruby: a && b || !c
来源：http://xyk.nwbrower.top

C#:   a && b || !c
来源：http://zjo.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://cgx.hywenlv.cn

Py:   if not data: return
来源：http://uxh.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://vnr.svipenyu.cn

JS:   if (!data) return;
来源：http://oey.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://vap.smart0.xyz

Java: if (data == null) return;
来源：http://rvc.mhx1999.top

Go:   if data == nil { return }
来源：http://wdm.iojbl.cn

Ruby: return if data.nil?
来源：http://gqt.jinqigfzy.top

C#:   if (data == null) return;
来源：http://mqc.iojbl.cn

================================================================================
来源：http://tvm.smart0.xyz

C. 函数与作用域
来源：http://tui.chenlongwang.top

================================================================================
来源：http://jms.jinqigfzy.top

[C01] 定义函数
来源：http://wig.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://mqq.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://llk.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://bxk.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yom.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ole.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://fcl.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://msa.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dll.cashguo.top

[C02] 默认参数
来源：http://mkb.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://prh.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zlt.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://gmp.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mdm.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cxd.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pdg.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://kwn.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://rtv.9152youxi.cn

[C03] 可变参数
来源：http://eqc.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://ogj.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ibc.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uee.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://abc.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yjo.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ynj.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://ovn.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://scb.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://yok.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lyu.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jbw.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ckn.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yfm.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://tnj.gotoacloud.top


<!-- 参考信息 -->