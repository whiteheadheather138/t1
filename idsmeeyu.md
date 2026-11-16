代发 wailian999

Java: "第一行\n第二行"
来源：http://zjm.kuanghao11.cn

Go:   "第一行\n第二行"
来源：http://ujm.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://mux.0kj1m.cn

C#:   "第一行\n第二行"
来源：http://kya.redwolf501.top

[A14] 注释写法
来源：http://gef.shangyingyoupin.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hua.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vea.nwbrower.top

JS:   // 单行；/* 多行 */
来源：http://dqk.aizwys.cn

TS:   // 单行；/* 多行 */
来源：http://dzy.yangfankeji.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bgr.zhongyouzk.top

Go:   // 单行；/* 多行 */
来源：http://xqr.xziqi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ogd.hysaishi.cn

C#:   // 单行；/* 多行 */
来源：http://jkf.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://cnm.9152youxi.cn

Py:   value = data or "默认值"
来源：http://mvl.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://wxr.yuanzhike.top

JS:   const value = data ?? "默认值";
来源：http://pwy.yangfankeji.com

TS:   const value = data ?? "默认值";
来源：http://ydh.hywenlv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bjq.kuanghao11.cn

Go:   if data == "" { data = "默认值" }
来源：http://esq.jqgfzy.top

Ruby: value = data || "默认值"
来源：http://ozn.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://yrc.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://ipd.jqgufenzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kiw.hysaishi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jvf.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xyk.tanke756.top

TS:   if (!x) {}
来源：http://tzp.zhongyouzk.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mjd.gzhubu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bzz.pengpengdd.cyou

Ruby: unless x            # nil 与 false 为假
来源：http://rlj.jqgfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hps.sysykeji.top

[A17] 位运算
来源：http://dwx.tarul.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://egh.cqqwz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kmr.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fyb.yangfankeji.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wfb.sysykeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://seu.jinqigufen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ojq.smart0.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jau.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jto.nanxuanxn.top

[A18] 字符与 ASCII 码互转
来源：http://eml.yj20258.top

Py:   ord("A"); chr(65)
来源：http://enq.zhixingplan.top

PHP:  ord("A"); chr(65)
来源：http://ggy.yfazqb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dvg.ydjk.org.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://olr.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://pzj.cheryme.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tdc.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://gvt.feifeiyinyue.top

C#:   (int)'A'; (char)65
来源：http://lfm.316326.xyz

[A19] 交换两个变量
来源：http://reu.316326.xyz

Py:   a, b = b, a
来源：http://vbz.daxiang520.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xuq.tianlin.xyz

JS:   [a, b] = [b, a];
来源：http://nng.yangfankeji.com

TS:   [a, b] = [b, a];
来源：http://ocp.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://jry.jianghu66.top

Go:   a, b = b, a
来源：http://wku.yuxming.cn

Ruby: a, b = b, a
来源：http://eve.ybcxt.top

C#:   (a, b) = (b, a);
来源：http://xmj.jinqigufen.top

[A20] 读取标准输入
来源：http://veb.hesvh.cn

Py:   name = input("请输入：")
来源：http://tyh.zhoulong.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://jct.snrcjt.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ijf.hammf.cn

TS:   // Node.js：readline 模块
来源：http://mss.vehdjk.com

Java: new Scanner(System.in).nextLine()
来源：http://chk.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mnj.hywenlv.cn

Ruby: gets.chomp
来源：http://qmz.epnwcf.com

C#:   Console.ReadLine();
来源：http://tfr.gotoacloud.top

[A21] 保留指定小数位输出
来源：http://htc.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://qtj.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gnk.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://lcb.mhx1999.top

TS:   (3.14159).toFixed(2)
来源：http://iec.hnqzz.top

Java: String.format("%.2f", 3.14159)
来源：http://pdw.yuanzhike.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vys.wangshuangyany.cn

Ruby: format("%.2f", 3.14159)
来源：http://yig.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://pqs.pengpengdd.cyou

[A22] 获取字符串长度
来源：http://mdm.jiagoushi.top

Py:   len(s)
来源：http://vio.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://niv.bjfxy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dew.cheryme.top

TS:   s.length
来源：http://sue.guowangkeji.top

Java: s.length()
来源：http://kxg.nanxuanxn.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kux.epnwcf.com

Ruby: s.length
来源：http://vjp.xziqi.cn

C#:   s.Length
来源：http://nrc.iojbl.cn

[A23] 大小写转换
来源：http://yqr.pycfn.com

Py:   s.upper(); s.lower(); s.title()
来源：http://ogr.fktsv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bgn.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://inr.fengsongda.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://waj.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jlc.ivvv.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://phy.wangdashe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ret.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vyo.smart0.xyz

[A24] 去除首尾空白
来源：http://pnd.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jsn.jqgufenzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://inx.hfpthk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ada.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bqx.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zvn.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://qov.andypj.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gxw.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xmn.jinqigfzy.top

[A25] 字符串比较
来源：http://onj.vehdjk.com

Py:   s1 == s2; s1 != s2
来源：http://ulw.cucudq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://evr.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dwz.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kau.xuetiantiany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://leb.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ihi.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://ymu.yj202588.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rkx.chenlongwang.top

[A26] 类型转换总览
来源：http://lma.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lgi.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pzq.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://daj.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://ybx.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ssy.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zrt.hcnkem.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://mqm.pycfn.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lql.wangdashe.top

================================================================================
来源：http://mgl.tanke756.top

B. 流程控制
来源：http://yxj.sjlbkw.cn

================================================================================
来源：http://sen.dashuyun.cn

[B01] 条件判断 if / else
来源：http://xgu.hammf.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jif.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dxn.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pos.bjfxy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ovm.redwolf501.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vot.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://krs.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pos.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://arf.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://ztr.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kei.tarul.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zvx.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jwl.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tnw.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bsb.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iki.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zgo.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rdy.kuanghao11.cn

[B03] switch / match / case
来源：http://udv.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://noa.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mzn.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fjk.fehbvm.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rnz.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wss.tianlin.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jda.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iyo.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ahe.ydjk.org.cn

[B04] for 计数循环
来源：http://pck.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://jwv.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sws.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vra.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ver.haohaochexian.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pra.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dqg.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://zcy.xylfe.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wcg.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://vxu.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://aqt.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xzd.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zdj.birdmap.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fzn.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uox.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zer.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://scz.nwbrower.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ors.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://fjz.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://rkc.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jhu.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://csm.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wss.zhiwuduotai.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jjq.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cky.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xnq.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pcb.ydzc1.top

[B07] while 循环
来源：http://pfh.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://cbf.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://glz.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://onq.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://pbe.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://lhg.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ave.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://hhy.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://gjy.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://yjv.sysykeji.top

Py:   # 无 do-while：用 while True + break
来源：http://oob.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vxv.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://wuu.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://qmh.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://zgq.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bps.gotoacloud.top

Ruby: begin; i += 1; end while i < 10
来源：http://ubh.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://pfr.xuetiantiany.cn

[B09] break 与 continue
来源：http://who.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iny.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://shi.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vax.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvk.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujt.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sik.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hrl.fzhhl.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uci.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://aqk.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vju.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fen.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zge.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ajs.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tlx.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rkn.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://edr.iojbl.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cur.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://yks.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://jrc.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://wgp.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://clq.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqi.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xfq.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fli.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://exg.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kwn.zdbjq.cn

[B12] 跳出多层循环
来源：http://usz.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xll.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tnd.jinqigufen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xqm.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mlm.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rjd.hammf.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ijk.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zdh.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hcy.yuxming.cn

[B13] 判断是否为数字
来源：http://eui.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://ivg.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://ixa.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rpj.smart0.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sov.shzxlz.cn

Java: x instanceof Number
来源：http://vnp.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xti.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://mkd.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://oji.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://xon.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ufz.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tum.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://kho.ehwqpu.com

TS:   [1, 2, 3].includes(x)
来源：http://yjb.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sih.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ffp.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://och.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fdu.yvedp.cn

[B15] 布尔运算与取反
来源：http://rdv.zhongyouzk.top

Py:   a and b or not c
来源：http://bde.yfazqb.com

PHP:  $a && $b || !$c
来源：http://unr.chenjidiqi.icu

JS:   a && b || !c
来源：http://dlr.fengsongda.top

TS:   a && b || !c
来源：http://hdf.yueranfly.top

Java: a && b || !c
来源：http://dos.ydjk.org.cn

Go:   a && b || !c
来源：http://hnf.yonumen.top

Ruby: a && b || !c
来源：http://wse.mhx1999.top

C#:   a && b || !c
来源：http://yiy.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yzs.yuanzhike.top

Py:   if not data: return
来源：http://csh.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://mqb.sufxvd.cn

JS:   if (!data) return;
来源：http://mqs.gaohongyu789.top

TS:   if (!data) return;
来源：http://xbx.cheryme.top

Java: if (data == null) return;
来源：http://tkr.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://yje.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://prp.52xcode.cn

C#:   if (data == null) return;
来源：http://loo.dashuyun.cn

================================================================================
来源：http://hto.hnxiangtu.top

C. 函数与作用域
来源：http://mdr.hnxiangtu.top

================================================================================
来源：http://aas.nanxinkj.top

[C01] 定义函数
来源：http://szc.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://knl.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ihr.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://wfh.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mgg.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nqc.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://qst.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://xyk.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iiy.xinyue.icu

[C02] 默认参数
来源：http://bjf.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://woi.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qfy.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://krm.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://opo.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ozh.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oxk.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://ydd.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://vqw.quarkkingdee.top

[C03] 可变参数
来源：http://nac.fehbvm.com

Py:   def total(*args): return sum(args)
来源：http://vhq.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xdc.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://drs.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lce.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cpc.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cbl.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://alc.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oez.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://mnz.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xtr.yanxiufei.cn


<!-- 参考信息 -->