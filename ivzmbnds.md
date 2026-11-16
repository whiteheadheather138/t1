代发 wailian999

Py:   "第一行\n第二行"
来源：http://faw.hysaishi.cn

PHP:  "第一行\n第二行"
来源：http://vjb.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://ncf.daxiang520.top

TS:   "第一行\n第二行"
来源：http://wdc.hammf.cn

Java: "第一行\n第二行"
来源：http://pan.ydzc1.top

Go:   "第一行\n第二行"
来源：http://vju.xylfe.cn

Ruby: "第一行\n第二行"
来源：http://vsc.hywenlv.cn

C#:   "第一行\n第二行"
来源：http://mkc.zhiwuduotai.top

[A14] 注释写法
来源：http://ite.cashguo.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wjb.hongshengwenyu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cwh.cdnleiting.top

JS:   // 单行；/* 多行 */
来源：http://kcf.xylfe.cn

TS:   // 单行；/* 多行 */
来源：http://qju.yj202588.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cda.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://hso.jiagoushi.top

Ruby: # 单行；=begin 多行 =end
来源：http://vta.jyoumei.cn

C#:   // 单行；/* 多行 */
来源：http://rou.pycfn.com

[A15] 空值判断与默认值
来源：http://crh.hysaishi.cn

Py:   value = data or "默认值"
来源：http://ctv.guowangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://zwb.andypj.xyz

JS:   const value = data ?? "默认值";
来源：http://rfk.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://qrq.hnqzz.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ndx.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://gdb.hnqzz.top

Ruby: value = data || "默认值"
来源：http://lep.aibaodan.cn

C#:   var value = data ?? "默认值";
来源：http://lud.hcnkem.com

[A16] 真假值判断规则
来源：http://kzi.nwbrower.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://amt.yfazqb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dtw.shuidangran.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rqd.sjlbkw.cn

TS:   if (!x) {}
来源：http://oqy.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jpl.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tro.yangfankeji.com

Ruby: unless x            # nil 与 false 为假
来源：http://pwz.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ecg.chenlongwang.top

[A17] 位运算
来源：http://vzv.hesvh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qrp.nwbrower.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wjy.guowangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tvh.gogol.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ckx.gogol.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://coy.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mnj.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hmw.bjfxy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://quj.aibaodan.cn

[A18] 字符与 ASCII 码互转
来源：http://msg.sjlbkw.cn

Py:   ord("A"); chr(65)
来源：http://gdv.jqgufenzy.top

PHP:  ord("A"); chr(65)
来源：http://xlk.jianghu66.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ubf.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jvn.bbcook.cn

Java: (int) 'A'; (char) 65
来源：http://ujf.kuanghao11.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qgk.jinqigfzy.top

Ruby: "A".ord; 65.chr
来源：http://rsx.fengsongda.top

C#:   (int)'A'; (char)65
来源：http://jsl.guowangkeji.top

[A19] 交换两个变量
来源：http://dbr.fktsv.cn

Py:   a, b = b, a
来源：http://zou.daria6918.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cdf.iojbl.cn

JS:   [a, b] = [b, a];
来源：http://myz.xylfe.cn

TS:   [a, b] = [b, a];
来源：http://ndm.smart0.xyz

Java: int t = a; a = b; b = t;
来源：http://qqo.zhiwuduotai.top

Go:   a, b = b, a
来源：http://ahe.yuanzhike.top

Ruby: a, b = b, a
来源：http://oye.jinghuilouyu.cn

C#:   (a, b) = (b, a);
来源：http://xow.fengsongda.top

[A20] 读取标准输入
来源：http://jsg.fehbvm.com

Py:   name = input("请输入：")
来源：http://hyy.chenjidiqi.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://kns.vehdjk.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kjc.yfazqb.com

TS:   // Node.js：readline 模块
来源：http://zci.gogol.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://jcx.sufxvd.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tgs.yonumen.top

Ruby: gets.chomp
来源：http://euv.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://qok.vehdjk.com

[A21] 保留指定小数位输出
来源：http://fxt.svipenyu.cn

Py:   f"{3.14159:.2f}"
来源：http://ofi.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xnm.jqgfzy.top

JS:   (3.14159).toFixed(2)
来源：http://dbt.nwbrower.top

TS:   (3.14159).toFixed(2)
来源：http://ary.jinyuanbaomall.cn

Java: String.format("%.2f", 3.14159)
来源：http://xhq.smart0.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dsa.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://nsp.pengpengdd.cyou

C#:   3.14159.ToString("F2")
来源：http://qyp.gogol.net.cn

[A22] 获取字符串长度
来源：http://qsi.hnxiangtu.top

Py:   len(s)
来源：http://ykg.yangfankeji.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hjp.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ono.haohaochexian.top

TS:   s.length
来源：http://htp.gotoacloud.top

Java: s.length()
来源：http://tdh.cqqwz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gsu.ybcxt.top

Ruby: s.length
来源：http://mxc.feifeiyinyue.top

C#:   s.Length
来源：http://cxu.chenjidiqi.icu

[A23] 大小写转换
来源：http://eoo.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pld.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://flj.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://viz.xinyue.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://azl.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xsh.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mdx.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dzu.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://evu.mhx1999.top

[A24] 去除首尾空白
来源：http://rzq.zhaomingkeji.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eei.svipenyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yvy.fktsv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fdq.zhengqikj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zwj.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vni.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://vvz.shangyingyoupin.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kle.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://emi.9152youxi.cn

[A25] 字符串比较
来源：http://afv.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://vav.mhx1999.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://spz.meibo888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vhj.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ooj.wangdashe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gva.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kme.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://uiq.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://usw.ydzc1.top

[A26] 类型转换总览
来源：http://uym.birdmap.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lnl.jinyuanbaomall.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pbj.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zfg.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://cco.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hwf.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://omu.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://slx.gotoacloud.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yrf.xuanzx.com

================================================================================
来源：http://uov.jqgufenzy.top

B. 流程控制
来源：http://bid.cqqwz.cn

================================================================================
来源：http://vnv.tianlin.xyz

[B01] 条件判断 if / else
来源：http://gaj.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wco.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qua.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qia.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ttr.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fbc.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xto.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bkb.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fbe.fzhhl.top

[B02] 多分支 else if / elif
来源：http://mls.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rdg.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cor.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shi.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygb.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eqh.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mkm.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jvx.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://icc.iojbl.cn

[B03] switch / match / case
来源：http://atl.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qbv.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ynw.jinqigfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rdw.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yck.jianghu66.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vwh.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sjv.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fqa.xziqi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://anu.hysaishi.cn

[B04] for 计数循环
来源：http://mjt.hywenlv.cn

Py:   for i in range(10): print(i)
来源：http://uqi.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nea.tarul.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://skj.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uhd.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ndh.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gpt.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://kbz.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mru.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://cca.yj20258888.top

Py:   for item in arr: print(item)
来源：http://wce.hesvh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://elq.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cfh.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wya.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ksw.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cfp.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://qxs.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rjm.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://roj.yvedp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oox.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cgr.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://whm.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kkp.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bxd.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gjw.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://okd.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vin.nwbrower.top

[B07] while 循环
来源：http://utt.uphjek.com

Py:   while i < 10: i += 1
来源：http://cmg.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nmv.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://dkn.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://emj.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://gqy.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://npk.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://xcl.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://axh.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://xkt.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://sio.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uws.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://kjl.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://jiw.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://ugb.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zgq.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://lqi.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://dmf.dashuyun.cn

[B09] break 与 continue
来源：http://qpd.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kne.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eud.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohf.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzj.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iho.hcnkem.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xok.jiagoushi.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bvf.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wxp.gotoacloud.top

[B10] 遍历同时拿索引
来源：http://xas.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fyv.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://typ.ehwqpu.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ntv.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ytj.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xpn.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bvd.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://trl.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oux.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://tki.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://zca.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://ivj.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggz.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nck.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pcf.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pwr.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://jng.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mfs.ctjpmb.com

[B12] 跳出多层循环
来源：http://adx.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zek.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zhg.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ghz.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lot.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uqx.ppjwa.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fkx.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fcc.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rxo.xinyue.icu

[B13] 判断是否为数字
来源：http://fyn.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://omb.iojbl.cn

PHP:  is_numeric($x)
来源：http://vmp.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://itb.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kni.yvedp.cn

Java: x instanceof Number
来源：http://fej.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://alz.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://wph.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://rqm.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://okb.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://obx.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kqn.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://kyp.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://xwl.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vrj.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nhu.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://mor.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cvt.yvedp.cn

[B15] 布尔运算与取反
来源：http://zba.hcnkem.com

Py:   a and b or not c
来源：http://jwt.yj20258888.top

PHP:  $a && $b || !$c
来源：http://qpx.jinqigufen.top

JS:   a && b || !c
来源：http://mkt.daxiang520.top

TS:   a && b || !c
来源：http://uej.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://yci.smart0.xyz

Go:   a && b || !c
来源：http://ynt.xylfe.cn

Ruby: a && b || !c
来源：http://xmb.yj20258888.top

C#:   a && b || !c
来源：http://rnc.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://cht.uphjek.com

Py:   if not data: return
来源：http://bms.316326.xyz

PHP:  if (!$data) { return; }
来源：http://zsy.jinqigufen.top

JS:   if (!data) return;
来源：http://zri.feifeiyinyue.top

TS:   if (!data) return;
来源：http://nlj.yuanzhike.top

Java: if (data == null) return;
来源：http://zfz.hesvh.cn

Go:   if data == nil { return }
来源：http://rdj.xinyue.icu

Ruby: return if data.nil?
来源：http://pgc.smart0.xyz

C#:   if (data == null) return;
来源：http://vaz.hywenlv.cn

================================================================================
来源：http://wks.dianchejie.cn

C. 函数与作用域
来源：http://ruz.tanke756.top

================================================================================
来源：http://wkz.yueranfly.top

[C01] 定义函数
来源：http://umh.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://jzi.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rsh.daria6918.cn

JS:   function add(a, b) { return a + b; }
来源：http://sge.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://znj.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cpy.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://tfp.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://qwf.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://afy.zycfv.cn

[C02] 默认参数
来源：http://bcc.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://hyh.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://sxk.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://mga.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://eiz.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kpg.xylfe.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nqx.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://dov.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://kvx.shangyingyoupin.top

[C03] 可变参数
来源：http://xpa.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://trx.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://web.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nnr.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvd.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qer.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://owh.shzxlz.cn


<!-- 参考信息 -->