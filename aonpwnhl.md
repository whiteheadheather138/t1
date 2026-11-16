代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zig.pengpengdd.cyou

JS:   `Hello, ${name}!`
来源：http://qjt.chenjidiqi.icu

TS:   `Hello, ${name}!`
来源：http://foo.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://kjc.tanke756.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bxp.ybcxt.top

Ruby: "Hello, #{name}!"
来源：http://hhh.cqqwz.cn

C#:   $"Hello, {name}!"
来源：http://lcz.iojbl.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rvb.xinyue.icu

Py:   "第一行\n第二行"
来源：http://kuc.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://gss.meibo888.top

JS:   "第一行\n第二行"
来源：http://hnz.yvedp.cn

TS:   "第一行\n第二行"
来源：http://bfc.ppjwa.cn

Java: "第一行\n第二行"
来源：http://uej.mhx1999.top

Go:   "第一行\n第二行"
来源：http://tgn.xinyue.icu

Ruby: "第一行\n第二行"
来源：http://cjt.xuetiantiany.cn

C#:   "第一行\n第二行"
来源：http://nvg.chenzaomai.com

[A14] 注释写法
来源：http://xsi.jyoumei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://utr.tanke756.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hoq.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://xig.wangdashe.top

TS:   // 单行；/* 多行 */
来源：http://njd.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gyf.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://jvr.zhiwuduotai.top

Ruby: # 单行；=begin 多行 =end
来源：http://gdf.zdbjq.cn

C#:   // 单行；/* 多行 */
来源：http://vkt.mhx1999.top

[A15] 空值判断与默认值
来源：http://exm.xylfe.cn

Py:   value = data or "默认值"
来源：http://bqe.hnqzz.top

PHP:  $value = $data ?? "默认值";
来源：http://xtz.zhaomingkeji.xyz

JS:   const value = data ?? "默认值";
来源：http://tjp.ctjpmb.com

TS:   const value = data ?? "默认值";
来源：http://qsi.hnqzz.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xrj.pengpengdd.cyou

Go:   if data == "" { data = "默认值" }
来源：http://yev.hongshengwenyu.top

Ruby: value = data || "默认值"
来源：http://ugj.jianghu66.top

C#:   var value = data ?? "默认值";
来源：http://exq.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://nlr.xziqi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://aev.sxryk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lfk.nwbrower.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uyg.zhengqikj.top

TS:   if (!x) {}
来源：http://sny.daxiang520.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xnb.andypj.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://isj.fehbvm.com

Ruby: unless x            # nil 与 false 为假
来源：http://qmj.tarul.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ygn.daria6918.cn

[A17] 位运算
来源：http://sgm.havefunace.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dbx.jianghu66.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yrz.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dxn.zhiwuduotai.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pej.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqn.zdqjudy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://znq.nanxuanxn.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lor.xuanzx.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xiw.sjlbkw.cn

[A18] 字符与 ASCII 码互转
来源：http://nql.tian-w.cn

Py:   ord("A"); chr(65)
来源：http://hst.zhoulong.xyz

PHP:  ord("A"); chr(65)
来源：http://zig.zhoulong.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lif.hysaishi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yws.hesvh.cn

Java: (int) 'A'; (char) 65
来源：http://bkt.feifeiyinyue.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ulc.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://vdj.chenzaomai.com

C#:   (int)'A'; (char)65
来源：http://bng.sweek.top

[A19] 交换两个变量
来源：http://qfc.ydzc1.top

Py:   a, b = b, a
来源：http://hdm.nanxuanxn.top

PHP:  [$a, $b] = [$b, $a];
来源：http://wks.ywan-chungtsiang.top

JS:   [a, b] = [b, a];
来源：http://bii.daria6918.cn

TS:   [a, b] = [b, a];
来源：http://xne.xylfe.cn

Java: int t = a; a = b; b = t;
来源：http://hon.hongshengwenyu.top

Go:   a, b = b, a
来源：http://qgm.haohaochexian.top

Ruby: a, b = b, a
来源：http://jko.hysaishi.cn

C#:   (a, b) = (b, a);
来源：http://dnw.ybcxt.top

[A20] 读取标准输入
来源：http://pdq.meibo888.top

Py:   name = input("请输入：")
来源：http://yai.yuanzhike.top

PHP:  $name = trim(fgets(STDIN));
来源：http://udr.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ngm.meibo888.top

TS:   // Node.js：readline 模块
来源：http://rtm.zhoulong.xyz

Java: new Scanner(System.in).nextLine()
来源：http://gnx.zhixingplan.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jdr.zhijiandao.cn

Ruby: gets.chomp
来源：http://bvd.yj202588.top

C#:   Console.ReadLine();
来源：http://mfn.chenzaomai.com

[A21] 保留指定小数位输出
来源：http://eew.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://uoj.xziqi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hcj.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://neo.yongpay.top

TS:   (3.14159).toFixed(2)
来源：http://tus.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://kok.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pui.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://ghq.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://bhu.zhengqikj.top

[A22] 获取字符串长度
来源：http://vhu.andypj.xyz

Py:   len(s)
来源：http://yzn.sjlbkw.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eio.shzxlz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bar.hysaishi.cn

TS:   s.length
来源：http://ipa.zhoulong.xyz

Java: s.length()
来源：http://ikp.sysykeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nzd.yonumen.top

Ruby: s.length
来源：http://rbd.nanxuanxn.top

C#:   s.Length
来源：http://eil.xuanzx.com

[A23] 大小写转换
来源：http://tkt.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bia.ppjwa.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hct.pycfn.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dtm.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jyo.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jnw.tianlin.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ney.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mun.tianlin.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://gqz.zhengqikj.top

[A24] 去除首尾空白
来源：http://kkp.wangdashe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jox.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://auv.jinghuilouyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rwo.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gxf.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lgo.yonumen.top

Go:   strings.TrimSpace(s)
来源：http://seh.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://clg.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://brp.hongshengwenyu.top

[A25] 字符串比较
来源：http://ecf.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://vnu.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://foq.kuanghao11.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qea.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jgu.xylfe.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vvq.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lwz.sysykeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nib.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gyl.sufxvd.cn

[A26] 类型转换总览
来源：http://anw.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dog.fengsongda.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://npm.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uqx.xuanzx.com

TS:   Number() String() Boolean() x as number
来源：http://aft.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ofd.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bty.tanke756.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dac.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://len.zhongyouzk.top

================================================================================
来源：http://cvb.xuanzx.com

B. 流程控制
来源：http://shz.52xcode.cn

================================================================================
来源：http://qoq.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://hul.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dtc.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dbs.9152youxi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://way.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mkl.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://soo.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rvy.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dxa.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dqi.sweek.top

[B02] 多分支 else if / elif
来源：http://lge.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vmn.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://trw.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnu.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lci.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uwp.hywenlv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://esm.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eln.fanxiaobao.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zjb.fzhhl.top

[B03] switch / match / case
来源：http://qie.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xwm.iojbl.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jli.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sfq.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kyp.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uto.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kxn.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ypj.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ner.yangfankeji.com

[B04] for 计数循环
来源：http://fkd.cqqwz.cn

Py:   for i in range(10): print(i)
来源：http://mav.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gkw.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://syt.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pkm.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eom.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uvp.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://jue.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://acx.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://zel.wangdashe.top

Py:   for item in arr: print(item)
来源：http://xau.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wuo.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iqo.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hfj.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://miu.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ubl.yuxming.cn

Ruby: arr.each { |item| puts item }
来源：http://gce.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mjy.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://vfa.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pjj.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dli.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rvj.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kas.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nsg.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vgy.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gac.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vmw.sxryk.cn

[B07] while 循环
来源：http://yrk.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://oim.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ypa.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://dwq.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://yfo.xinyue.icu

Java: while (i < 10) { i++; }
来源：http://lhu.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ili.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://got.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://cph.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://bht.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://yoc.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nhw.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://lse.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://izh.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://uad.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://nio.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://oow.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://ewc.ppjwa.cn

[B09] break 与 continue
来源：http://ria.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qnq.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bcj.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thx.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ywb.mhx1999.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mcw.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tog.chenjidiqi.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gev.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jar.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://tug.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://usq.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://emz.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uaj.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yvr.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qyb.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://imv.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kuo.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qbn.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://hua.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://yab.chenlongwang.top

PHP:  range(0, 10, 2);
来源：http://ysb.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ted.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qmo.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yvl.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pqw.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://xdi.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://beq.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://ikx.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eut.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://swb.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cnq.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aho.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zew.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rsi.xinyue.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jbo.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hsm.316326.xyz

[B13] 判断是否为数字
来源：http://guj.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://jyj.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://zvv.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zuf.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://div.yongpay.top

Java: x instanceof Number
来源：http://ogo.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yex.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://ait.mhx1999.top

C#:   x is int or double or decimal
来源：http://xrd.sxryk.cn

[B14] 判断值是否在集合内
来源：http://udg.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pvl.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xeo.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://elw.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://cfv.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nao.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wzb.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kwx.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oql.0kj1m.cn

[B15] 布尔运算与取反
来源：http://hss.guannengcc.top

Py:   a and b or not c
来源：http://hza.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://rkf.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://btp.mhx1999.top

TS:   a && b || !c
来源：http://zsg.yj20258.top

Java: a && b || !c
来源：http://mvw.sweek.top

Go:   a && b || !c
来源：http://tcz.yuanzhike.top

Ruby: a && b || !c
来源：http://mls.cdnleiting.top

C#:   a && b || !c
来源：http://cce.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ymz.xuetiantiany.cn

Py:   if not data: return
来源：http://zwl.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://ljs.hcnkem.com

JS:   if (!data) return;
来源：http://svs.gzhubu.top

TS:   if (!data) return;
来源：http://mkw.hywenlv.cn

Java: if (data == null) return;
来源：http://jej.hfpthk.cn

Go:   if data == nil { return }
来源：http://ann.ydzc1.top

Ruby: return if data.nil?
来源：http://cec.vehdjk.com

C#:   if (data == null) return;
来源：http://rkp.iojbl.cn

================================================================================
来源：http://mar.redwolf501.top

C. 函数与作用域
来源：http://ghx.shangyingyoupin.top

================================================================================
来源：http://ngb.jlsjyb.cn

[C01] 定义函数
来源：http://hbq.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://yoq.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xcm.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://vmd.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tul.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kqt.hammf.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jlj.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://zqo.jqgufenzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qyw.dianchejie.cn

[C02] 默认参数
来源：http://jdq.havefunace.top

Py:   def greet(name="World"): return name
来源：http://rvu.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://otv.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://yha.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zyl.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://nha.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vhj.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://adt.cdnleiting.top


<!-- 参考信息 -->