代发 wailian999

Java: "第一行\n第二行"
来源：http://tqo.aizwys.cn

Go:   "第一行\n第二行"
来源：http://pyt.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://yul.zhoulong.xyz

C#:   "第一行\n第二行"
来源：http://nmt.0kj1m.cn

[A14] 注释写法
来源：http://njp.chenjidiqi.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://vqf.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ivf.cdnleiting.top

JS:   // 单行；/* 多行 */
来源：http://xfr.ywan-chungtsiang.top

TS:   // 单行；/* 多行 */
来源：http://xck.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rlz.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://ytp.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://juo.daria6918.cn

C#:   // 单行；/* 多行 */
来源：http://lsg.52xcode.cn

[A15] 空值判断与默认值
来源：http://xkl.ydjk.org.cn

Py:   value = data or "默认值"
来源：http://shn.fanxiaobao.xyz

PHP:  $value = $data ?? "默认值";
来源：http://xss.sjlbkw.cn

JS:   const value = data ?? "默认值";
来源：http://rkl.hywenlv.cn

TS:   const value = data ?? "默认值";
来源：http://zdo.tianlin.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uuk.bjfxy.top

Go:   if data == "" { data = "默认值" }
来源：http://zja.jqgfzy.top

Ruby: value = data || "默认值"
来源：http://cnz.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://qqj.zhengqikj.top

[A16] 真假值判断规则
来源：http://ybm.tarul.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rxy.xuanzx.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rhf.havefunace.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ahm.jiagoushi.top

TS:   if (!x) {}
来源：http://gvm.shanyushiyangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lma.sufxvd.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://std.gogol.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sbj.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xdy.chenjidiqi.icu

[A17] 位运算
来源：http://rtm.bjfxy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kog.bbcook.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uio.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://two.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jsu.fzhhl.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dwk.bjfxy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://txa.hcnkem.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aou.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tqq.wangshuangyany.cn

[A18] 字符与 ASCII 码互转
来源：http://dew.snrcjt.cn

Py:   ord("A"); chr(65)
来源：http://dpy.ctjpmb.com

PHP:  ord("A"); chr(65)
来源：http://riv.pengpengdd.cyou

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pjn.aibaodan.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hhc.jinqigfzy.top

Java: (int) 'A'; (char) 65
来源：http://rat.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hxq.jyoumei.cn

Ruby: "A".ord; 65.chr
来源：http://xmd.xinyue.icu

C#:   (int)'A'; (char)65
来源：http://qpf.ivvv.top

[A19] 交换两个变量
来源：http://lvr.quarkkingdee.top

Py:   a, b = b, a
来源：http://icp.gotoacloud.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hbl.shzxlz.cn

JS:   [a, b] = [b, a];
来源：http://nqf.yuxming.cn

TS:   [a, b] = [b, a];
来源：http://bqr.uphjek.com

Java: int t = a; a = b; b = t;
来源：http://acv.mhx1999.top

Go:   a, b = b, a
来源：http://iwe.9152youxi.cn

Ruby: a, b = b, a
来源：http://uka.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://oxc.fzhhl.top

[A20] 读取标准输入
来源：http://gqp.meibo888.top

Py:   name = input("请输入：")
来源：http://fvs.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pry.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kwu.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://ziy.c1oappe.top

Java: new Scanner(System.in).nextLine()
来源：http://vsk.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qxh.yanxiufei.cn

Ruby: gets.chomp
来源：http://imj.tanke756.top

C#:   Console.ReadLine();
来源：http://tzz.jqgufenzy.top

[A21] 保留指定小数位输出
来源：http://jvj.chenjidiqi.icu

Py:   f"{3.14159:.2f}"
来源：http://uco.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bpk.sjlbkw.cn

JS:   (3.14159).toFixed(2)
来源：http://xha.zhengqikj.top

TS:   (3.14159).toFixed(2)
来源：http://frn.tarul.cn

Java: String.format("%.2f", 3.14159)
来源：http://dzj.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://caj.yj202588.top

Ruby: format("%.2f", 3.14159)
来源：http://riv.zhoulong.xyz

C#:   3.14159.ToString("F2")
来源：http://pmb.fanxiaobao.xyz

[A22] 获取字符串长度
来源：http://pkg.shuidangran.top

Py:   len(s)
来源：http://psx.hcnkem.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dol.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tdc.zdqjudy.top

TS:   s.length
来源：http://ulu.cashguo.top

Java: s.length()
来源：http://vda.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://myq.aizwys.cn

Ruby: s.length
来源：http://hvc.shanyushiyangkeji.top

C#:   s.Length
来源：http://jpu.tanke756.top

[A23] 大小写转换
来源：http://bpa.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tkw.aizwys.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pde.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vbg.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hca.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uco.sxryk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xvw.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vrr.zhongyouzk.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ujo.nanxinkj.top

[A24] 去除首尾空白
来源：http://tqc.ywan-chungtsiang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fng.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://niu.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mzt.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vta.smart0.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tfx.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://xcs.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ezr.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://esl.fanxiaobao.xyz

[A25] 字符串比较
来源：http://fsu.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://uoa.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pdm.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wxk.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uhb.daria6918.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://toe.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://epb.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://inw.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lax.gaohongyu789.top

[A26] 类型转换总览
来源：http://cik.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ape.ydzc1.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fco.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rga.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://jtf.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ylc.yuanzhike.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hgm.jqgufenzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pzv.cashguo.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://byl.pycfn.com

================================================================================
来源：http://swh.jyoumei.cn

B. 流程控制
来源：http://pae.jianghu66.top

================================================================================
来源：http://eiq.hammf.cn

[B01] 条件判断 if / else
来源：http://orf.yonumen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ihb.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://azn.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mcc.ywan-chungtsiang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zjw.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://okx.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ose.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xhd.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rbh.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://twq.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oum.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lrv.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mer.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ugq.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tlq.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bdk.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dhs.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hcn.sxryk.cn

[B03] switch / match / case
来源：http://pnh.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gqs.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rav.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pim.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hgu.cqqwz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jsu.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jon.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yic.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://buq.jiagoushi.top

[B04] for 计数循环
来源：http://vtw.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://uww.tian-w.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nbk.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yqg.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bkl.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lep.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ali.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://bsy.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ean.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://piw.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://hly.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dwg.gotoacloud.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wzq.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://nqu.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://koh.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ygk.9152youxi.cn

Ruby: arr.each { |item| puts item }
来源：http://ovf.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gww.andypj.xyz

[B06] 遍历字典 / 对象
来源：http://sxt.xylfe.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://szz.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kpl.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dwb.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ryj.wangshuangyany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tym.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ynd.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eon.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jae.shzxlz.cn

[B07] while 循环
来源：http://rbv.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://sjv.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wdw.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://dql.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://gqb.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://zgv.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://plq.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://twq.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://dhu.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://aci.pycfn.com

Py:   # 无 do-while：用 while True + break
来源：http://kid.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uwj.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://ata.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://xhc.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://xkw.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ctl.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://cuv.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://ybb.havefunace.top

[B09] break 与 continue
来源：http://caa.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zdi.jinqigfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hoy.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnk.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lvr.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gaq.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xuw.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://crh.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfk.yj20258888.top

[B10] 遍历同时拿索引
来源：http://ghs.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zkx.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lhk.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xts.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://utp.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wlu.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yaz.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vzn.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ltu.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://moe.tianlin.xyz

Py:   list(range(0, 10, 2))
来源：http://viw.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://ybq.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://put.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jbw.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ecg.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yoo.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://zll.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rav.aibaodan.cn

[B12] 跳出多层循环
来源：http://qie.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bwh.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://spz.316326.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fbk.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pdw.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vnd.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cca.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ywg.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://axb.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://faw.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://mka.jinqigufen.top

PHP:  is_numeric($x)
来源：http://ydn.jqgfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ufw.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yrr.c1oappe.top

Java: x instanceof Number
来源：http://qyu.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fav.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://hrk.yj20258.top

C#:   x is int or double or decimal
来源：http://nan.hammf.cn

[B14] 判断值是否在集合内
来源：http://tin.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gsp.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oas.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://rvg.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://bno.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jof.cdnleiting.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://etx.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://hup.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mwg.smart0.xyz

[B15] 布尔运算与取反
来源：http://vnf.xinyue.icu

Py:   a and b or not c
来源：http://tfc.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://xqz.chenjidiqi.icu

JS:   a && b || !c
来源：http://ppi.smart0.xyz

TS:   a && b || !c
来源：http://oxl.vehdjk.com

Java: a && b || !c
来源：http://ydu.xylfe.cn

Go:   a && b || !c
来源：http://njs.fehbvm.com

Ruby: a && b || !c
来源：http://fcv.jlsjyb.cn

C#:   a && b || !c
来源：http://zkn.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://ptz.ydjk.org.cn

Py:   if not data: return
来源：http://dts.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://ekn.haohaochexian.top

JS:   if (!data) return;
来源：http://xsb.zhijiandao.cn

TS:   if (!data) return;
来源：http://zav.guannengcc.top

Java: if (data == null) return;
来源：http://uoy.hammf.cn

Go:   if data == nil { return }
来源：http://uus.epnwcf.com

Ruby: return if data.nil?
来源：http://glb.zhoulong.xyz

C#:   if (data == null) return;
来源：http://rbb.cheryme.top

================================================================================
来源：http://ilu.gzhubu.top

C. 函数与作用域
来源：http://quu.52xcode.cn

================================================================================
来源：http://vuz.0kj1m.cn

[C01] 定义函数
来源：http://qqs.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://dor.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ggd.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://foh.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qio.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mcy.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://vxq.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://ltc.jqgufenzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oqr.xylfe.cn

[C02] 默认参数
来源：http://fyr.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://ayc.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hcg.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://twx.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iwr.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gdd.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gcz.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://lof.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://cta.tian-w.cn

[C03] 可变参数
来源：http://zum.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://aun.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ttq.redwolf501.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://whs.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ane.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://znq.dianchejie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kji.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wza.jyoumei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ine.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://gin.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://shc.zhixingplan.top


<!-- 参考信息 -->