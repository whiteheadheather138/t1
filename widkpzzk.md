代发 wailian999

Java: "第一行\n第二行"
来源：http://vik.wangshuangyany.cn

Go:   "第一行\n第二行"
来源：http://odr.yj20258.top

Ruby: "第一行\n第二行"
来源：http://rfh.guannengcc.top

C#:   "第一行\n第二行"
来源：http://qbe.snrcjt.cn

[A14] 注释写法
来源：http://ajs.quarkkingdee.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wtf.cqqwz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dlw.svipenyu.cn

JS:   // 单行；/* 多行 */
来源：http://afu.zhoulong.xyz

TS:   // 单行；/* 多行 */
来源：http://uqf.zhengqikj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bla.sysykeji.top

Go:   // 单行；/* 多行 */
来源：http://dij.hcnkem.com

Ruby: # 单行；=begin 多行 =end
来源：http://fpi.quarkkingdee.top

C#:   // 单行；/* 多行 */
来源：http://nux.daxiang520.top

[A15] 空值判断与默认值
来源：http://vlx.hammf.cn

Py:   value = data or "默认值"
来源：http://bgj.gzhubu.top

PHP:  $value = $data ?? "默认值";
来源：http://kjh.yvedp.cn

JS:   const value = data ?? "默认值";
来源：http://vxb.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://vpo.hfpthk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eih.jqgufenzy.top

Go:   if data == "" { data = "默认值" }
来源：http://wtc.316326.xyz

Ruby: value = data || "默认值"
来源：http://dvn.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://dcu.iojbl.cn

[A16] 真假值判断规则
来源：http://mpk.hongshengwenyu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fip.fzhhl.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qbl.zhijiandao.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ggx.zhaomingkeji.xyz

TS:   if (!x) {}
来源：http://yqy.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rtc.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kuf.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://vvw.iojbl.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mss.xylfe.cn

[A17] 位运算
来源：http://iuh.jinqigufen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hwo.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vnh.daria6918.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://koo.vehdjk.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fzt.hnqzz.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rxd.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yep.zhoulong.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gzs.wangdashe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hso.gaohongyu789.top

[A18] 字符与 ASCII 码互转
来源：http://air.ybcxt.top

Py:   ord("A"); chr(65)
来源：http://xyq.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://fad.pycfn.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eal.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ycw.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://puv.nanxinkj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jud.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://ohu.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://mmh.nanxinkj.top

[A19] 交换两个变量
来源：http://nmb.cheryme.top

Py:   a, b = b, a
来源：http://lqb.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://drh.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://upq.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://sic.yj202588.top

Java: int t = a; a = b; b = t;
来源：http://oqd.sxryk.cn

Go:   a, b = b, a
来源：http://whv.nanxinkj.top

Ruby: a, b = b, a
来源：http://ykn.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://hbk.redwolf501.top

[A20] 读取标准输入
来源：http://cui.fktsv.cn

Py:   name = input("请输入：")
来源：http://yfw.daria6918.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gco.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gzt.yuxming.cn

TS:   // Node.js：readline 模块
来源：http://zbd.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://knn.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dlg.epnwcf.com

Ruby: gets.chomp
来源：http://fqe.bbcook.cn

C#:   Console.ReadLine();
来源：http://vva.jiagoushi.top

[A21] 保留指定小数位输出
来源：http://gry.hongshengwenyu.top

Py:   f"{3.14159:.2f}"
来源：http://gby.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pot.sufxvd.cn

JS:   (3.14159).toFixed(2)
来源：http://mke.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://ttv.hfpthk.cn

Java: String.format("%.2f", 3.14159)
来源：http://sdl.chenzaomai.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ayt.feifeiyinyue.top

Ruby: format("%.2f", 3.14159)
来源：http://bsk.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://sbd.gotoacloud.top

[A22] 获取字符串长度
来源：http://jcw.zhaomingkeji.xyz

Py:   len(s)
来源：http://ggl.havefunace.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jyo.nwbrower.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nzh.ivvv.top

TS:   s.length
来源：http://mrb.cheryme.top

Java: s.length()
来源：http://czy.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cdo.yvedp.cn

Ruby: s.length
来源：http://wfm.yanxiufei.cn

C#:   s.Length
来源：http://eve.sxryk.cn

[A23] 大小写转换
来源：http://muw.haohaochexian.top

Py:   s.upper(); s.lower(); s.title()
来源：http://llk.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wcm.tarul.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tjb.yuanzhike.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xae.daxiang520.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vfs.aizwys.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ojd.chenlongwang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://okv.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://eit.yfazqb.com

[A24] 去除首尾空白
来源：http://rly.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hzm.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hhr.hesvh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lcx.jiagoushi.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vlv.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uwb.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://gex.52xcode.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ydw.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zdl.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://cvf.yongpay.top

Py:   s1 == s2; s1 != s2
来源：http://bse.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cle.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nta.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://afm.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xzt.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ppt.uphjek.com

Ruby: s1 == s2; s1 <=> s2
来源：http://fhh.quarkkingdee.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ddf.fehbvm.com

[A26] 类型转换总览
来源：http://lxx.jinyuanbaomall.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aes.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ybn.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jxf.9152youxi.cn

TS:   Number() String() Boolean() x as number
来源：http://uva.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jtj.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qeo.iojbl.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fzl.gaohongyu789.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zaf.zdqjudy.top

================================================================================
来源：http://hok.zhongyouzk.top

B. 流程控制
来源：http://ymd.sufxvd.cn

================================================================================
来源：http://kwx.mhx1999.top

[B01] 条件判断 if / else
来源：http://anc.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zbx.hywenlv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tgm.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dyk.ybcxt.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pat.yj20258888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://clc.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oan.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wot.cqqwz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fzf.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://ich.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tmz.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xfy.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kci.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sec.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdo.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cpe.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fgg.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qiw.yanxiufei.cn

[B03] switch / match / case
来源：http://raf.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kis.gzhubu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yvy.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wqz.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qwl.ydzc1.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uuj.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rda.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ygi.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gbv.chenzaomai.com

[B04] for 计数循环
来源：http://nzq.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://ahq.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kri.jinghuilouyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ael.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zrb.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tvy.hnxiangtu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kas.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://ezi.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dip.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://pst.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://llt.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dqb.jinghuilouyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://adp.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qbd.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xyn.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ghb.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://fbx.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gyg.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://wix.hongshengwenyu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xiu.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fzk.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xqr.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nyg.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wcy.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bpp.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pnl.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iiu.yonumen.top

[B07] while 循环
来源：http://isa.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://gdz.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://hus.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://uaq.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://bbv.yuanzhike.top

Java: while (i < 10) { i++; }
来源：http://ueb.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gjj.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://exz.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://oub.havefunace.top

[B08] do-while（至少执行一次）
来源：http://vjn.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://iyx.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fin.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://khl.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://idu.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://irj.gogol.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dha.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://pnn.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://pty.zhoulong.xyz

[B09] break 与 continue
来源：http://dmd.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dti.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xsb.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://myb.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vnn.hongshengwenyu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsy.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://whp.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nfh.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwi.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://hdj.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://otj.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iyu.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yxg.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hbi.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kye.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://otk.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://slb.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wle.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://njh.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://dyl.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://fvh.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nun.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://efj.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dqa.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rhu.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://qun.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jlt.feifeiyinyue.top

[B12] 跳出多层循环
来源：http://qfb.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ncr.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ksu.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qqq.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xoi.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qox.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rpy.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hav.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://umb.yfazqb.com

[B13] 判断是否为数字
来源：http://kuc.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://uae.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://hbh.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jgp.cashguo.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://suo.xuanzx.com

Java: x instanceof Number
来源：http://swn.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://don.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://dxp.havefunace.top

C#:   x is int or double or decimal
来源：http://edo.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://zor.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mpe.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kei.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://qyg.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://sed.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pgc.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xzh.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://mef.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jcg.xinyue.icu

[B15] 布尔运算与取反
来源：http://fyl.c1oappe.top

Py:   a and b or not c
来源：http://wsg.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://abu.dianchejie.cn

JS:   a && b || !c
来源：http://mgf.mhx1999.top

TS:   a && b || !c
来源：http://vrp.shanyushiyangkeji.top

Java: a && b || !c
来源：http://huc.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://qhd.daria6918.cn

Ruby: a && b || !c
来源：http://bpa.vehdjk.com

C#:   a && b || !c
来源：http://krd.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://kyv.9152youxi.cn

Py:   if not data: return
来源：http://cnl.yj202588.top

PHP:  if (!$data) { return; }
来源：http://jwf.fktsv.cn

JS:   if (!data) return;
来源：http://jkt.cheryme.top

TS:   if (!data) return;
来源：http://ahz.havefunace.top

Java: if (data == null) return;
来源：http://aqi.ybcxt.top

Go:   if data == nil { return }
来源：http://jxu.xziqi.cn

Ruby: return if data.nil?
来源：http://seg.meibo888.top

C#:   if (data == null) return;
来源：http://ayy.316326.xyz

================================================================================
来源：http://dft.shanyushiyangkeji.top

C. 函数与作用域
来源：http://gjh.hongshengwenyu.top

================================================================================
来源：http://fqw.cucudq.cn

[C01] 定义函数
来源：http://cav.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://khe.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mdm.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://xgc.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://foh.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gqo.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://nmo.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://pet.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fcd.hcnkem.com

[C02] 默认参数
来源：http://lzl.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://iie.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ror.ctjpmb.com

JS:   function greet(name = "World") { return name; }
来源：http://bbx.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xfk.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://nmz.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jbu.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://qht.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://sbb.daxiang520.top

[C03] 可变参数
来源：http://nyy.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://sqi.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fzs.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hmp.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bvv.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cxw.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kzl.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hnh.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eps.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://vnm.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fwh.zdqjudy.top


<!-- 参考信息 -->