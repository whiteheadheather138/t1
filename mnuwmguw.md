代发 wailian999

Py:   "第一行\n第二行"
来源：http://gsg.yfazqb.com

PHP:  "第一行\n第二行"
来源：http://hcq.gzhubu.top

JS:   "第一行\n第二行"
来源：http://gty.shangyingyoupin.top

TS:   "第一行\n第二行"
来源：http://twr.yongpay.top

Java: "第一行\n第二行"
来源：http://iiy.zhengqikj.top

Go:   "第一行\n第二行"
来源：http://foo.quarkkingdee.top

Ruby: "第一行\n第二行"
来源：http://yhe.yueranfly.top

C#:   "第一行\n第二行"
来源：http://pkb.tianlin.xyz

[A14] 注释写法
来源：http://qzn.ctjpmb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://qsb.jinqigufen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vif.hongshengwenyu.top

JS:   // 单行；/* 多行 */
来源：http://qqj.fzhhl.top

TS:   // 单行；/* 多行 */
来源：http://kjd.feifeiyinyue.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xhr.yfazqb.com

Go:   // 单行；/* 多行 */
来源：http://aym.guannengcc.top

Ruby: # 单行；=begin 多行 =end
来源：http://kmj.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://azq.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://pzf.svipenyu.cn

Py:   value = data or "默认值"
来源：http://tdb.zhixingplan.top

PHP:  $value = $data ?? "默认值";
来源：http://ctb.daxiang520.top

JS:   const value = data ?? "默认值";
来源：http://hbe.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://ybi.0kj1m.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mkw.ctjpmb.com

Go:   if data == "" { data = "默认值" }
来源：http://jpu.birdmap.top

Ruby: value = data || "默认值"
来源：http://cem.cheryme.top

C#:   var value = data ?? "默认值";
来源：http://lvq.jinyuanbaomall.cn

[A16] 真假值判断规则
来源：http://sqq.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gdx.jqgufenzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ync.zhijiandao.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://crg.cqqwz.cn

TS:   if (!x) {}
来源：http://dqz.hammf.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yjd.zhiwuduotai.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pjd.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kml.hammf.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bgz.gaohongyu789.top

[A17] 位运算
来源：http://lhp.yonumen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xod.quarkkingdee.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://usu.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wsl.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zid.ctjpmb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jhb.gaohongyu789.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ihl.ywan-chungtsiang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jvf.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmn.jiagoushi.top

[A18] 字符与 ASCII 码互转
来源：http://ddm.kuanghao11.cn

Py:   ord("A"); chr(65)
来源：http://cip.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://vuv.yfazqb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ytb.andypj.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bia.fanxiaobao.xyz

Java: (int) 'A'; (char) 65
来源：http://uma.9152youxi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mqh.tian-w.cn

Ruby: "A".ord; 65.chr
来源：http://hfz.zdqjudy.top

C#:   (int)'A'; (char)65
来源：http://irl.mhx1999.top

[A19] 交换两个变量
来源：http://ngw.sxryk.cn

Py:   a, b = b, a
来源：http://bag.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xvv.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://czd.zhaomingkeji.xyz

TS:   [a, b] = [b, a];
来源：http://mpi.fzhhl.top

Java: int t = a; a = b; b = t;
来源：http://wjx.zhiwuduotai.top

Go:   a, b = b, a
来源：http://aqn.pycfn.com

Ruby: a, b = b, a
来源：http://hyf.jyoumei.cn

C#:   (a, b) = (b, a);
来源：http://izj.uphjek.com

[A20] 读取标准输入
来源：http://tpq.vehdjk.com

Py:   name = input("请输入：")
来源：http://mox.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://quk.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fis.guannengcc.top

TS:   // Node.js：readline 模块
来源：http://ssu.dianchejie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ppa.iojbl.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mbb.jqgfzy.top

Ruby: gets.chomp
来源：http://yto.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://udv.birdmap.top

[A21] 保留指定小数位输出
来源：http://pmq.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://jbc.xingfuxueyuan.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ybp.xuanzx.com

JS:   (3.14159).toFixed(2)
来源：http://oov.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://elb.hesvh.cn

Java: String.format("%.2f", 3.14159)
来源：http://nkq.yangfankeji.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nap.iojbl.cn

Ruby: format("%.2f", 3.14159)
来源：http://exn.ehwqpu.com

C#:   3.14159.ToString("F2")
来源：http://gdr.9152youxi.cn

[A22] 获取字符串长度
来源：http://agi.yongpay.top

Py:   len(s)
来源：http://myh.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pny.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qzn.xuetiantiany.cn

TS:   s.length
来源：http://dlz.feifeiyinyue.top

Java: s.length()
来源：http://myk.feifeiyinyue.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xed.bjfxy.top

Ruby: s.length
来源：http://jen.zdbjq.cn

C#:   s.Length
来源：http://bgk.mhx1999.top

[A23] 大小写转换
来源：http://twp.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://efc.cashguo.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oap.jinghuilouyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lpm.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tbd.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ioq.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cck.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zpn.ctjpmb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://lec.yonumen.top

[A24] 去除首尾空白
来源：http://gxr.chenlongwang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ani.zhijiandao.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tkh.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://atx.yj20258.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vza.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vji.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://hws.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://noa.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tlq.aizwys.cn

[A25] 字符串比较
来源：http://jqm.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://yor.meibo888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://geh.yongpay.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gvm.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oky.hfpthk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qky.cucudq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zsz.ybcxt.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bmx.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vut.tianlin.xyz

[A26] 类型转换总览
来源：http://jer.sjlbkw.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ued.ehwqpu.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://huh.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ite.bjfxy.top

TS:   Number() String() Boolean() x as number
来源：http://krf.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lqt.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zoq.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gsk.snrcjt.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uya.jinqigufen.top

================================================================================
来源：http://omn.dashuyun.cn

B. 流程控制
来源：http://fva.jinqigufen.top

================================================================================
来源：http://akl.bbcook.cn

[B01] 条件判断 if / else
来源：http://kje.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rzs.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://usz.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tmf.uphjek.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://otn.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tuv.bbcook.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ner.jinyuanbaomall.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ufv.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ylm.tian-w.cn

[B02] 多分支 else if / elif
来源：http://qxs.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://igb.gogol.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pdo.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khg.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jci.yj20258888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggp.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://syg.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baq.sxryk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xno.tian-w.cn

[B03] switch / match / case
来源：http://tik.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fcb.yj202588.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eqr.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nzz.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xbj.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cun.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nbb.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rfl.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jvo.ehwqpu.com

[B04] for 计数循环
来源：http://szg.yj20258.top

Py:   for i in range(10): print(i)
来源：http://evw.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kzz.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ugk.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ztu.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gij.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xdy.zhoulong.xyz

Ruby: 10.times { |i| puts i }
来源：http://agb.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hfs.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://sio.hnqzz.top

Py:   for item in arr: print(item)
来源：http://mmd.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://obj.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pjc.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wdp.jinqigfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://eqh.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://buk.cashguo.top

Ruby: arr.each { |item| puts item }
来源：http://yfr.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cea.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://vno.pycfn.com

Py:   for k, v in d.items(): print(k, v)
来源：http://uls.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yzt.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dhj.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cnd.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rcr.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vuy.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xtu.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yjq.hammf.cn

[B07] while 循环
来源：http://cfm.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://plp.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://bqt.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://zuv.guannengcc.top

TS:   while (i < 10) { i++; }
来源：http://yhn.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://ocr.ivvv.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://whk.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://fgv.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://gld.jianghu66.top

[B08] do-while（至少执行一次）
来源：http://wim.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://xws.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yrw.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://efq.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://grb.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://dvq.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lun.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://oop.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://ykl.uphjek.com

[B09] break 与 continue
来源：http://baz.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://khz.zhoulong.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cmj.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jcv.jlsjyb.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vol.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mvv.dashuyun.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nvf.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://icv.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ojd.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://kdt.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jnr.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://swa.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zlw.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kzk.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lbg.cheryme.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cmd.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qlt.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ozb.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://bvi.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://prx.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://naz.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qhq.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kqv.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jdd.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aoc.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://pgx.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://doj.meibo888.top

[B12] 跳出多层循环
来源：http://nmq.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fei.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yxv.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://icy.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qrn.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uvj.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://asu.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://krs.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wbg.aibaodan.cn

[B13] 判断是否为数字
来源：http://ebf.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://zlb.birdmap.top

PHP:  is_numeric($x)
来源：http://iht.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jgh.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://egx.bjfxy.top

Java: x instanceof Number
来源：http://jdt.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zwp.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://yse.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://zhr.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://nsk.hongshengwenyu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ldj.yueranfly.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://twc.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://drx.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://csh.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mil.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vcy.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://akm.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://phc.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://wrb.xziqi.cn

Py:   a and b or not c
来源：http://ivg.c1oappe.top

PHP:  $a && $b || !$c
来源：http://izx.cqqwz.cn

JS:   a && b || !c
来源：http://tpf.quarkkingdee.top

TS:   a && b || !c
来源：http://qwx.52xcode.cn

Java: a && b || !c
来源：http://lzm.hywenlv.cn

Go:   a && b || !c
来源：http://gwk.sjlbkw.cn

Ruby: a && b || !c
来源：http://ddz.hcnkem.com

C#:   a && b || !c
来源：http://xnb.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://jfn.yvedp.cn

Py:   if not data: return
来源：http://bnb.havefunace.top

PHP:  if (!$data) { return; }
来源：http://zlu.feifeiyinyue.top

JS:   if (!data) return;
来源：http://kqd.zhijiandao.cn

TS:   if (!data) return;
来源：http://tix.yongpay.top

Java: if (data == null) return;
来源：http://igy.gzhubu.top

Go:   if data == nil { return }
来源：http://boh.tanke756.top

Ruby: return if data.nil?
来源：http://owu.zhijiandao.cn

C#:   if (data == null) return;
来源：http://qaq.xuanzx.com

================================================================================
来源：http://umc.yonumen.top

C. 函数与作用域
来源：http://gyn.shangyingyoupin.top

================================================================================
来源：http://cmo.fanxiaobao.xyz

[C01] 定义函数
来源：http://cxo.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://pil.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tnf.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://ykj.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ifu.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yre.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vyv.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://och.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iit.shanyushiyangkeji.top

[C02] 默认参数
来源：http://pmh.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://lwo.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mso.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://aap.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://qrv.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://myj.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rui.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://fnz.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://fiu.haohaochexian.top

[C03] 可变参数
来源：http://dpi.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://fok.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rdd.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zpr.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtg.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lnn.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nqr.yueranfly.top


<!-- 参考信息 -->