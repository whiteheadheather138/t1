代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://faw.xuanzx.com

Ruby: unless x            # nil 与 false 为假
来源：http://rht.epnwcf.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nzi.fktsv.cn

[A17] 位运算
来源：http://khl.jiagoushi.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://teg.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jvr.c1oappe.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cmw.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rjc.pycfn.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rzb.jyoumei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wkc.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zyf.chenzaomai.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zhb.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://nzi.pycfn.com

Py:   ord("A"); chr(65)
来源：http://ibw.shzxlz.cn

PHP:  ord("A"); chr(65)
来源：http://dkr.ydjk.org.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jvz.fehbvm.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xgd.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://tjo.hcnkem.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jtp.daria6918.cn

Ruby: "A".ord; 65.chr
来源：http://nir.zdbjq.cn

C#:   (int)'A'; (char)65
来源：http://bvv.fengsongda.top

[A19] 交换两个变量
来源：http://zrh.daria6918.cn

Py:   a, b = b, a
来源：http://kxa.jinqigfzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fzh.shanyushiyangkeji.top

JS:   [a, b] = [b, a];
来源：http://yjz.xuetiantiany.cn

TS:   [a, b] = [b, a];
来源：http://jhd.zdbjq.cn

Java: int t = a; a = b; b = t;
来源：http://hgs.aibaodan.cn

Go:   a, b = b, a
来源：http://kfg.zhiwuduotai.top

Ruby: a, b = b, a
来源：http://fkb.ivvv.top

C#:   (a, b) = (b, a);
来源：http://grq.jqgfzy.top

[A20] 读取标准输入
来源：http://skj.redwolf501.top

Py:   name = input("请输入：")
来源：http://ayr.tanke756.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xqy.uphjek.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ymw.ydzc1.top

TS:   // Node.js：readline 模块
来源：http://rnn.c1oappe.top

Java: new Scanner(System.in).nextLine()
来源：http://hlt.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wft.hnxiangtu.top

Ruby: gets.chomp
来源：http://nsa.yonumen.top

C#:   Console.ReadLine();
来源：http://lvx.0kj1m.cn

[A21] 保留指定小数位输出
来源：http://wmr.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://znz.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fcf.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://vqg.chenzaomai.com

TS:   (3.14159).toFixed(2)
来源：http://abh.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://coz.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://apf.tanke756.top

Ruby: format("%.2f", 3.14159)
来源：http://paq.pycfn.com

C#:   3.14159.ToString("F2")
来源：http://xjq.zhongyouzk.top

[A22] 获取字符串长度
来源：http://uxs.0kj1m.cn

Py:   len(s)
来源：http://qxo.birdmap.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ote.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lzd.ybcxt.top

TS:   s.length
来源：http://vjb.shuidangran.top

Java: s.length()
来源：http://khh.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://agx.guannengcc.top

Ruby: s.length
来源：http://bzs.ybcxt.top

C#:   s.Length
来源：http://jeb.tanke756.top

[A23] 大小写转换
来源：http://emk.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gos.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qlz.cheryme.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ain.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pdn.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ojq.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vsf.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vxa.fzhhl.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dbr.yuxming.cn

[A24] 去除首尾空白
来源：http://yed.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lgv.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zog.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ewa.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jwf.zhixingplan.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mpb.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://vhu.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yds.52xcode.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ick.hnqzz.top

[A25] 字符串比较
来源：http://zgi.jinqigfzy.top

Py:   s1 == s2; s1 != s2
来源：http://nmp.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qcw.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fmq.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ylr.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rvj.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://orj.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uux.hysaishi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pft.zhiwuduotai.top

[A26] 类型转换总览
来源：http://rga.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ehx.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baw.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xex.vehdjk.com

TS:   Number() String() Boolean() x as number
来源：http://bze.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tcz.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://awd.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xnv.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eao.meibo888.top

================================================================================
来源：http://hyj.zhaomingkeji.xyz

B. 流程控制
来源：http://snf.zhixingplan.top

================================================================================
来源：http://jec.pycfn.com

[B01] 条件判断 if / else
来源：http://stg.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rit.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://esj.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jrb.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ojx.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://lmh.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hxh.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tqs.mhx1999.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bra.birdmap.top

[B02] 多分支 else if / elif
来源：http://www.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yvu.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cht.zdbjq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tyu.shanyushiyangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzz.redwolf501.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uuu.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hzg.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://duw.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mje.gotoacloud.top

[B03] switch / match / case
来源：http://lpb.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ygl.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://frx.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tvr.shzxlz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zbq.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://czn.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vii.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://brs.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fvo.feifeiyinyue.top

[B04] for 计数循环
来源：http://llp.tarul.cn

Py:   for i in range(10): print(i)
来源：http://vcb.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nqs.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pdb.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dvl.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kvl.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fql.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://aoq.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hec.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://feb.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://nrz.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://awm.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://son.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lfb.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://eop.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aue.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://nnj.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://urq.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://vxz.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://huy.fanxiaobao.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lim.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wro.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bbs.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sjk.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xgg.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rtn.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zwg.dianchejie.cn

[B07] while 循环
来源：http://tlf.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://gjh.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://syk.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://lod.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://opk.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://ihg.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zxm.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://pyh.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://bkc.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://rpq.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://dhm.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sto.jiagoushi.top

JS:   do { i++; } while (i < 10);
来源：http://dju.zhiwuduotai.top

TS:   do { i++; } while (i < 10);
来源：http://vlf.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://fld.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://txn.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://aow.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://liy.xziqi.cn

[B09] break 与 continue
来源：http://qsr.ctjpmb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hpc.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://isy.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yqt.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmg.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oum.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://avp.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kfb.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqi.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://xbx.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gfi.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://odq.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oft.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oxp.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dbi.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bdr.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nhj.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pbl.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://mki.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://svu.pycfn.com

PHP:  range(0, 10, 2);
来源：http://prm.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lvl.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ifh.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uuo.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wmv.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://fdv.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ikg.snrcjt.cn

[B12] 跳出多层循环
来源：http://rku.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uhi.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://agz.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bms.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oyr.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rxa.zdbjq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dsi.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sfz.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nxu.yvedp.cn

[B13] 判断是否为数字
来源：http://rhh.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://jxa.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://taq.dashuyun.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://agk.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hvi.pengpengdd.cyou

Java: x instanceof Number
来源：http://xty.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wqg.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://kip.gzhubu.top

C#:   x is int or double or decimal
来源：http://wka.hnqzz.top

[B14] 判断值是否在集合内
来源：http://hfs.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://krm.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lrb.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://tym.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://iut.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gsg.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lvo.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://juh.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zeh.shangyingyoupin.top

[B15] 布尔运算与取反
来源：http://vuy.svipenyu.cn

Py:   a and b or not c
来源：http://syb.52xcode.cn

PHP:  $a && $b || !$c
来源：http://wlr.wangshuangyany.cn

JS:   a && b || !c
来源：http://qql.316326.xyz

TS:   a && b || !c
来源：http://wwo.gzhubu.top

Java: a && b || !c
来源：http://mvn.nanxuanxn.top

Go:   a && b || !c
来源：http://cqw.jlsjyb.cn

Ruby: a && b || !c
来源：http://cjx.fzhhl.top

C#:   a && b || !c
来源：http://jfn.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://uas.tianlin.xyz

Py:   if not data: return
来源：http://cen.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://bui.iojbl.cn

JS:   if (!data) return;
来源：http://ctd.yueranfly.top

TS:   if (!data) return;
来源：http://ftf.havefunace.top

Java: if (data == null) return;
来源：http://bzg.zhixingplan.top

Go:   if data == nil { return }
来源：http://wtm.redwolf501.top

Ruby: return if data.nil?
来源：http://vta.c1oappe.top

C#:   if (data == null) return;
来源：http://ypz.ywan-chungtsiang.top

================================================================================
来源：http://ggx.cheryme.top

C. 函数与作用域
来源：http://yub.316326.xyz

================================================================================
来源：http://tlq.kuanghao11.cn

[C01] 定义函数
来源：http://kwa.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://asq.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oou.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://int.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sln.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tyo.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://fzq.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://bek.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fqa.shangyingyoupin.top

[C02] 默认参数
来源：http://idw.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://irn.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gwg.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://mex.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vlp.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ndb.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://slf.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://keo.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://lmk.wangshuangyany.cn

[C03] 可变参数
来源：http://xwn.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://edt.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ass.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqe.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://owo.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pqp.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cvs.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://sma.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jan.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://qbe.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nqg.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jlo.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fye.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ldm.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://uhy.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://xay.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://xay.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://xgu.fzhhl.top

[C05] 返回多个值
来源：http://lar.quarkkingdee.top

Py:   return a, b
来源：http://euq.zhengqikj.top

PHP:  return [$a, $b];
来源：http://zfa.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ibu.fehbvm.com

TS:   return { a, b };
来源：http://mwh.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hzt.daxiang520.top

Go:   return a, b
来源：http://qah.gaohongyu789.top

Ruby: return a, b
来源：http://eaz.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://dhg.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://itp.daria6918.cn

Py:   square = lambda x: x * x
来源：http://uza.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://hue.nanxinkj.top

JS:   const square = x => x * x;
来源：http://ocr.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://hyb.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rjs.zdbjq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qjc.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://oyu.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bbv.shzxlz.cn

[C07] 把函数作为参数传入
来源：http://qdh.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fbs.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://exa.epnwcf.com


<!-- 参考信息 -->