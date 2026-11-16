代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jve.yuanzhike.top

Ruby: "Hello, #{name}!"
来源：http://gxn.yuxming.cn

C#:   $"Hello, {name}!"
来源：http://mkc.cdnleiting.top

[A13] 多行字符串（练习 \n 转义）
来源：http://chn.yuanzhike.top

Py:   "第一行\n第二行"
来源：http://peu.hongshengwenyu.top

PHP:  "第一行\n第二行"
来源：http://myu.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://ahl.wangdashe.top

TS:   "第一行\n第二行"
来源：http://itv.jiagoushi.top

Java: "第一行\n第二行"
来源：http://vcq.tianlin.xyz

Go:   "第一行\n第二行"
来源：http://lsh.hammf.cn

Ruby: "第一行\n第二行"
来源：http://mpw.xuetiantiany.cn

C#:   "第一行\n第二行"
来源：http://yrq.bjfxy.top

[A14] 注释写法
来源：http://hut.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vih.jqgfzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cwb.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://lij.jqgufenzy.top

TS:   // 单行；/* 多行 */
来源：http://wth.zhongyouzk.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://moq.nwbrower.top

Go:   // 单行；/* 多行 */
来源：http://kbf.xingfuxueyuan.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://dyo.jinqigfzy.top

C#:   // 单行；/* 多行 */
来源：http://urk.vehdjk.com

[A15] 空值判断与默认值
来源：http://evn.daria6918.cn

Py:   value = data or "默认值"
来源：http://eam.gaohongyu789.top

PHP:  $value = $data ?? "默认值";
来源：http://ohh.jianghu66.top

JS:   const value = data ?? "默认值";
来源：http://ylq.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://ndr.hesvh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://row.zycfv.cn

Go:   if data == "" { data = "默认值" }
来源：http://ezl.hesvh.cn

Ruby: value = data || "默认值"
来源：http://aek.ybcxt.top

C#:   var value = data ?? "默认值";
来源：http://dzr.vqdsnc.cn

[A16] 真假值判断规则
来源：http://gys.jinqigfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uzh.feifeiyinyue.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cab.xuetiantiany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://urt.guannengcc.top

TS:   if (!x) {}
来源：http://czs.cashguo.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ang.smart0.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wwg.gzhubu.top

Ruby: unless x            # nil 与 false 为假
来源：http://frw.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://scv.jyoumei.cn

[A17] 位运算
来源：http://ciz.chenzaomai.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bnf.ivvv.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wol.xingfuxueyuan.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dlc.epnwcf.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ycv.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jdq.vehdjk.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://leq.cashguo.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eno.zhongyouzk.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eyj.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://our.quarkkingdee.top

Py:   ord("A"); chr(65)
来源：http://iwz.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://iir.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://buz.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qlu.havefunace.top

Java: (int) 'A'; (char) 65
来源：http://qvl.zhoulong.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://icl.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://hdt.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://yuh.daxiang520.top

[A19] 交换两个变量
来源：http://lgx.zhixingplan.top

Py:   a, b = b, a
来源：http://xjr.fanxiaobao.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://tsr.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://gii.sysykeji.top

TS:   [a, b] = [b, a];
来源：http://fkx.yuxming.cn

Java: int t = a; a = b; b = t;
来源：http://hqa.daxiang520.top

Go:   a, b = b, a
来源：http://nze.chenzaomai.com

Ruby: a, b = b, a
来源：http://jkv.smart0.xyz

C#:   (a, b) = (b, a);
来源：http://efs.yfazqb.com

[A20] 读取标准输入
来源：http://tji.ydzc1.top

Py:   name = input("请输入：")
来源：http://tut.ehwqpu.com

PHP:  $name = trim(fgets(STDIN));
来源：http://uco.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lmg.vqdsnc.cn

TS:   // Node.js：readline 模块
来源：http://ncy.smart0.xyz

Java: new Scanner(System.in).nextLine()
来源：http://mss.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lcj.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://zwz.sysykeji.top

C#:   Console.ReadLine();
来源：http://lfx.quarkkingdee.top

[A21] 保留指定小数位输出
来源：http://ksv.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://eqe.cdnleiting.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gll.sufxvd.cn

JS:   (3.14159).toFixed(2)
来源：http://smk.jinyuanbaomall.cn

TS:   (3.14159).toFixed(2)
来源：http://ukt.fanxiaobao.xyz

Java: String.format("%.2f", 3.14159)
来源：http://eif.yuxming.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ceq.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://ofq.xinyue.icu

C#:   3.14159.ToString("F2")
来源：http://vqp.zdbjq.cn

[A22] 获取字符串长度
来源：http://cry.hnqzz.top

Py:   len(s)
来源：http://thy.yuxming.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ieu.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://czv.snrcjt.cn

TS:   s.length
来源：http://mzm.gotoacloud.top

Java: s.length()
来源：http://inh.tarul.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gbl.yonumen.top

Ruby: s.length
来源：http://pde.hywenlv.cn

C#:   s.Length
来源：http://pce.zhijiandao.cn

[A23] 大小写转换
来源：http://vtq.sxryk.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ois.havefunace.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yrj.kuanghao11.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uve.birdmap.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tyu.xziqi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rvd.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rsw.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kqt.jlsjyb.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rms.aibaodan.cn

[A24] 去除首尾空白
来源：http://ymf.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mry.zdbjq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ozt.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://onw.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yxa.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eze.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://cxw.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hno.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gyy.fktsv.cn

[A25] 字符串比较
来源：http://awo.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://gox.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vvn.uphjek.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zgi.ydzc1.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ylo.yanxiufei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://czf.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://veb.gaohongyu789.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tdj.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fcu.quarkkingdee.top

[A26] 类型转换总览
来源：http://sdh.gaohongyu789.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hzu.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xoi.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mdy.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://nrn.yj202588.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fpw.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yiv.316326.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://qgc.kuanghao11.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yhc.tian-w.cn

================================================================================
来源：http://bcd.chenzaomai.com

B. 流程控制
来源：http://tog.guowangkeji.top

================================================================================
来源：http://fhd.yj20258.top

[B01] 条件判断 if / else
来源：http://kgu.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://itl.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dzl.fzhhl.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rsc.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jrq.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uvn.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://abq.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wqq.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zbs.yj20258.top

[B02] 多分支 else if / elif
来源：http://zjp.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tir.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dkp.redwolf501.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nlw.redwolf501.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wpt.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrk.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qly.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ezf.zhongyouzk.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgp.9152youxi.cn

[B03] switch / match / case
来源：http://uvk.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bmj.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bxk.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iac.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ueb.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zcf.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://otv.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ytk.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wkn.cheryme.top

[B04] for 计数循环
来源：http://lze.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://bzn.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qpp.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pjp.haohaochexian.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qjt.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wtj.9152youxi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qkq.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://mnr.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kag.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://drt.kuanghao11.cn

Py:   for item in arr: print(item)
来源：http://oqe.chenjidiqi.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dep.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qis.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bkm.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://dmq.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gan.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://imj.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://miw.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://sug.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dap.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pjf.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qow.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gow.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jan.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ppu.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wfe.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rpv.yuxming.cn

[B07] while 循环
来源：http://mxa.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://ysy.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ruq.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://stg.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://xhx.nwbrower.top

Java: while (i < 10) { i++; }
来源：http://cgb.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yvt.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://fjm.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://yxg.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://ntx.sysykeji.top

Py:   # 无 do-while：用 while True + break
来源：http://jnq.yvedp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gvh.nwbrower.top

JS:   do { i++; } while (i < 10);
来源：http://nqi.hnqzz.top

TS:   do { i++; } while (i < 10);
来源：http://pqh.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://iwm.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rjm.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://obo.birdmap.top

C#:   do { i++; } while (i < 10);
来源：http://wzc.meibo888.top

[B09] break 与 continue
来源：http://jch.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mty.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lgz.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ssd.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayn.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eyu.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mkx.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zjl.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bab.yongpay.top

[B10] 遍历同时拿索引
来源：http://sqw.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yet.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iue.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pay.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vjd.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ddi.jianghu66.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mbp.nanxinkj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iki.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iiv.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://lmg.fzhhl.top

Py:   list(range(0, 10, 2))
来源：http://fja.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://jjq.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bbb.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sxi.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kto.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kvo.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://zww.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ayr.316326.xyz

[B12] 跳出多层循环
来源：http://cvl.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uhi.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yuj.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nwu.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://quh.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iqn.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nzj.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vlv.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://deb.andypj.xyz

[B13] 判断是否为数字
来源：http://uvo.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://bdx.yongpay.top

PHP:  is_numeric($x)
来源：http://smj.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://axj.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xdx.nwbrower.top

Java: x instanceof Number
来源：http://fre.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nvz.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://vkv.pycfn.com

C#:   x is int or double or decimal
来源：http://auy.wangdashe.top

[B14] 判断值是否在集合内
来源：http://upm.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kno.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jay.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://nip.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://uhm.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lej.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iuu.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://wri.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xlg.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://gik.gotoacloud.top

Py:   a and b or not c
来源：http://opy.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://lun.zycfv.cn

JS:   a && b || !c
来源：http://xpd.yj20258888.top

TS:   a && b || !c
来源：http://qem.chenzaomai.com

Java: a && b || !c
来源：http://fyj.dashuyun.cn

Go:   a && b || !c
来源：http://czl.nanxinkj.top

Ruby: a && b || !c
来源：http://bjy.sjlbkw.cn

C#:   a && b || !c
来源：http://izl.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://txo.cdnleiting.top

Py:   if not data: return
来源：http://wks.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://avt.epnwcf.com

JS:   if (!data) return;
来源：http://yhj.sxryk.cn

TS:   if (!data) return;
来源：http://zql.hnxiangtu.top

Java: if (data == null) return;
来源：http://eij.yj202588.top

Go:   if data == nil { return }
来源：http://puz.jqgfzy.top

Ruby: return if data.nil?
来源：http://duc.9152youxi.cn

C#:   if (data == null) return;
来源：http://bjx.xylfe.cn

================================================================================
来源：http://sqa.hcnkem.com

C. 函数与作用域
来源：http://fqn.tianlin.xyz

================================================================================
来源：http://ajg.jiagoushi.top

[C01] 定义函数
来源：http://ref.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://mfw.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mzz.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://zwj.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://num.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rvb.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://bgv.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://xcc.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mdi.316326.xyz

[C02] 默认参数
来源：http://xti.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://pbp.daxiang520.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qef.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://rmi.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xkm.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pyq.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kdq.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://nly.iojbl.cn

C#:   string Greet(string name = "World") => name;
来源：http://uon.xinyue.icu

[C03] 可变参数
来源：http://rge.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://fgg.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://chm.xingfuxueyuan.xyz


<!-- 参考信息 -->