代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eqy.jinghuilouyu.cn

JS:   `Hello, ${name}!`
来源：http://ufj.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://oju.shuidangran.top

Java: "Hello, %s!".formatted(name)
来源：http://gzl.mhx1999.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lep.andypj.xyz

Ruby: "Hello, #{name}!"
来源：http://xpt.tian-w.cn

C#:   $"Hello, {name}!"
来源：http://uct.mhx1999.top

[A13] 多行字符串（练习 \n 转义）
来源：http://sjw.zhiwuduotai.top

Py:   "第一行\n第二行"
来源：http://jbf.uphjek.com

PHP:  "第一行\n第二行"
来源：http://ilp.cucudq.cn

JS:   "第一行\n第二行"
来源：http://pbd.fanxiaobao.xyz

TS:   "第一行\n第二行"
来源：http://wvr.hesvh.cn

Java: "第一行\n第二行"
来源：http://wfi.shanyushiyangtech.top

Go:   "第一行\n第二行"
来源：http://ywk.ivvv.top

Ruby: "第一行\n第二行"
来源：http://svr.sjlbkw.cn

C#:   "第一行\n第二行"
来源：http://sgv.jinqigufen.top

[A14] 注释写法
来源：http://uue.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rqw.cashguo.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lnn.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://hib.haohaochexian.top

TS:   // 单行；/* 多行 */
来源：http://vjn.yueranfly.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xpd.xuetiantiany.cn

Go:   // 单行；/* 多行 */
来源：http://nrn.nanxinkj.top

Ruby: # 单行；=begin 多行 =end
来源：http://vmc.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://fkp.nwbrower.top

[A15] 空值判断与默认值
来源：http://lgw.hongshengwenyu.top

Py:   value = data or "默认值"
来源：http://vrk.zhoulong.xyz

PHP:  $value = $data ?? "默认值";
来源：http://hcb.xinyue.icu

JS:   const value = data ?? "默认值";
来源：http://txb.smart0.xyz

TS:   const value = data ?? "默认值";
来源：http://xwl.ppjwa.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rge.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://cmb.chenzaomai.com

Ruby: value = data || "默认值"
来源：http://wud.fanxiaobao.xyz

C#:   var value = data ?? "默认值";
来源：http://ycs.iojbl.cn

[A16] 真假值判断规则
来源：http://xho.sufxvd.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rki.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mxq.zhongyouzk.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zrz.aibaodan.cn

TS:   if (!x) {}
来源：http://bqc.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dyx.wangdashe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://amq.xingfuxueyuan.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://ziz.svipenyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gdv.jqgfzy.top

[A17] 位运算
来源：http://ryn.wangdashe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cif.cheryme.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rwf.sweek.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xoo.tian-w.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://buk.yj20258888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uyg.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hic.smart0.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ypu.chenzaomai.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ffx.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://hsq.zhongyouzk.top

Py:   ord("A"); chr(65)
来源：http://xqu.daxiang520.top

PHP:  ord("A"); chr(65)
来源：http://mip.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wfn.havefunace.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zps.havefunace.top

Java: (int) 'A'; (char) 65
来源：http://zzh.sysykeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mkx.fzhhl.top

Ruby: "A".ord; 65.chr
来源：http://qls.yongpay.top

C#:   (int)'A'; (char)65
来源：http://lgd.jiagoushi.top

[A19] 交换两个变量
来源：http://roj.0kj1m.cn

Py:   a, b = b, a
来源：http://zeu.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qdw.chenzaomai.com

JS:   [a, b] = [b, a];
来源：http://vah.jinqigfzy.top

TS:   [a, b] = [b, a];
来源：http://wnq.yonumen.top

Java: int t = a; a = b; b = t;
来源：http://gbr.cucudq.cn

Go:   a, b = b, a
来源：http://hnt.tianlin.xyz

Ruby: a, b = b, a
来源：http://npg.yj20258.top

C#:   (a, b) = (b, a);
来源：http://iia.hysaishi.cn

[A20] 读取标准输入
来源：http://rwu.tianlin.xyz

Py:   name = input("请输入：")
来源：http://yir.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://khn.gotoacloud.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://etf.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://trt.sysykeji.top

Java: new Scanner(System.in).nextLine()
来源：http://nvi.aibaodan.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://orq.0kj1m.cn

Ruby: gets.chomp
来源：http://uvj.haohaochexian.top

C#:   Console.ReadLine();
来源：http://lvy.cucudq.cn

[A21] 保留指定小数位输出
来源：http://tou.wangdashe.top

Py:   f"{3.14159:.2f}"
来源：http://ohu.vehdjk.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rrr.fktsv.cn

JS:   (3.14159).toFixed(2)
来源：http://ybu.epnwcf.com

TS:   (3.14159).toFixed(2)
来源：http://ylw.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://ltx.guowangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fkq.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://tyd.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://hjd.havefunace.top

[A22] 获取字符串长度
来源：http://cyn.yueranfly.top

Py:   len(s)
来源：http://sye.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kgv.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qzh.zhixingplan.top

TS:   s.length
来源：http://vrd.cashguo.top

Java: s.length()
来源：http://hum.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aso.yueranfly.top

Ruby: s.length
来源：http://ibt.hnqzz.top

C#:   s.Length
来源：http://pad.zhoulong.xyz

[A23] 大小写转换
来源：http://yzc.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bfm.tian-w.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lea.kuanghao11.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wyj.tarul.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zry.shanyushiyangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ixc.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rkp.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dtp.gogol.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://knj.sjlbkw.cn

[A24] 去除首尾空白
来源：http://vvp.xinyue.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://drd.jinqigfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://foj.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lkx.meibo888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fkq.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xpr.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://rbr.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yzf.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lyd.smart0.xyz

[A25] 字符串比较
来源：http://yie.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://its.meibo888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://faz.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pxy.hammf.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ifi.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://epg.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kxi.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jez.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bqj.cucudq.cn

[A26] 类型转换总览
来源：http://wqx.kuanghao11.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://toy.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ejl.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uii.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://fmt.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ekm.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://auo.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lkc.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://szh.yonumen.top

================================================================================
来源：http://udi.shzxlz.cn

B. 流程控制
来源：http://ipn.ppjwa.cn

================================================================================
来源：http://tyg.pengpengdd.cyou

[B01] 条件判断 if / else
来源：http://kfj.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://rzh.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kuk.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tuk.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://elp.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://szi.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gyu.tarul.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jye.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cqa.cucudq.cn

[B02] 多分支 else if / elif
来源：http://jzo.fengsongda.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bbb.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iii.yj20258.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bkh.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lkp.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://etv.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ugo.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mpk.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dtd.9152youxi.cn

[B03] switch / match / case
来源：http://bhd.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://glc.epnwcf.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jic.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rti.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jbo.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fwm.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vsn.jqgufenzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nrc.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zar.havefunace.top

[B04] for 计数循环
来源：http://mpe.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://fgb.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lkn.cdnleiting.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dyi.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oxf.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cvg.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qhm.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://iyq.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xbs.zdbjq.cn

[B05] 遍历数组 / 列表
来源：http://slc.uphjek.com

Py:   for item in arr: print(item)
来源：http://jfd.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lzw.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uch.yvedp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nnr.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fmv.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kaz.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://isu.jinyuanbaomall.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pxb.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://gqq.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wsk.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vzb.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qpt.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bsm.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bmw.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hbt.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yan.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://frr.fengsongda.top

[B07] while 循环
来源：http://ovy.tarul.cn

Py:   while i < 10: i += 1
来源：http://zsb.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fef.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://czd.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://fjk.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://qmj.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://duk.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://mzm.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://lnt.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://pen.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://hgf.jqgfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cfu.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://wub.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://lvc.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://byy.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dyd.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://lyo.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://aor.wangshuangyany.cn

[B09] break 与 continue
来源：http://gby.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cjf.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jcp.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lfv.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gam.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://buw.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yyo.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ask.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qpu.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://nty.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tan.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rwx.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zwb.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wqa.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qvr.dashuyun.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wem.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jtb.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yjv.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://uon.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://xgy.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://qqj.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zkv.chenlongwang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dfp.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zsj.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://haz.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://mkl.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ikh.xylfe.cn

[B12] 跳出多层循环
来源：http://ofy.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://oew.aibaodan.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dmr.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gie.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gpr.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://etc.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://upx.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wgd.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jxu.dashuyun.cn

[B13] 判断是否为数字
来源：http://uud.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://bud.fktsv.cn

PHP:  is_numeric($x)
来源：http://vkn.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gps.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yoy.dashuyun.cn

Java: x instanceof Number
来源：http://rkg.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pqm.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://ffa.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://lpe.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://zjm.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uuy.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zlk.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://jeg.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://kmj.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mlo.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ktv.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://qpk.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oxw.guannengcc.top

[B15] 布尔运算与取反
来源：http://zcm.daria6918.cn

Py:   a and b or not c
来源：http://dwl.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://zjh.daxiang520.top

JS:   a && b || !c
来源：http://zve.svipenyu.cn

TS:   a && b || !c
来源：http://fqb.shuidangran.top

Java: a && b || !c
来源：http://toz.aizwys.cn

Go:   a && b || !c
来源：http://zoa.ppjwa.cn

Ruby: a && b || !c
来源：http://hgx.jqgfzy.top

C#:   a && b || !c
来源：http://vzv.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://lgt.cheryme.top

Py:   if not data: return
来源：http://wep.gzhubu.top

PHP:  if (!$data) { return; }
来源：http://xyr.quarkkingdee.top

JS:   if (!data) return;
来源：http://mvz.yangfankeji.com

TS:   if (!data) return;
来源：http://pfp.zhiwuduotai.top

Java: if (data == null) return;
来源：http://izt.jinqigufen.top

Go:   if data == nil { return }
来源：http://rgz.mhx1999.top

Ruby: return if data.nil?
来源：http://mlw.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://coq.xingfuxueyuan.xyz

================================================================================
来源：http://vlo.c1oappe.top

C. 函数与作用域
来源：http://uie.pengpengdd.cyou

================================================================================
来源：http://kfw.pengpengdd.cyou

[C01] 定义函数
来源：http://wlz.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://obr.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ttm.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://wca.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://edm.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jca.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://fwz.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://dcq.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bkf.yj202588.top

[C02] 默认参数
来源：http://bxf.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://jcu.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zuu.hnqzz.top

JS:   function greet(name = "World") { return name; }
来源：http://dsp.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ugf.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uqc.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rzf.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://eka.zhijiandao.cn


<!-- 参考信息 -->