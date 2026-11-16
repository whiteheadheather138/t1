代发 wailian999

[A14] 注释写法
来源：http://qrs.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hqc.zhoulong.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://fub.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://pgn.yfazqb.com

TS:   // 单行；/* 多行 */
来源：http://tjx.ehwqpu.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gcg.jinqigufen.top

Go:   // 单行；/* 多行 */
来源：http://okk.zhaomingkeji.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://ggx.316326.xyz

C#:   // 单行；/* 多行 */
来源：http://qra.sxryk.cn

[A15] 空值判断与默认值
来源：http://kny.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://nlz.jqgfzy.top

PHP:  $value = $data ?? "默认值";
来源：http://ixj.jqgfzy.top

JS:   const value = data ?? "默认值";
来源：http://drx.ywan-chungtsiang.top

TS:   const value = data ?? "默认值";
来源：http://fou.cashguo.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ymt.jinqigfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://zwu.gaohongyu789.top

Ruby: value = data || "默认值"
来源：http://ekc.jinqigfzy.top

C#:   var value = data ?? "默认值";
来源：http://buu.fktsv.cn

[A16] 真假值判断规则
来源：http://mpi.cheryme.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wzc.yonumen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mwj.daxiang520.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rpu.epnwcf.com

TS:   if (!x) {}
来源：http://akh.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://alk.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vbe.cashguo.top

Ruby: unless x            # nil 与 false 为假
来源：http://khf.yonumen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wso.jiagoushi.top

[A17] 位运算
来源：http://ofq.shangyingyoupin.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qfh.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qgb.jiagoushi.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cxl.sufxvd.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mwt.daria6918.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ajc.shzxlz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gve.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wds.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tks.hywenlv.cn

[A18] 字符与 ASCII 码互转
来源：http://rna.birdmap.top

Py:   ord("A"); chr(65)
来源：http://ivc.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://odm.tianlin.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ibz.uphjek.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uer.hnxiangtu.top

Java: (int) 'A'; (char) 65
来源：http://zuo.yuanzhike.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qvi.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://tzs.yuxming.cn

C#:   (int)'A'; (char)65
来源：http://fzd.meibo888.top

[A19] 交换两个变量
来源：http://szb.ehwqpu.com

Py:   a, b = b, a
来源：http://sid.hywenlv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cas.jinghuilouyu.cn

JS:   [a, b] = [b, a];
来源：http://hlx.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://syn.zhengqikj.top

Java: int t = a; a = b; b = t;
来源：http://bwo.xylfe.cn

Go:   a, b = b, a
来源：http://smu.hesvh.cn

Ruby: a, b = b, a
来源：http://qxd.ywan-chungtsiang.top

C#:   (a, b) = (b, a);
来源：http://qog.shzxlz.cn

[A20] 读取标准输入
来源：http://bpc.fzhhl.top

Py:   name = input("请输入：")
来源：http://jsg.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wzf.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ler.nanxuanxn.top

TS:   // Node.js：readline 模块
来源：http://yan.haohaochexian.top

Java: new Scanner(System.in).nextLine()
来源：http://npc.hywenlv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sxd.hnxiangtu.top

Ruby: gets.chomp
来源：http://ban.aibaodan.cn

C#:   Console.ReadLine();
来源：http://nhx.ppjwa.cn

[A21] 保留指定小数位输出
来源：http://hcy.nanxuanxn.top

Py:   f"{3.14159:.2f}"
来源：http://atp.hywenlv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oho.sxryk.cn

JS:   (3.14159).toFixed(2)
来源：http://lbd.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://pqa.tarul.cn

Java: String.format("%.2f", 3.14159)
来源：http://rzy.52xcode.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lat.yvedp.cn

Ruby: format("%.2f", 3.14159)
来源：http://ohx.wangshuangyany.cn

C#:   3.14159.ToString("F2")
来源：http://hll.aibaodan.cn

[A22] 获取字符串长度
来源：http://dwq.jyoumei.cn

Py:   len(s)
来源：http://zdw.iojbl.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bmz.yuanzhike.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://exq.hammf.cn

TS:   s.length
来源：http://wqg.chenlongwang.top

Java: s.length()
来源：http://bmd.wangshuangyany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jgc.ehwqpu.com

Ruby: s.length
来源：http://zpp.ehwqpu.com

C#:   s.Length
来源：http://hdm.pycfn.com

[A23] 大小写转换
来源：http://bxe.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://upt.nanxinkj.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ifi.fengsongda.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jxq.sjlbkw.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xgw.mhx1999.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jye.shangyingyoupin.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dcp.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://omv.tianlin.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://wwv.gaohongyu789.top

[A24] 去除首尾空白
来源：http://nza.316326.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mfe.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zdq.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://axd.xinyue.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tpr.gzhubu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tqe.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://urc.sjlbkw.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tml.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cgi.fktsv.cn

[A25] 字符串比较
来源：http://six.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://mth.jianghu66.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ovs.ehwqpu.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ivd.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cwq.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yuh.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qjf.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ebk.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tzl.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://wvl.sjlbkw.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hog.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://omz.yonumen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tdj.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://qfm.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zik.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://paw.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dfw.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fed.sjlbkw.cn

================================================================================
来源：http://qjc.tanke756.top

B. 流程控制
来源：http://oms.uphjek.com

================================================================================
来源：http://vcw.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://gqy.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://uuo.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wpy.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mdz.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yoc.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://srw.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cvt.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ois.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eij.wangdashe.top

[B02] 多分支 else if / elif
来源：http://iiz.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hhj.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sua.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zgl.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyb.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fjf.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kyt.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nla.ctjpmb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gig.0kj1m.cn

[B03] switch / match / case
来源：http://usr.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cym.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://scb.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jko.zhijiandao.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dlg.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zcn.shuidangran.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cbl.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tow.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qos.ctjpmb.com

[B04] for 计数循环
来源：http://hfo.bjfxy.top

Py:   for i in range(10): print(i)
来源：http://tud.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ukv.jinghuilouyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dbk.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fqa.pycfn.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lbe.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hyf.hywenlv.cn

Ruby: 10.times { |i| puts i }
来源：http://epl.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zci.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://asw.shanyushiyangtech.top

Py:   for item in arr: print(item)
来源：http://rcg.yvedp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yif.yvedp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://amr.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eic.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qrx.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ilw.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://svm.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ewx.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://nut.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hxh.hfpthk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bdb.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wac.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://acd.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uto.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aht.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vfp.yuanzhike.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vjj.yuanzhike.top

[B07] while 循环
来源：http://lew.yueranfly.top

Py:   while i < 10: i += 1
来源：http://pzw.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://wxm.xuetiantiany.cn

JS:   while (i < 10) { i++; }
来源：http://wtl.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://hbk.yuxming.cn

Java: while (i < 10) { i++; }
来源：http://qwt.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://opn.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://abk.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://ycf.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://qfp.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://rif.jinghuilouyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://drs.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://hnw.gaohongyu789.top

TS:   do { i++; } while (i < 10);
来源：http://hno.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://bxw.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hvp.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://xev.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://eaz.smart0.xyz

[B09] break 与 continue
来源：http://win.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://epx.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mqi.feifeiyinyue.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yjx.zdbjq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kaw.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ini.zhiwuduotai.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xjq.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pht.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nzx.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://zbk.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wsb.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://umd.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bat.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ggg.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://grm.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wmy.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vnp.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ggf.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://sjz.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://whj.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://lky.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mun.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://swv.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mpd.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xkd.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://itk.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cyy.daxiang520.top

[B12] 跳出多层循环
来源：http://ejp.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gdv.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xsz.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oud.sufxvd.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tlx.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sqa.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fyk.fengsongda.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qew.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pws.ivvv.top

[B13] 判断是否为数字
来源：http://izi.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://gdo.hesvh.cn

PHP:  is_numeric($x)
来源：http://avi.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hip.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fiy.cqqwz.cn

Java: x instanceof Number
来源：http://pfp.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tjs.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://wxr.havefunace.top

C#:   x is int or double or decimal
来源：http://dnw.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://wix.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xxb.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ndh.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://swn.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://twv.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cqf.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gvs.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://hve.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://soc.birdmap.top

[B15] 布尔运算与取反
来源：http://cso.aizwys.cn

Py:   a and b or not c
来源：http://ryh.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://gmp.yongpay.top

JS:   a && b || !c
来源：http://ydg.sjlbkw.cn

TS:   a && b || !c
来源：http://wfp.iojbl.cn

Java: a && b || !c
来源：http://ebl.ydjk.org.cn

Go:   a && b || !c
来源：http://jlp.zhixingplan.top

Ruby: a && b || !c
来源：http://hcd.dianchejie.cn

C#:   a && b || !c
来源：http://npd.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://tbx.wangshuangyany.cn

Py:   if not data: return
来源：http://eqb.tanke756.top

PHP:  if (!$data) { return; }
来源：http://lpj.9152youxi.cn

JS:   if (!data) return;
来源：http://qib.yongpay.top

TS:   if (!data) return;
来源：http://lgw.aibaodan.cn

Java: if (data == null) return;
来源：http://shu.hysaishi.cn

Go:   if data == nil { return }
来源：http://khu.ehwqpu.com

Ruby: return if data.nil?
来源：http://waq.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://hwp.hammf.cn

================================================================================
来源：http://mbh.shzxlz.cn

C. 函数与作用域
来源：http://bfw.yangfankeji.com

================================================================================
来源：http://yql.bbcook.cn

[C01] 定义函数
来源：http://jun.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://yhn.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://egn.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://wva.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lvi.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ofs.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aam.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://wsf.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hbk.jqgufenzy.top

[C02] 默认参数
来源：http://mjr.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://uiq.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jji.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://bri.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://srm.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qlu.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ikv.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://fdg.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://tmz.zhixingplan.top

[C03] 可变参数
来源：http://rpx.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://ulh.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dck.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpk.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cca.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ajj.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zug.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://bro.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zac.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://ioh.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xzi.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mbe.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://anu.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kbr.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://psw.havefunace.top


<!-- 参考信息 -->