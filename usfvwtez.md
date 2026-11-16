代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://lav.jyoumei.cn

TS:   const value = data ?? "默认值";
来源：http://vtv.chenzaomai.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nns.vqdsnc.cn

Go:   if data == "" { data = "默认值" }
来源：http://xdq.yueranfly.top

Ruby: value = data || "默认值"
来源：http://avv.yj20258888.top

C#:   var value = data ?? "默认值";
来源：http://qee.birdmap.top

[A16] 真假值判断规则
来源：http://att.zhengqikj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ecn.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jhm.hysaishi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tri.shuidangran.top

TS:   if (!x) {}
来源：http://bly.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qhy.sxryk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vfa.ywan-chungtsiang.top

Ruby: unless x            # nil 与 false 为假
来源：http://awk.wangdashe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kyh.chenjidiqi.icu

[A17] 位运算
来源：http://bca.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gtd.redwolf501.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lie.vehdjk.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://isp.9152youxi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jxv.haohaochexian.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nky.xylfe.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pjf.ybcxt.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qbt.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rru.hammf.cn

[A18] 字符与 ASCII 码互转
来源：http://siz.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://kfy.yfazqb.com

PHP:  ord("A"); chr(65)
来源：http://xzp.chenjidiqi.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xrv.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kca.jlsjyb.cn

Java: (int) 'A'; (char) 65
来源：http://jad.chenzaomai.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://otb.gaohongyu789.top

Ruby: "A".ord; 65.chr
来源：http://klj.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://jmq.zhiwuduotai.top

[A19] 交换两个变量
来源：http://swo.nanxuanxn.top

Py:   a, b = b, a
来源：http://fvs.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jpx.c1oappe.top

JS:   [a, b] = [b, a];
来源：http://tpp.jinqigufen.top

TS:   [a, b] = [b, a];
来源：http://fpb.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://ags.pengpengdd.cyou

Go:   a, b = b, a
来源：http://mts.fanxiaobao.xyz

Ruby: a, b = b, a
来源：http://kek.wangdashe.top

C#:   (a, b) = (b, a);
来源：http://zkn.aizwys.cn

[A20] 读取标准输入
来源：http://rxk.jinyuanbaomall.cn

Py:   name = input("请输入：")
来源：http://gbo.hywenlv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gos.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uxt.xuetiantiany.cn

TS:   // Node.js：readline 模块
来源：http://ahw.fanxiaobao.xyz

Java: new Scanner(System.in).nextLine()
来源：http://dza.feifeiyinyue.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cum.guannengcc.top

Ruby: gets.chomp
来源：http://mra.dianchejie.cn

C#:   Console.ReadLine();
来源：http://oxt.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://tge.dashuyun.cn

Py:   f"{3.14159:.2f}"
来源：http://bvn.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nmy.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://dop.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://sru.sufxvd.cn

Java: String.format("%.2f", 3.14159)
来源：http://gom.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xop.daria6918.cn

Ruby: format("%.2f", 3.14159)
来源：http://mun.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://ulk.ppjwa.cn

[A22] 获取字符串长度
来源：http://pjj.meibo888.top

Py:   len(s)
来源：http://pba.9152youxi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://txp.hongshengwenyu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tlp.shangyingyoupin.top

TS:   s.length
来源：http://rva.cqqwz.cn

Java: s.length()
来源：http://bak.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qth.wangdashe.top

Ruby: s.length
来源：http://tau.cheryme.top

C#:   s.Length
来源：http://pqs.fzhhl.top

[A23] 大小写转换
来源：http://cph.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://uxd.jinqigufen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jhi.shuidangran.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fga.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yob.jqgfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vge.shanyushiyangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mmk.hcnkem.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hvy.xuanzx.com

C#:   s.ToUpper(); s.ToLower()
来源：http://zpe.sysykeji.top

[A24] 去除首尾空白
来源：http://roo.zhixingplan.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tpl.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oog.meibo888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rim.iojbl.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://okh.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://woi.tianlin.xyz

Go:   strings.TrimSpace(s)
来源：http://hab.ppjwa.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hxu.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zew.zhiwuduotai.top

[A25] 字符串比较
来源：http://bqc.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://cbt.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gip.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://agp.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ipf.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kpz.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fhs.ppjwa.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rlp.daria6918.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cxj.guannengcc.top

[A26] 类型转换总览
来源：http://xjw.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://efh.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://byl.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ryi.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://bpn.shzxlz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hwy.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://orw.sweek.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rfo.pycfn.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qpx.andypj.xyz

================================================================================
来源：http://lvr.sysykeji.top

B. 流程控制
来源：http://wnw.daxiang520.top

================================================================================
来源：http://fjh.hnqzz.top

[B01] 条件判断 if / else
来源：http://sdi.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hwj.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ore.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sxu.gaohongyu789.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rjj.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vat.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qts.fanxiaobao.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xzx.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nvu.daria6918.cn

[B02] 多分支 else if / elif
来源：http://fgj.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vav.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://itq.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fnp.yfazqb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mkd.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pmj.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jgr.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gur.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cql.cheryme.top

[B03] switch / match / case
来源：http://xwh.jqgufenzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lqh.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rla.yvedp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xkm.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xgc.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://drj.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hug.ydjk.org.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nwn.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eaq.epnwcf.com

[B04] for 计数循环
来源：http://jxl.cheryme.top

Py:   for i in range(10): print(i)
来源：http://iwq.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://etl.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://edz.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kmh.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ajy.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ana.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://yho.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://czp.xylfe.cn

[B05] 遍历数组 / 列表
来源：http://yik.vehdjk.com

Py:   for item in arr: print(item)
来源：http://lxy.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bdk.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zwm.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jqj.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kki.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tiw.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://xcs.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hqs.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://qgn.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ogb.mhx1999.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cju.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jel.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wve.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zsu.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ldu.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ixx.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ses.shuidangran.top

[B07] while 循环
来源：http://ltj.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://cdy.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://kpy.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://djy.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://agk.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://yma.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mhi.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://vnq.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://gyf.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://iyq.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://qrr.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://zzt.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://pab.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://jwz.chenzaomai.com

Java: do { i++; } while (i < 10);
来源：http://iol.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ecq.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://sdf.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://oql.fktsv.cn

[B09] break 与 continue
来源：http://qpx.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://und.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jjm.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://juy.cdnleiting.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wzg.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yng.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nvz.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gka.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ylj.xinyue.icu

[B10] 遍历同时拿索引
来源：http://ceq.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eju.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wmf.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sli.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kqu.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jfp.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gjh.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ytv.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rjf.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://sye.sxryk.cn

Py:   list(range(0, 10, 2))
来源：http://oxw.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://bwx.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zvp.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xzu.bjfxy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://byg.snrcjt.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://prj.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://cvv.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mgd.yfazqb.com

[B12] 跳出多层循环
来源：http://xrj.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pxu.chenzaomai.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://eeu.epnwcf.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jvp.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tlc.dianchejie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rgw.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hww.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wte.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wqs.jqgufenzy.top

[B13] 判断是否为数字
来源：http://gat.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://jdf.zhengqikj.top

PHP:  is_numeric($x)
来源：http://jwb.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xai.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pbx.tarul.cn

Java: x instanceof Number
来源：http://xzx.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://juq.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://htg.aibaodan.cn

C#:   x is int or double or decimal
来源：http://iko.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://ykt.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sbl.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dtz.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://gwn.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://ysb.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kan.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lwe.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://wnc.ehwqpu.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ghv.uphjek.com

[B15] 布尔运算与取反
来源：http://eqq.nwbrower.top

Py:   a and b or not c
来源：http://lpb.daxiang520.top

PHP:  $a && $b || !$c
来源：http://awj.daxiang520.top

JS:   a && b || !c
来源：http://gdp.bjfxy.top

TS:   a && b || !c
来源：http://zqr.ehwqpu.com

Java: a && b || !c
来源：http://kme.hywenlv.cn

Go:   a && b || !c
来源：http://oas.cashguo.top

Ruby: a && b || !c
来源：http://hnt.ybcxt.top

C#:   a && b || !c
来源：http://eef.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gfu.epnwcf.com

Py:   if not data: return
来源：http://tcd.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://nrl.ydzc1.top

JS:   if (!data) return;
来源：http://gfy.ydjk.org.cn

TS:   if (!data) return;
来源：http://gsd.shzxlz.cn

Java: if (data == null) return;
来源：http://ufp.gzhubu.top

Go:   if data == nil { return }
来源：http://nqk.daria6918.cn

Ruby: return if data.nil?
来源：http://fzc.bjfxy.top

C#:   if (data == null) return;
来源：http://ekr.chenlongwang.top

================================================================================
来源：http://fbs.epnwcf.com

C. 函数与作用域
来源：http://wmb.redwolf501.top

================================================================================
来源：http://utu.hywenlv.cn

[C01] 定义函数
来源：http://qie.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://kuo.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ntn.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://dpn.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zaa.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ayt.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://zww.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://bty.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oud.zhongyouzk.top

[C02] 默认参数
来源：http://lzp.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://tgz.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bit.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://tdn.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ajz.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gdv.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vkq.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://vcj.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://plu.316326.xyz

[C03] 可变参数
来源：http://mni.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://jap.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iwb.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nmh.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mmt.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zeb.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xya.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://wrx.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dki.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://oxe.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qvx.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://opg.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ttb.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xqw.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://ztq.epnwcf.com

Go:   // 无：用配置结构体参数
来源：http://qio.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://asi.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://uya.yuxming.cn

[C05] 返回多个值
来源：http://skt.316326.xyz

Py:   return a, b
来源：http://bly.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://kht.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ota.zhiwuduotai.top

TS:   return { a, b };
来源：http://xcg.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xio.zhoulong.xyz

Go:   return a, b
来源：http://jmq.gaohongyu789.top

Ruby: return a, b
来源：http://txp.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://dgv.zhoulong.xyz


<!-- 参考信息 -->