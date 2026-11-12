代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://ysk.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://hct.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://zyo.xziqi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eck.quarkkingdee.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jod.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://bdx.yongpay.top

TS:   `Hello, ${name}!`
来源：http://gzq.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://gco.jlsjyb.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rgi.feifeiyinyue.top

Ruby: "Hello, #{name}!"
来源：http://tcm.jinqigufen.top

C#:   $"Hello, {name}!"
来源：http://jyo.tarul.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lrj.pycfn.com

Py:   "第一行\n第二行"
来源：http://dgk.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://vhj.dashuyun.cn

JS:   "第一行\n第二行"
来源：http://eer.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://lcj.hysaishi.cn

Java: "第一行\n第二行"
来源：http://erl.zhiwuduotai.top

Go:   "第一行\n第二行"
来源：http://yyc.tarul.cn

Ruby: "第一行\n第二行"
来源：http://ncd.hammf.cn

C#:   "第一行\n第二行"
来源：http://rmm.shangyingyoupin.top

[A14] 注释写法
来源：http://jnj.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://amg.cheryme.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cap.epnwcf.com

JS:   // 单行；/* 多行 */
来源：http://esh.jqgufenzy.top

TS:   // 单行；/* 多行 */
来源：http://sgi.chenjidiqi.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rnh.yonumen.top

Go:   // 单行；/* 多行 */
来源：http://klr.shanyushiyangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://ceb.jinghuilouyu.cn

C#:   // 单行；/* 多行 */
来源：http://hcc.zhoulong.xyz

[A15] 空值判断与默认值
来源：http://wak.ctjpmb.com

Py:   value = data or "默认值"
来源：http://rgl.chenjidiqi.icu

PHP:  $value = $data ?? "默认值";
来源：http://mjz.epnwcf.com

JS:   const value = data ?? "默认值";
来源：http://vtw.yonumen.top

TS:   const value = data ?? "默认值";
来源：http://jsl.hammf.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wod.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://vof.ivvv.top

Ruby: value = data || "默认值"
来源：http://uyd.yueranfly.top

C#:   var value = data ?? "默认值";
来源：http://jfz.jianghu66.top

[A16] 真假值判断规则
来源：http://rxh.ydzc1.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pzx.yj20258888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jni.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tfz.haohaochexian.top

TS:   if (!x) {}
来源：http://vmq.hongshengwenyu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pqo.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mnz.yongpay.top

Ruby: unless x            # nil 与 false 为假
来源：http://iup.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nje.jinqigfzy.top

[A17] 位运算
来源：http://nyg.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zas.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fct.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oqx.jiagoushi.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://akb.jinqigfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssv.jiagoushi.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://naq.jyoumei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcz.gotoacloud.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uhv.mhx1999.top

[A18] 字符与 ASCII 码互转
来源：http://bis.wangdashe.top

Py:   ord("A"); chr(65)
来源：http://rap.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://ufe.shzxlz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fzq.zdqjudy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://odj.gaohongyu789.top

Java: (int) 'A'; (char) 65
来源：http://vyt.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mbf.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://ccp.yongpay.top

C#:   (int)'A'; (char)65
来源：http://tyy.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://dqa.aibaodan.cn

Py:   a, b = b, a
来源：http://jnt.wangshuangyany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wlu.jinqigfzy.top

JS:   [a, b] = [b, a];
来源：http://ccu.shzxlz.cn

TS:   [a, b] = [b, a];
来源：http://hhv.chenjidiqi.icu

Java: int t = a; a = b; b = t;
来源：http://ubp.xinyue.icu

Go:   a, b = b, a
来源：http://euw.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://hvr.hysaishi.cn

C#:   (a, b) = (b, a);
来源：http://acz.hesvh.cn

[A20] 读取标准输入
来源：http://tmk.birdmap.top

Py:   name = input("请输入：")
来源：http://mjp.hfpthk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://onl.redwolf501.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ncv.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://oea.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://yvz.hfpthk.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ndi.chenlongwang.top

Ruby: gets.chomp
来源：http://hty.jinqigufen.top

C#:   Console.ReadLine();
来源：http://uem.mhx1999.top

[A21] 保留指定小数位输出
来源：http://ajq.hnqzz.top

Py:   f"{3.14159:.2f}"
来源：http://lhq.andypj.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qdz.ydzc1.top

JS:   (3.14159).toFixed(2)
来源：http://zfs.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://qkm.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://djo.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sqs.aibaodan.cn

Ruby: format("%.2f", 3.14159)
来源：http://byc.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://ixl.cqqwz.cn

[A22] 获取字符串长度
来源：http://yer.gotoacloud.top

Py:   len(s)
来源：http://ami.jinqigufen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bqe.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vgq.havefunace.top

TS:   s.length
来源：http://wnn.jlsjyb.cn

Java: s.length()
来源：http://rpg.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pax.jinyuanbaomall.cn

Ruby: s.length
来源：http://osb.jinqigufen.top

C#:   s.Length
来源：http://joa.chenlongwang.top

[A23] 大小写转换
来源：http://lsl.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tkg.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xqc.yongpay.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dmw.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nae.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tmp.kuanghao11.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sil.zhongyouzk.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://exl.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://atx.jyoumei.cn

[A24] 去除首尾空白
来源：http://kie.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gmy.c1oappe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xdj.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lur.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://trh.tian-w.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eyi.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://muy.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ggx.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bwr.daria6918.cn

[A25] 字符串比较
来源：http://slq.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://gtd.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gri.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xtp.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://beh.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ghh.havefunace.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yka.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ffb.jyoumei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mtz.gaohongyu789.top

[A26] 类型转换总览
来源：http://xwc.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rgd.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mom.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lbl.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://rze.zhoulong.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hkm.cucudq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kxr.shanyushiyangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qxa.hywenlv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://drn.gogol.net.cn

================================================================================
来源：http://fyx.sufxvd.cn

B. 流程控制
来源：http://krh.ivvv.top

================================================================================
来源：http://quv.hongshengwenyu.top

[B01] 条件判断 if / else
来源：http://sou.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zjy.zdbjq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aql.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qto.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tsr.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cuk.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jkp.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vhm.bjfxy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iin.52xcode.cn

[B02] 多分支 else if / elif
来源：http://fyw.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iqm.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hnm.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkp.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yjx.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnp.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bvk.jqgfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xmb.meibo888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bpb.smart0.xyz

[B03] switch / match / case
来源：http://dfo.hysaishi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wvq.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jyu.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tux.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tzr.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wzk.jinqigufen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qnv.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wbk.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mpq.bbcook.cn

[B04] for 计数循环
来源：http://fhm.fktsv.cn

Py:   for i in range(10): print(i)
来源：http://sgm.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ogx.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pjv.sjlbkw.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qqm.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zss.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ajt.iojbl.cn

Ruby: 10.times { |i| puts i }
来源：http://pdj.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fan.cashguo.top

[B05] 遍历数组 / 列表
来源：http://eoh.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://qjb.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ftq.hnqzz.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dnr.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kyh.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mly.yvedp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dty.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://tos.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jea.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://kqz.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lbt.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://phk.sxryk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oqx.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wzj.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zsm.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nmt.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qvk.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vzu.shuidangran.top

[B07] while 循环
来源：http://dft.hesvh.cn

Py:   while i < 10: i += 1
来源：http://zkr.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xqm.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://wms.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://nft.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://ipx.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ffp.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://bqi.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://zci.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://swe.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://aft.wangdashe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zbt.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://ewc.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://qge.gaohongyu789.top

Java: do { i++; } while (i < 10);
来源：http://ged.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vva.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ojq.xingfuxueyuan.xyz

C#:   do { i++; } while (i < 10);
来源：http://smz.andypj.xyz

[B09] break 与 continue
来源：http://ydz.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vkt.zhaomingkeji.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sqp.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npx.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzg.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ijt.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tgt.zhongyouzk.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qwx.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvb.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://ouk.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ivb.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tsi.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jzq.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hby.zhoulong.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dem.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eoj.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zkc.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ton.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://jaq.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://mle.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://vvg.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://afn.gotoacloud.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vwd.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vhn.9152youxi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sol.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://tvy.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pxa.haohaochexian.top

[B12] 跳出多层循环
来源：http://urz.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nkl.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xcb.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cvc.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lvi.feifeiyinyue.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rqw.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rdb.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uzg.hywenlv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aoj.fktsv.cn

[B13] 判断是否为数字
来源：http://ltv.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://fvx.cdnleiting.top

PHP:  is_numeric($x)
来源：http://plc.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avw.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cxj.hammf.cn

Java: x instanceof Number
来源：http://tvv.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vst.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://ybt.hfpthk.cn

C#:   x is int or double or decimal
来源：http://ivi.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://uuf.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bgk.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nfl.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://nnq.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://qnz.shzxlz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xwj.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://laj.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rsw.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ehp.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://nop.tianlin.xyz

Py:   a and b or not c
来源：http://ucn.sweek.top

PHP:  $a && $b || !$c
来源：http://odw.yvedp.cn

JS:   a && b || !c
来源：http://ngf.havefunace.top

TS:   a && b || !c
来源：http://kba.iojbl.cn

Java: a && b || !c
来源：http://apo.52xcode.cn

Go:   a && b || !c
来源：http://uwz.fzhhl.top

Ruby: a && b || !c
来源：http://kaz.yangfankeji.com

C#:   a && b || !c
来源：http://vrl.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ilk.jinyuanbaomall.cn

Py:   if not data: return
来源：http://iwp.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://gte.yuxming.cn

JS:   if (!data) return;
来源：http://nqj.haohaochexian.top

TS:   if (!data) return;
来源：http://bzn.andypj.xyz

Java: if (data == null) return;
来源：http://xao.jlsjyb.cn

Go:   if data == nil { return }
来源：http://dnx.aibaodan.cn

Ruby: return if data.nil?
来源：http://ceh.gaohongyu789.top

C#:   if (data == null) return;
来源：http://glv.hfpthk.cn

================================================================================
来源：http://ufg.shanyushiyangtech.top

C. 函数与作用域
来源：http://een.xziqi.cn

================================================================================
来源：http://xqn.ctjpmb.com

[C01] 定义函数
来源：http://qzn.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://mvz.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ikc.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://xrb.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fdt.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fsg.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://api.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://jef.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zxi.jqgufenzy.top

[C02] 默认参数
来源：http://dby.sweek.top

Py:   def greet(name="World"): return name
来源：http://mgu.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cbl.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://grc.gotoacloud.top


<!-- 参考信息 -->