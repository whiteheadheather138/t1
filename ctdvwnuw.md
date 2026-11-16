代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://atv.daxiang520.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://abo.cheryme.top

TS:   if (!x) {}
来源：http://lpq.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ztx.ydjk.org.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vsc.jqgufenzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://dkm.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cay.pycfn.com

[A17] 位运算
来源：http://eyx.hcnkem.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmo.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kfs.dashuyun.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qra.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rwp.andypj.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ein.bbcook.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rzz.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://myw.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hng.xziqi.cn

[A18] 字符与 ASCII 码互转
来源：http://ews.yvedp.cn

Py:   ord("A"); chr(65)
来源：http://hjv.gaohongyu789.top

PHP:  ord("A"); chr(65)
来源：http://pcr.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hdw.hfpthk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rcu.gogol.net.cn

Java: (int) 'A'; (char) 65
来源：http://loy.0kj1m.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vuv.cheryme.top

Ruby: "A".ord; 65.chr
来源：http://zbr.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://rnc.nanxinkj.top

[A19] 交换两个变量
来源：http://qou.nanxuanxn.top

Py:   a, b = b, a
来源：http://vli.zhoulong.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://nmc.hesvh.cn

JS:   [a, b] = [b, a];
来源：http://fvx.zhongyouzk.top

TS:   [a, b] = [b, a];
来源：http://enn.gogol.net.cn

Java: int t = a; a = b; b = t;
来源：http://mrj.nanxinkj.top

Go:   a, b = b, a
来源：http://qlz.fzhhl.top

Ruby: a, b = b, a
来源：http://fuv.fengsongda.top

C#:   (a, b) = (b, a);
来源：http://hms.zhengqikj.top

[A20] 读取标准输入
来源：http://clx.guannengcc.top

Py:   name = input("请输入：")
来源：http://tii.yvedp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rln.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bmb.snrcjt.cn

TS:   // Node.js：readline 模块
来源：http://ydq.cashguo.top

Java: new Scanner(System.in).nextLine()
来源：http://igr.vehdjk.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ouh.havefunace.top

Ruby: gets.chomp
来源：http://syh.fzhhl.top

C#:   Console.ReadLine();
来源：http://goh.hnqzz.top

[A21] 保留指定小数位输出
来源：http://zfs.gogol.net.cn

Py:   f"{3.14159:.2f}"
来源：http://qfm.jinqigfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hac.kuanghao11.cn

JS:   (3.14159).toFixed(2)
来源：http://xjv.hnqzz.top

TS:   (3.14159).toFixed(2)
来源：http://qmk.xuetiantiany.cn

Java: String.format("%.2f", 3.14159)
来源：http://vaz.gaohongyu789.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://aqm.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://eqw.snrcjt.cn

C#:   3.14159.ToString("F2")
来源：http://qbj.pengpengdd.cyou

[A22] 获取字符串长度
来源：http://mbg.epnwcf.com

Py:   len(s)
来源：http://sav.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ufy.cheryme.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fct.jqgfzy.top

TS:   s.length
来源：http://adi.quarkkingdee.top

Java: s.length()
来源：http://exj.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nsv.mhx1999.top

Ruby: s.length
来源：http://ovq.jianghu66.top

C#:   s.Length
来源：http://cvp.zhixingplan.top

[A23] 大小写转换
来源：http://tjb.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nsf.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jxd.zhongyouzk.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://opl.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eqz.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ttp.yangfankeji.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ath.tian-w.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jjr.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://xbn.zhaomingkeji.xyz

[A24] 去除首尾空白
来源：http://prn.bbcook.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vdp.yanxiufei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zzc.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ngh.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kdp.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cjv.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://ajs.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bgj.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://skn.ydzc1.top

[A25] 字符串比较
来源：http://dej.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://lcg.cqqwz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ynj.fktsv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wlk.zdqjudy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://upk.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yui.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ssu.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ftk.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gfb.iojbl.cn

[A26] 类型转换总览
来源：http://onb.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://haz.hywenlv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kqk.nanxuanxn.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://syl.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://qwd.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oga.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://anf.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fkm.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kih.ivvv.top

================================================================================
来源：http://kdv.sjlbkw.cn

B. 流程控制
来源：http://mcc.yvedp.cn

================================================================================
来源：http://aqd.hywenlv.cn

[B01] 条件判断 if / else
来源：http://mdo.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://byg.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ltv.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://luj.ywan-chungtsiang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ikh.snrcjt.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://osc.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wue.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ags.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://twy.hammf.cn

[B02] 多分支 else if / elif
来源：http://kja.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hze.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qwo.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swl.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vhi.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxs.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jlq.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qit.zhiwuduotai.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exs.zhoulong.xyz

[B03] switch / match / case
来源：http://voa.zhongyouzk.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dof.guannengcc.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ylb.jinqigufen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xyp.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hll.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tmh.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jvl.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pem.nanxinkj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ccv.chenlongwang.top

[B04] for 计数循环
来源：http://zhl.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://ntc.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pxe.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://psd.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bui.zycfv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oga.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ulr.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://gaw.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://amj.uphjek.com

[B05] 遍历数组 / 列表
来源：http://sgu.shanyushiyangtech.top

Py:   for item in arr: print(item)
来源：http://vfc.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wqq.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://feb.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nim.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://jid.wangdashe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qqw.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://jim.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://afm.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://khn.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tdl.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kct.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yli.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qsk.shuidangran.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ggb.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xje.yanxiufei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jta.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jxv.52xcode.cn

[B07] while 循环
来源：http://snb.redwolf501.top

Py:   while i < 10: i += 1
来源：http://kuj.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://zjp.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://giu.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://sme.meibo888.top

Java: while (i < 10) { i++; }
来源：http://efz.sjlbkw.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tjt.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://eqa.chenjidiqi.icu

C#:   while (i < 10) { i++; }
来源：http://mov.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://frr.zhongyouzk.top

Py:   # 无 do-while：用 while True + break
来源：http://ixp.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rbz.yfazqb.com

JS:   do { i++; } while (i < 10);
来源：http://get.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://dxz.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://cdu.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rtq.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xas.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://swg.shangyingyoupin.top

[B09] break 与 continue
来源：http://rne.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jgj.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://evt.smart0.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsh.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://daz.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trq.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vrh.zdqjudy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xnv.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gia.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://asl.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bcl.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zsw.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pnc.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dxo.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lmv.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dqc.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wpt.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oex.hcnkem.com

[B11] 生成数字序列 / 区间
来源：http://vzc.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://ibl.yj20258.top

PHP:  range(0, 10, 2);
来源：http://vvg.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pdg.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://agw.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aho.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xai.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://xcd.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wnv.zhengqikj.top

[B12] 跳出多层循环
来源：http://qil.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wka.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rwc.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nca.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hbt.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vtt.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ewl.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qpl.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://whl.yfazqb.com

[B13] 判断是否为数字
来源：http://cqp.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://dvi.nwbrower.top

PHP:  is_numeric($x)
来源：http://rgq.tian-w.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ybu.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dye.yonumen.top

Java: x instanceof Number
来源：http://uej.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ryz.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://xrw.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://acl.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://prf.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pno.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zsd.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://kmr.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://dba.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mmp.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dwm.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://mar.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uld.316326.xyz

[B15] 布尔运算与取反
来源：http://qjp.fzhhl.top

Py:   a and b or not c
来源：http://sqy.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://oas.yvedp.cn

JS:   a && b || !c
来源：http://utz.sjlbkw.cn

TS:   a && b || !c
来源：http://gpt.ppjwa.cn

Java: a && b || !c
来源：http://ozp.wangshuangyany.cn

Go:   a && b || !c
来源：http://wwc.guowangkeji.top

Ruby: a && b || !c
来源：http://uqy.jianghu66.top

C#:   a && b || !c
来源：http://kfc.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ohw.316326.xyz

Py:   if not data: return
来源：http://iwt.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://uxb.nanxinkj.top

JS:   if (!data) return;
来源：http://cym.zdqjudy.top

TS:   if (!data) return;
来源：http://hej.zycfv.cn

Java: if (data == null) return;
来源：http://sog.jinqigfzy.top

Go:   if data == nil { return }
来源：http://xre.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://qrn.sweek.top

C#:   if (data == null) return;
来源：http://kik.feifeiyinyue.top

================================================================================
来源：http://stn.9152youxi.cn

C. 函数与作用域
来源：http://qaa.ctjpmb.com

================================================================================
来源：http://srk.zhaomingkeji.xyz

[C01] 定义函数
来源：http://oxy.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://zey.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pzr.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://jjk.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xsm.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rnf.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uer.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://rlj.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jnb.tarul.cn

[C02] 默认参数
来源：http://ych.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://mla.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xfx.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://zat.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://vtn.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zpp.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eyf.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://cin.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://xyc.chenzaomai.com

[C03] 可变参数
来源：http://fwy.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://oni.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eyk.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uct.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cpn.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zzn.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://scn.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://agx.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ufh.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://gnn.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zjr.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vng.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bbf.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jzn.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://vsq.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://hkv.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://tlm.chenjidiqi.icu

C#:   f(a: 1, b: 2)
来源：http://uow.bbcook.cn

[C05] 返回多个值
来源：http://hvc.ybcxt.top

Py:   return a, b
来源：http://tby.jianghu66.top

PHP:  return [$a, $b];
来源：http://nhf.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ugs.yueranfly.top

TS:   return { a, b };
来源：http://xao.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vmj.tanke756.top

Go:   return a, b
来源：http://jkd.guowangkeji.top

Ruby: return a, b
来源：http://ddg.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://tlo.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://aen.xylfe.cn

Py:   square = lambda x: x * x
来源：http://owj.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ile.chenzaomai.com

JS:   const square = x => x * x;
来源：http://akq.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://txu.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fkj.yongpay.top

Go:   sq := func(x int) int { return x * x }
来源：http://xso.hnxiangtu.top

Ruby: square = ->(x) { x * x }
来源：http://mui.hysaishi.cn


<!-- 参考信息 -->