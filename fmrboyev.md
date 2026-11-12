代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hxy.xingfuxueyuan.xyz

Ruby: "Hello, #{name}!"
来源：http://ung.fktsv.cn

C#:   $"Hello, {name}!"
来源：http://zer.nanxuanxn.top

[A13] 多行字符串（练习 \n 转义）
来源：http://aza.fktsv.cn

Py:   "第一行\n第二行"
来源：http://mko.pycfn.com

PHP:  "第一行\n第二行"
来源：http://zcr.yuxming.cn

JS:   "第一行\n第二行"
来源：http://psi.birdmap.top

TS:   "第一行\n第二行"
来源：http://ghy.jianghu66.top

Java: "第一行\n第二行"
来源：http://xyg.yueranfly.top

Go:   "第一行\n第二行"
来源：http://tip.ivvv.top

Ruby: "第一行\n第二行"
来源：http://phi.kuanghao11.cn

C#:   "第一行\n第二行"
来源：http://nxe.fzhhl.top

[A14] 注释写法
来源：http://xrm.sxryk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://czf.wangdashe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kbw.nanxinkj.top

JS:   // 单行；/* 多行 */
来源：http://xpw.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://rfz.chenzaomai.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kit.gzhubu.top

Go:   // 单行；/* 多行 */
来源：http://noa.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://ftp.bbcook.cn

C#:   // 单行；/* 多行 */
来源：http://qmy.zdbjq.cn

[A15] 空值判断与默认值
来源：http://two.shzxlz.cn

Py:   value = data or "默认值"
来源：http://umm.gaohongyu789.top

PHP:  $value = $data ?? "默认值";
来源：http://owa.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://qmh.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://ozo.ivvv.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://aei.havefunace.top

Go:   if data == "" { data = "默认值" }
来源：http://tnj.redwolf501.top

Ruby: value = data || "默认值"
来源：http://crm.ctjpmb.com

C#:   var value = data ?? "默认值";
来源：http://cay.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://lzk.zdbjq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rbc.gogol.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dqt.jinqigufen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nvp.cucudq.cn

TS:   if (!x) {}
来源：http://hzf.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kou.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zhj.zhiwuduotai.top

Ruby: unless x            # nil 与 false 为假
来源：http://aen.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eqx.zhixingplan.top

[A17] 位运算
来源：http://ubr.zhijiandao.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjo.bjfxy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bhg.nanxuanxn.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pdz.hammf.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vzi.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pcp.hesvh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xfn.jlsjyb.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vjv.ydjk.org.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxw.jqgfzy.top

[A18] 字符与 ASCII 码互转
来源：http://jad.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://euu.svipenyu.cn

PHP:  ord("A"); chr(65)
来源：http://jjs.zhixingplan.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oaf.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qsr.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://ryl.cheryme.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bqb.hongshengwenyu.top

Ruby: "A".ord; 65.chr
来源：http://lcn.tianlin.xyz

C#:   (int)'A'; (char)65
来源：http://ghc.xuetiantiany.cn

[A19] 交换两个变量
来源：http://qtp.ehwqpu.com

Py:   a, b = b, a
来源：http://kar.ivvv.top

PHP:  [$a, $b] = [$b, $a];
来源：http://amw.smart0.xyz

JS:   [a, b] = [b, a];
来源：http://xls.aizwys.cn

TS:   [a, b] = [b, a];
来源：http://qsb.guowangkeji.top

Java: int t = a; a = b; b = t;
来源：http://jjy.nanxinkj.top

Go:   a, b = b, a
来源：http://ixy.guannengcc.top

Ruby: a, b = b, a
来源：http://yjp.ydjk.org.cn

C#:   (a, b) = (b, a);
来源：http://cbf.meibo888.top

[A20] 读取标准输入
来源：http://grs.zdqjudy.top

Py:   name = input("请输入：")
来源：http://jfj.tarul.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nvp.zhijiandao.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ljf.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://djv.shanyushiyangtech.top

Java: new Scanner(System.in).nextLine()
来源：http://wez.cashguo.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vnt.hfpthk.cn

Ruby: gets.chomp
来源：http://qxq.wangshuangyany.cn

C#:   Console.ReadLine();
来源：http://gai.tanke756.top

[A21] 保留指定小数位输出
来源：http://ztk.bjfxy.top

Py:   f"{3.14159:.2f}"
来源：http://grb.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://loo.jqgufenzy.top

JS:   (3.14159).toFixed(2)
来源：http://ptf.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://qpu.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://hjv.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gyd.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://zxo.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://ujp.aizwys.cn

[A22] 获取字符串长度
来源：http://auc.pengpengdd.cyou

Py:   len(s)
来源：http://jxo.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uxh.cdnleiting.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zjv.52xcode.cn

TS:   s.length
来源：http://opr.zhoulong.xyz

Java: s.length()
来源：http://nux.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qga.yongpay.top

Ruby: s.length
来源：http://xrk.tanke756.top

C#:   s.Length
来源：http://wxo.fanxiaobao.xyz

[A23] 大小写转换
来源：http://dcz.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://eeo.shanyushiyangtech.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://etd.shzxlz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://god.tian-w.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wom.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vma.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oon.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jab.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fjz.cucudq.cn

[A24] 去除首尾空白
来源：http://vwm.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fzb.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ccd.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gov.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jgx.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fsl.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://ent.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aca.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://clk.xuetiantiany.cn

[A25] 字符串比较
来源：http://fmp.yfazqb.com

Py:   s1 == s2; s1 != s2
来源：http://rpg.hesvh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jiu.redwolf501.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hmf.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yse.ydzc1.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vjj.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dds.xingfuxueyuan.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://yph.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wnc.fehbvm.com

[A26] 类型转换总览
来源：http://ssc.52xcode.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qdc.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qcq.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://myi.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://slm.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ipa.aizwys.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oml.tanke756.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://uav.dashuyun.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ovo.zdbjq.cn

================================================================================
来源：http://joj.sufxvd.cn

B. 流程控制
来源：http://ggs.yj20258.top

================================================================================
来源：http://krd.zycfv.cn

[B01] 条件判断 if / else
来源：http://yuy.wangshuangyany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ouk.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kcw.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ngg.9152youxi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gvi.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cze.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tof.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qdm.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://prq.aizwys.cn

[B02] 多分支 else if / elif
来源：http://gjo.shangyingyoupin.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ywe.birdmap.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ikq.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfc.zhiwuduotai.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogx.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hfs.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ggg.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://foh.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndn.iojbl.cn

[B03] switch / match / case
来源：http://piv.ivvv.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mcr.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aja.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kby.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nts.xylfe.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wxj.yonumen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://skt.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fjy.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ugb.cdnleiting.top

[B04] for 计数循环
来源：http://ggi.yj20258.top

Py:   for i in range(10): print(i)
来源：http://hkf.jianghu66.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bmz.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vwg.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bij.zhijiandao.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dwf.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nhc.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://vzm.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bmf.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://pgf.meibo888.top

Py:   for item in arr: print(item)
来源：http://icp.smart0.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hgj.bbcook.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gvv.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cwt.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dmj.cdnleiting.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://reu.zhengqikj.top

Ruby: arr.each { |item| puts item }
来源：http://hhr.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vbu.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://okg.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ebr.kuanghao11.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yny.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://anp.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uam.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uxb.ivvv.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cmg.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://haz.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yek.ctjpmb.com

[B07] while 循环
来源：http://rcx.uphjek.com

Py:   while i < 10: i += 1
来源：http://kqv.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jql.hnxiangtu.top

JS:   while (i < 10) { i++; }
来源：http://vqv.wangshuangyany.cn

TS:   while (i < 10) { i++; }
来源：http://jap.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://dzm.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://plh.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://htj.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://mzv.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://pyw.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://olm.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://thc.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://axs.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://vby.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://tvd.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://yzu.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rrj.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://agp.hcnkem.com

[B09] break 与 continue
来源：http://fwu.chenjidiqi.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ykq.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wrf.ctjpmb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hyi.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfv.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oip.fktsv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://foo.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vov.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://coa.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://pru.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://szk.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://djc.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bpt.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nqo.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tte.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fay.yueranfly.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cwy.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qhb.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://ujy.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://dad.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://tdq.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ffr.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://shw.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yla.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://szb.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://fgt.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uhn.guowangkeji.top

[B12] 跳出多层循环
来源：http://wlz.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://utm.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bbc.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iqx.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hso.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ics.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lrx.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xoj.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kas.svipenyu.cn

[B13] 判断是否为数字
来源：http://eqc.ybcxt.top

Py:   isinstance(x, (int, float))
来源：http://xkm.shuidangran.top

PHP:  is_numeric($x)
来源：http://gdv.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fgr.nanxuanxn.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bin.tianlin.xyz

Java: x instanceof Number
来源：http://ugu.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://btc.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://hfg.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://tub.bjfxy.top

[B14] 判断值是否在集合内
来源：http://zjw.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rfp.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kbf.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://hwt.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://zoc.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mgh.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://srf.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://tah.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://exe.zhixingplan.top

[B15] 布尔运算与取反
来源：http://xkn.ivvv.top

Py:   a and b or not c
来源：http://sob.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://esr.fzhhl.top

JS:   a && b || !c
来源：http://fte.cdnleiting.top

TS:   a && b || !c
来源：http://vhz.hnqzz.top

Java: a && b || !c
来源：http://msd.quarkkingdee.top

Go:   a && b || !c
来源：http://jal.sxryk.cn

Ruby: a && b || !c
来源：http://uat.sweek.top

C#:   a && b || !c
来源：http://gao.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qzu.yfazqb.com

Py:   if not data: return
来源：http://ncq.cheryme.top

PHP:  if (!$data) { return; }
来源：http://edk.hfpthk.cn

JS:   if (!data) return;
来源：http://dvk.bbcook.cn

TS:   if (!data) return;
来源：http://ktx.iojbl.cn

Java: if (data == null) return;
来源：http://hok.yuanzhike.top

Go:   if data == nil { return }
来源：http://imh.gotoacloud.top

Ruby: return if data.nil?
来源：http://zuw.gogol.net.cn

C#:   if (data == null) return;
来源：http://nbz.sxryk.cn

================================================================================
来源：http://xch.havefunace.top

C. 函数与作用域
来源：http://cbv.hnxiangtu.top

================================================================================
来源：http://bwn.tanke756.top

[C01] 定义函数
来源：http://cqq.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://fbw.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gnt.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://wop.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://onw.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xkb.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bfj.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://kgb.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://web.chenzaomai.com

[C02] 默认参数
来源：http://uur.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://lxh.zdbjq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vin.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://bvl.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://czj.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://add.ivvv.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qvi.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://zgh.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://nyc.jinyuanbaomall.cn

[C03] 可变参数
来源：http://bbi.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://sar.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jzp.9152youxi.cn


<!-- 参考信息 -->