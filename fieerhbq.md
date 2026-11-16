代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://mix.nanxuanxn.top

TS:   const value = data ?? "默认值";
来源：http://bdc.hnqzz.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://thr.fzhhl.top

Go:   if data == "" { data = "默认值" }
来源：http://kaq.wangshuangyany.cn

Ruby: value = data || "默认值"
来源：http://qmd.c1oappe.top

C#:   var value = data ?? "默认值";
来源：http://jzm.jinqigfzy.top

[A16] 真假值判断规则
来源：http://rtg.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cez.vqdsnc.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ouc.sweek.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ttl.ydjk.org.cn

TS:   if (!x) {}
来源：http://mko.sjlbkw.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://slz.redwolf501.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rrj.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gud.hysaishi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eww.svipenyu.cn

[A17] 位运算
来源：http://byb.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qem.fanxiaobao.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ozi.aibaodan.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lny.9152youxi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://khn.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntf.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hgg.sysykeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xxp.52xcode.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ded.shuidangran.top

[A18] 字符与 ASCII 码互转
来源：http://qya.316326.xyz

Py:   ord("A"); chr(65)
来源：http://mmk.jlsjyb.cn

PHP:  ord("A"); chr(65)
来源：http://rxb.zdbjq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://odz.yonumen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vdq.quarkkingdee.top

Java: (int) 'A'; (char) 65
来源：http://bko.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uwy.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://dyn.fanxiaobao.xyz

C#:   (int)'A'; (char)65
来源：http://zti.ppjwa.cn

[A19] 交换两个变量
来源：http://zgl.nanxinkj.top

Py:   a, b = b, a
来源：http://qyd.cheryme.top

PHP:  [$a, $b] = [$b, $a];
来源：http://gdi.pengpengdd.cyou

JS:   [a, b] = [b, a];
来源：http://yjn.guowangkeji.top

TS:   [a, b] = [b, a];
来源：http://kik.yonumen.top

Java: int t = a; a = b; b = t;
来源：http://pyw.shanyushiyangtech.top

Go:   a, b = b, a
来源：http://hxo.sufxvd.cn

Ruby: a, b = b, a
来源：http://aqj.cashguo.top

C#:   (a, b) = (b, a);
来源：http://mjz.epnwcf.com

[A20] 读取标准输入
来源：http://zuc.snrcjt.cn

Py:   name = input("请输入：")
来源：http://svf.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mvp.yangfankeji.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jlc.c1oappe.top

TS:   // Node.js：readline 模块
来源：http://nza.feifeiyinyue.top

Java: new Scanner(System.in).nextLine()
来源：http://acz.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xiw.gaohongyu789.top

Ruby: gets.chomp
来源：http://zkr.zhaomingkeji.xyz

C#:   Console.ReadLine();
来源：http://vbt.316326.xyz

[A21] 保留指定小数位输出
来源：http://ajw.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://tiw.jinghuilouyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ofk.sufxvd.cn

JS:   (3.14159).toFixed(2)
来源：http://jgx.xinyue.icu

TS:   (3.14159).toFixed(2)
来源：http://hqc.wangdashe.top

Java: String.format("%.2f", 3.14159)
来源：http://ivj.tarul.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gju.fengsongda.top

Ruby: format("%.2f", 3.14159)
来源：http://cqh.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://vdm.ctjpmb.com

[A22] 获取字符串长度
来源：http://gfs.yuanzhike.top

Py:   len(s)
来源：http://eod.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://seg.xinyue.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://okg.havefunace.top

TS:   s.length
来源：http://gti.andypj.xyz

Java: s.length()
来源：http://rpk.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kss.zycfv.cn

Ruby: s.length
来源：http://opl.xylfe.cn

C#:   s.Length
来源：http://mbw.sysykeji.top

[A23] 大小写转换
来源：http://brg.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dpo.zhixingplan.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nry.yanxiufei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://frb.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jsb.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zex.pycfn.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gsb.epnwcf.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://agw.fehbvm.com

C#:   s.ToUpper(); s.ToLower()
来源：http://qxh.bjfxy.top

[A24] 去除首尾空白
来源：http://akb.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bgc.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wsb.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://suw.hysaishi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rjc.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qsm.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://unp.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jlu.hfpthk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xlf.haohaochexian.top

[A25] 字符串比较
来源：http://ppo.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://lwd.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://enp.sweek.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://goz.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lbl.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ktb.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://clh.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://law.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lum.daria6918.cn

[A26] 类型转换总览
来源：http://xeh.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yms.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cxq.xylfe.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ypn.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://jqd.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iol.ppjwa.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kaw.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rae.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qqm.hysaishi.cn

================================================================================
来源：http://bbw.zhaomingkeji.xyz

B. 流程控制
来源：http://adp.yangfankeji.com

================================================================================
来源：http://kbc.cashguo.top

[B01] 条件判断 if / else
来源：http://qux.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://teb.c1oappe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://psv.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://akl.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zuh.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://xhe.mhx1999.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://toc.ydjk.org.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fyl.fzhhl.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cnb.bbcook.cn

[B02] 多分支 else if / elif
来源：http://yku.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lzu.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zqs.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://asm.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jvd.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ffu.xuanzx.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wcs.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://grq.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wfe.xuetiantiany.cn

[B03] switch / match / case
来源：http://xwa.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eln.fanxiaobao.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jyc.aibaodan.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jhy.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fnr.yvedp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dfh.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ojx.316326.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wqa.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://twn.jiagoushi.top

[B04] for 计数循环
来源：http://ois.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://ril.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wrv.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://obo.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yxw.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ran.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ydv.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://oea.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kxe.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://sli.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://ndl.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://axg.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://pfk.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://guf.daxiang520.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pma.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nky.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://ogy.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hjr.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://bhh.haohaochexian.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cyg.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://otj.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wtz.bjfxy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gya.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cjw.gzhubu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zki.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bka.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lnd.cqqwz.cn

[B07] while 循环
来源：http://gai.sysykeji.top

Py:   while i < 10: i += 1
来源：http://sdq.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rfz.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://gtr.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://tji.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://pmy.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lcj.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://pos.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://gim.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://dgh.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://tma.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cha.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://jaz.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://zjj.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://zox.cashguo.top

Go:   for { i++; if i >= 10 { break } }
来源：http://sft.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://tlo.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://fte.yongpay.top

[B09] break 与 continue
来源：http://iag.hesvh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mni.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hjd.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igz.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tdf.fktsv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cph.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qvf.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yqh.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxg.vehdjk.com

[B10] 遍历同时拿索引
来源：http://hxx.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lqy.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bwl.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hzs.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fur.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uup.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nxs.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://der.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://upz.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://ihe.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://jfi.yongpay.top

PHP:  range(0, 10, 2);
来源：http://sxo.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://crm.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wts.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gey.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vgu.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://tnk.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nfm.ctjpmb.com

[B12] 跳出多层循环
来源：http://moy.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yws.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://odc.chenjidiqi.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jmr.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mmc.xziqi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lwn.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ejo.birdmap.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gql.zdbjq.cn

[B13] 判断是否为数字
来源：http://mem.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://mvr.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://mho.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ntx.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wfw.zhijiandao.cn

Java: x instanceof Number
来源：http://imm.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mvy.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://jgf.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://ohm.birdmap.top

[B14] 判断值是否在集合内
来源：http://mqv.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hyu.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sph.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://vvu.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://elq.jiagoushi.top

Java: List.of(1, 2, 3).contains(x)
来源：http://npa.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lgr.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kgq.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rdf.aibaodan.cn

[B15] 布尔运算与取反
来源：http://msh.xuetiantiany.cn

Py:   a and b or not c
来源：http://bwp.wangdashe.top

PHP:  $a && $b || !$c
来源：http://wsl.tian-w.cn

JS:   a && b || !c
来源：http://sme.feifeiyinyue.top

TS:   a && b || !c
来源：http://uyp.jinqigfzy.top

Java: a && b || !c
来源：http://vlo.smart0.xyz

Go:   a && b || !c
来源：http://ikv.jiagoushi.top

Ruby: a && b || !c
来源：http://qjc.jlsjyb.cn

C#:   a && b || !c
来源：http://hsd.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qyt.birdmap.top

Py:   if not data: return
来源：http://vix.uphjek.com

PHP:  if (!$data) { return; }
来源：http://ipn.ybcxt.top

JS:   if (!data) return;
来源：http://fit.shuidangran.top

TS:   if (!data) return;
来源：http://fuf.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://jlu.kuanghao11.cn

Go:   if data == nil { return }
来源：http://swp.yangfankeji.com

Ruby: return if data.nil?
来源：http://nbl.hnxiangtu.top

C#:   if (data == null) return;
来源：http://opd.yj20258888.top

================================================================================
来源：http://bji.52xcode.cn

C. 函数与作用域
来源：http://ieo.yanxiufei.cn

================================================================================
来源：http://wag.zhixingplan.top

[C01] 定义函数
来源：http://umq.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://cfd.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kbx.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://lvl.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://laf.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ras.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yig.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://udq.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gsz.daxiang520.top

[C02] 默认参数
来源：http://qkw.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://anv.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oce.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://see.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pvi.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yhy.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://onr.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://fuq.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://tzh.chenzaomai.com

[C03] 可变参数
来源：http://mdb.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://npp.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yid.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wcf.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yad.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qio.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pwh.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://dvv.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rft.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://wbw.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://skp.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rai.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qyl.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jko.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://fke.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://ped.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://dyc.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://sca.fanxiaobao.xyz

[C05] 返回多个值
来源：http://wal.dianchejie.cn

Py:   return a, b
来源：http://rmr.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://efr.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xle.shzxlz.cn

TS:   return { a, b };
来源：http://sao.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fqj.hongshengwenyu.top

Go:   return a, b
来源：http://osy.cashguo.top

Ruby: return a, b
来源：http://kyk.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://jrf.zhiwuduotai.top


<!-- 参考信息 -->