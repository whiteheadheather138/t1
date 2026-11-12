代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://orb.daria6918.cn

JS:   `Hello, ${name}!`
来源：http://get.nanxuanxn.top

TS:   `Hello, ${name}!`
来源：http://mhp.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://ylf.bbcook.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xjd.guowangkeji.top

Ruby: "Hello, #{name}!"
来源：http://oxi.jqgfzy.top

C#:   $"Hello, {name}!"
来源：http://rgb.redwolf501.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qxm.vehdjk.com

Py:   "第一行\n第二行"
来源：http://wiz.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://fpv.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://mqn.zdbjq.cn

TS:   "第一行\n第二行"
来源：http://jir.svipenyu.cn

Java: "第一行\n第二行"
来源：http://jvd.ydjk.org.cn

Go:   "第一行\n第二行"
来源：http://fma.fktsv.cn

Ruby: "第一行\n第二行"
来源：http://fwl.fzhhl.top

C#:   "第一行\n第二行"
来源：http://pmi.xuanzx.com

[A14] 注释写法
来源：http://zba.zhijiandao.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://urg.vqdsnc.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lqp.c1oappe.top

JS:   // 单行；/* 多行 */
来源：http://wft.daxiang520.top

TS:   // 单行；/* 多行 */
来源：http://mok.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://klj.fzhhl.top

Go:   // 单行；/* 多行 */
来源：http://zgn.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hqf.svipenyu.cn

C#:   // 单行；/* 多行 */
来源：http://eoz.guannengcc.top

[A15] 空值判断与默认值
来源：http://afs.iojbl.cn

Py:   value = data or "默认值"
来源：http://sym.shzxlz.cn

PHP:  $value = $data ?? "默认值";
来源：http://slc.aizwys.cn

JS:   const value = data ?? "默认值";
来源：http://xzh.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://cbt.yuxming.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sra.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://uef.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://lhk.zhixingplan.top

C#:   var value = data ?? "默认值";
来源：http://xjx.cucudq.cn

[A16] 真假值判断规则
来源：http://gwq.yonumen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://shv.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ioy.fktsv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jxi.snrcjt.cn

TS:   if (!x) {}
来源：http://wgn.fanxiaobao.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gmq.sufxvd.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dyk.meibo888.top

Ruby: unless x            # nil 与 false 为假
来源：http://ocx.daxiang520.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hzs.fengsongda.top

[A17] 位运算
来源：http://new.daxiang520.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wbh.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ods.jiagoushi.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hyc.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ciq.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jbm.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zid.cdnleiting.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hcv.hammf.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfx.bbcook.cn

[A18] 字符与 ASCII 码互转
来源：http://rcp.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://fbc.sxryk.cn

PHP:  ord("A"); chr(65)
来源：http://oln.fanxiaobao.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kft.wangshuangyany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aly.jiagoushi.top

Java: (int) 'A'; (char) 65
来源：http://hjy.jinghuilouyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://khn.cashguo.top

Ruby: "A".ord; 65.chr
来源：http://jpf.birdmap.top

C#:   (int)'A'; (char)65
来源：http://pam.redwolf501.top

[A19] 交换两个变量
来源：http://txi.jinqigfzy.top

Py:   a, b = b, a
来源：http://jjt.shangyingyoupin.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hso.sufxvd.cn

JS:   [a, b] = [b, a];
来源：http://dnj.snrcjt.cn

TS:   [a, b] = [b, a];
来源：http://tga.daxiang520.top

Java: int t = a; a = b; b = t;
来源：http://lwi.uphjek.com

Go:   a, b = b, a
来源：http://tps.zhijiandao.cn

Ruby: a, b = b, a
来源：http://hah.meibo888.top

C#:   (a, b) = (b, a);
来源：http://ysg.bbcook.cn

[A20] 读取标准输入
来源：http://hnt.jqgfzy.top

Py:   name = input("请输入：")
来源：http://zwd.sxryk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aqk.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qck.chenlongwang.top

TS:   // Node.js：readline 模块
来源：http://paa.zdbjq.cn

Java: new Scanner(System.in).nextLine()
来源：http://pjl.redwolf501.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://boj.gzhubu.top

Ruby: gets.chomp
来源：http://rfs.nanxuanxn.top

C#:   Console.ReadLine();
来源：http://obi.fktsv.cn

[A21] 保留指定小数位输出
来源：http://fgf.hnqzz.top

Py:   f"{3.14159:.2f}"
来源：http://pyl.fanxiaobao.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dep.zhiwuduotai.top

JS:   (3.14159).toFixed(2)
来源：http://zza.ivvv.top

TS:   (3.14159).toFixed(2)
来源：http://aua.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://qfo.chenzaomai.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tyf.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://ywf.gaohongyu789.top

C#:   3.14159.ToString("F2")
来源：http://wft.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://aii.yuanzhike.top

Py:   len(s)
来源：http://spl.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vie.aibaodan.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://isi.ctjpmb.com

TS:   s.length
来源：http://evf.cqqwz.cn

Java: s.length()
来源：http://nxf.fanxiaobao.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dtp.sysykeji.top

Ruby: s.length
来源：http://awt.yuanzhike.top

C#:   s.Length
来源：http://kdl.gaohongyu789.top

[A23] 大小写转换
来源：http://gnr.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lae.cucudq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bqu.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tkt.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lzu.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lfc.dianchejie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tus.yj202588.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lcr.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yej.wangshuangyany.cn

[A24] 去除首尾空白
来源：http://jmr.ctjpmb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ttg.vqdsnc.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tnn.zdqjudy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ceq.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cag.fktsv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vxq.gaohongyu789.top

Go:   strings.TrimSpace(s)
来源：http://swt.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uao.snrcjt.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nxm.fanxiaobao.xyz

[A25] 字符串比较
来源：http://uev.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://ekb.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iyy.jinyuanbaomall.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rji.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mwf.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tyd.fengsongda.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://alc.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zue.cheryme.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wra.haohaochexian.top

[A26] 类型转换总览
来源：http://hwc.aibaodan.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wsc.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xcq.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qtd.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://jze.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ezd.zdbjq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iwd.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dwl.shangyingyoupin.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qng.chenjidiqi.icu

================================================================================
来源：http://lhw.jqgfzy.top

B. 流程控制
来源：http://lzn.xingfuxueyuan.xyz

================================================================================
来源：http://wyi.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://mtq.ctjpmb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://hdk.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eyn.cdnleiting.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ppk.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://inc.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kww.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gfd.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://glq.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://utd.ybcxt.top

[B02] 多分支 else if / elif
来源：http://ryj.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fky.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ogt.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iwr.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fix.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sll.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rsw.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eum.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rpl.jyoumei.cn

[B03] switch / match / case
来源：http://gmk.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qmk.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lvp.shanyushiyangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mcm.havefunace.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jvo.pengpengdd.cyou

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bed.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://brp.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cqz.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qgq.tian-w.cn

[B04] for 计数循环
来源：http://ork.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://pwk.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gtu.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yud.yonumen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ziu.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jdr.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yts.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://qfk.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gci.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://cgn.hammf.cn

Py:   for item in arr: print(item)
来源：http://poq.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qjo.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cpf.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wjl.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kbz.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qdm.aibaodan.cn

Ruby: arr.each { |item| puts item }
来源：http://lwc.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zof.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://dvy.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rso.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jxm.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ntv.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ilm.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ken.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gxv.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vuk.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aby.jiagoushi.top

[B07] while 循环
来源：http://ocs.xinyue.icu

Py:   while i < 10: i += 1
来源：http://wmk.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://edw.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://uma.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://wqd.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://gqq.yj20258.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://csf.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://siy.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://sug.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://zsz.hnxiangtu.top

Py:   # 无 do-while：用 while True + break
来源：http://zua.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fvr.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://wbo.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://csb.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://hyl.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://szu.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://eiq.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://yoy.svipenyu.cn

[B09] break 与 continue
来源：http://xzq.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://stp.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kfb.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyj.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vob.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smj.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oyx.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://igx.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwn.nanxuanxn.top

[B10] 遍历同时拿索引
来源：http://voo.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sau.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tvr.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zpj.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://isg.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dfr.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ckm.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kck.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oru.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://eum.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://qfu.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://lds.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mzf.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bqj.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hzs.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://syv.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://ubt.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vpy.tarul.cn

[B12] 跳出多层循环
来源：http://mob.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://qtb.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vgp.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xky.yj202588.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hfe.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wew.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rrq.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lsa.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ryh.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://tnw.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://epu.guannengcc.top

PHP:  is_numeric($x)
来源：http://cxh.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rfn.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alg.tarul.cn

Java: x instanceof Number
来源：http://juf.ivvv.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eto.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://vmz.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://ttr.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://nrb.guowangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mca.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rsd.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://rtc.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://lym.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://exk.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ymn.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nlw.andypj.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xsw.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://wis.hnxiangtu.top

Py:   a and b or not c
来源：http://myt.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://tqs.yj20258.top

JS:   a && b || !c
来源：http://dul.wangdashe.top

TS:   a && b || !c
来源：http://koy.andypj.xyz

Java: a && b || !c
来源：http://qgo.jinqigfzy.top

Go:   a && b || !c
来源：http://wmk.cdnleiting.top

Ruby: a && b || !c
来源：http://caa.iojbl.cn

C#:   a && b || !c
来源：http://uuq.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://iqf.andypj.xyz

Py:   if not data: return
来源：http://icz.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://gne.uphjek.com

JS:   if (!data) return;
来源：http://zwh.meibo888.top

TS:   if (!data) return;
来源：http://phd.yj202588.top

Java: if (data == null) return;
来源：http://oso.andypj.xyz

Go:   if data == nil { return }
来源：http://yjc.sxryk.cn

Ruby: return if data.nil?
来源：http://esu.smart0.xyz

C#:   if (data == null) return;
来源：http://fpx.fzhhl.top

================================================================================
来源：http://nap.hysaishi.cn

C. 函数与作用域
来源：http://cdi.tian-w.cn

================================================================================
来源：http://hqg.cdnleiting.top

[C01] 定义函数
来源：http://aec.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://bxd.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qze.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://nij.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kaj.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qpm.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://nwi.hcnkem.com

Ruby: def add(a, b); a + b; end
来源：http://ltd.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vxj.zhengqikj.top

[C02] 默认参数
来源：http://pru.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://guq.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://toh.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://itl.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gzd.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xoc.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ylw.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://cos.meibo888.top


<!-- 参考信息 -->