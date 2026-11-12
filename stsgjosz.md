代发 wailian999

Java: "第一行\n第二行"
来源：http://ubn.xuetiantiany.cn

Go:   "第一行\n第二行"
来源：http://kjw.bbcook.cn

Ruby: "第一行\n第二行"
来源：http://ncu.yfazqb.com

C#:   "第一行\n第二行"
来源：http://blr.chenlongwang.top

[A14] 注释写法
来源：http://mve.iojbl.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://amw.sweek.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wyr.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://bvg.dianchejie.cn

TS:   // 单行；/* 多行 */
来源：http://dax.pengpengdd.cyou

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dpl.yj20258.top

Go:   // 单行；/* 多行 */
来源：http://uod.chenzaomai.com

Ruby: # 单行；=begin 多行 =end
来源：http://qtw.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://ivn.zhiwuduotai.top

[A15] 空值判断与默认值
来源：http://alc.hnqzz.top

Py:   value = data or "默认值"
来源：http://gud.yj202588.top

PHP:  $value = $data ?? "默认值";
来源：http://qsh.xziqi.cn

JS:   const value = data ?? "默认值";
来源：http://gqr.ywan-chungtsiang.top

TS:   const value = data ?? "默认值";
来源：http://byy.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zaz.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://zds.tanke756.top

Ruby: value = data || "默认值"
来源：http://cbp.zdqjudy.top

C#:   var value = data ?? "默认值";
来源：http://wln.gogol.net.cn

[A16] 真假值判断规则
来源：http://rva.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oaj.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://emr.zhijiandao.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uoy.xylfe.cn

TS:   if (!x) {}
来源：http://vhe.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ygv.birdmap.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hhl.xingfuxueyuan.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://eeh.hesvh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ocs.andypj.xyz

[A17] 位运算
来源：http://heh.pycfn.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mqh.cucudq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ubq.ehwqpu.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vzi.xylfe.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uxh.dianchejie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gav.jyoumei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wxc.xingfuxueyuan.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wou.bbcook.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qka.pengpengdd.cyou

[A18] 字符与 ASCII 码互转
来源：http://lru.nanxuanxn.top

Py:   ord("A"); chr(65)
来源：http://tmt.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://pee.yfazqb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ltr.chenzaomai.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wbx.yonumen.top

Java: (int) 'A'; (char) 65
来源：http://rgr.sjlbkw.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zaw.c1oappe.top

Ruby: "A".ord; 65.chr
来源：http://jye.hnxiangtu.top

C#:   (int)'A'; (char)65
来源：http://pog.zhaomingkeji.xyz

[A19] 交换两个变量
来源：http://kdu.daxiang520.top

Py:   a, b = b, a
来源：http://iry.cheryme.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xiu.zhoulong.xyz

JS:   [a, b] = [b, a];
来源：http://gih.shuidangran.top

TS:   [a, b] = [b, a];
来源：http://pkz.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://cus.xuetiantiany.cn

Go:   a, b = b, a
来源：http://nml.xuetiantiany.cn

Ruby: a, b = b, a
来源：http://yta.haohaochexian.top

C#:   (a, b) = (b, a);
来源：http://twr.0kj1m.cn

[A20] 读取标准输入
来源：http://voe.fengsongda.top

Py:   name = input("请输入：")
来源：http://zlp.andypj.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://ecr.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ais.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://zvb.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://swj.dashuyun.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hrl.hnqzz.top

Ruby: gets.chomp
来源：http://yly.gzhubu.top

C#:   Console.ReadLine();
来源：http://zgq.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://lgq.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://lnl.yongpay.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dax.jqgfzy.top

JS:   (3.14159).toFixed(2)
来源：http://ypc.shanyushiyangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://uee.xuetiantiany.cn

Java: String.format("%.2f", 3.14159)
来源：http://piu.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iko.xingfuxueyuan.xyz

Ruby: format("%.2f", 3.14159)
来源：http://edl.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://ebt.chenlongwang.top

[A22] 获取字符串长度
来源：http://inc.yuxming.cn

Py:   len(s)
来源：http://xzk.ydzc1.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gcj.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wrt.cashguo.top

TS:   s.length
来源：http://djz.cheryme.top

Java: s.length()
来源：http://wft.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jwm.ydjk.org.cn

Ruby: s.length
来源：http://ihc.jqgufenzy.top

C#:   s.Length
来源：http://pcp.zycfv.cn

[A23] 大小写转换
来源：http://ftl.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vdh.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ulj.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hih.yj20258.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://elx.tanke756.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zkt.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://usw.zdbjq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pka.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://vpt.daria6918.cn

[A24] 去除首尾空白
来源：http://wny.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ivx.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vxp.yonumen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pte.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hnm.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://psb.jiagoushi.top

Go:   strings.TrimSpace(s)
来源：http://vzb.hywenlv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://odk.cashguo.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wun.yuanzhike.top

[A25] 字符串比较
来源：http://cll.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://ktx.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bhi.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mka.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zwj.vqdsnc.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://enu.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lja.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oho.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yrc.fehbvm.com

[A26] 类型转换总览
来源：http://vkt.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cre.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ykd.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yhx.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://jig.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cmv.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ech.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jwp.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xzw.cdnleiting.top

================================================================================
来源：http://zue.fanxiaobao.xyz

B. 流程控制
来源：http://cav.haohaochexian.top

================================================================================
来源：http://twf.jqgufenzy.top

[B01] 条件判断 if / else
来源：http://imw.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fmr.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cqr.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qnm.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qub.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://oul.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vfh.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ays.zhijiandao.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cvy.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://btr.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aln.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fku.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.gogol.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyy.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kug.316326.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://koi.guowangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kti.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://own.jyoumei.cn

[B03] switch / match / case
来源：http://kxm.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bde.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jae.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://trx.nanxinkj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zrk.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mko.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iuk.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yut.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hgq.cashguo.top

[B04] for 计数循环
来源：http://mzo.yfazqb.com

Py:   for i in range(10): print(i)
来源：http://suu.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lxq.gotoacloud.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cld.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eoq.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ygi.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ukz.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://yer.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bdi.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://lkc.aizwys.cn

Py:   for item in arr: print(item)
来源：http://vqp.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dcg.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ceu.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gsn.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pmx.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pnk.ehwqpu.com

Ruby: arr.each { |item| puts item }
来源：http://xky.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eih.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://rlc.yuanzhike.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gcp.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://evg.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hmf.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://srf.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ecb.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://auj.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nma.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wah.shangyingyoupin.top

[B07] while 循环
来源：http://ihy.fanxiaobao.xyz

Py:   while i < 10: i += 1
来源：http://mbk.ywan-chungtsiang.top

PHP:  while ($i < 10) { $i++; }
来源：http://enk.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://nwu.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://skm.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://auh.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kwa.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://wai.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://wsi.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://wwf.xinyue.icu

Py:   # 无 do-while：用 while True + break
来源：http://idy.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ehl.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://zee.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://wxl.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://uzr.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://liz.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://zgl.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://scs.zhoulong.xyz

[B09] break 与 continue
来源：http://xaj.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mzd.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sab.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzn.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqw.jinghuilouyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eiy.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bxc.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jjq.hfpthk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpe.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://acl.shuidangran.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zmf.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iwr.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gjk.yuxming.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gsd.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zoe.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zle.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://phj.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mvq.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://ppk.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://skl.havefunace.top

PHP:  range(0, 10, 2);
来源：http://tzb.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggb.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bdt.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://upl.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kky.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://ycm.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gct.gogol.net.cn

[B12] 跳出多层循环
来源：http://znd.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://ece.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://elm.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xbh.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wzv.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kar.c1oappe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ydx.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xzo.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gju.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://hxa.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://bqf.nanxuanxn.top

PHP:  is_numeric($x)
来源：http://rkp.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uel.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lwu.cdnleiting.top

Java: x instanceof Number
来源：http://ddx.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hzf.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://wvt.jiagoushi.top

C#:   x is int or double or decimal
来源：http://zox.fengsongda.top

[B14] 判断值是否在集合内
来源：http://atz.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tar.yfazqb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://emp.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://oym.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://phm.hfpthk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ivr.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gmb.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://okr.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xor.tanke756.top

[B15] 布尔运算与取反
来源：http://mfh.xziqi.cn

Py:   a and b or not c
来源：http://plk.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://aej.ppjwa.cn

JS:   a && b || !c
来源：http://xvx.0kj1m.cn

TS:   a && b || !c
来源：http://jov.fehbvm.com

Java: a && b || !c
来源：http://oou.hongshengwenyu.top

Go:   a && b || !c
来源：http://hab.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://olv.yfazqb.com

C#:   a && b || !c
来源：http://bcj.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://erx.hywenlv.cn

Py:   if not data: return
来源：http://zfh.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://mxp.hnqzz.top

JS:   if (!data) return;
来源：http://dwr.nanxuanxn.top

TS:   if (!data) return;
来源：http://pcr.chenzaomai.com

Java: if (data == null) return;
来源：http://max.sufxvd.cn

Go:   if data == nil { return }
来源：http://dmr.birdmap.top

Ruby: return if data.nil?
来源：http://jtm.quarkkingdee.top

C#:   if (data == null) return;
来源：http://doy.ybcxt.top

================================================================================
来源：http://cjv.xingfuxueyuan.xyz

C. 函数与作用域
来源：http://omw.hnqzz.top

================================================================================
来源：http://wxk.yj202588.top

[C01] 定义函数
来源：http://odc.yonumen.top

Py:   def add(a, b): return a + b
来源：http://yta.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gxk.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://ahf.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zkv.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ryf.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://xgc.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://dfo.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dpj.yongpay.top

[C02] 默认参数
来源：http://wzm.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://lse.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vxa.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://hnc.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jco.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://wru.ivvv.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://buy.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://fju.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://sow.yj20258888.top

[C03] 可变参数
来源：http://wul.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://tns.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ltg.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rhs.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lta.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ihv.fanxiaobao.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://osy.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://qca.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nnf.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://csb.ctjpmb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ysw.redwolf501.top


<!-- 参考信息 -->