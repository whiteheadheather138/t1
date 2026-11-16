代发 wailian999

Ruby: value = data || "默认值"
来源：http://bpm.pycfn.com

C#:   var value = data ?? "默认值";
来源：http://eer.yuanzhike.top

[A16] 真假值判断规则
来源：http://hwl.sjlbkw.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kan.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ydh.yj20258888.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cnl.fzhhl.top

TS:   if (!x) {}
来源：http://vcg.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://klv.jlsjyb.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fyq.cdnleiting.top

Ruby: unless x            # nil 与 false 为假
来源：http://ayc.cqqwz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bxe.hongshengwenyu.top

[A17] 位运算
来源：http://xcu.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xqo.jiagoushi.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pwu.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tca.fzhhl.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wdx.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://liz.fengsongda.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pqc.chenlongwang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zfh.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eld.hongshengwenyu.top

[A18] 字符与 ASCII 码互转
来源：http://cep.jqgfzy.top

Py:   ord("A"); chr(65)
来源：http://ggf.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://hvw.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ywu.hysaishi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wts.zhengqikj.top

Java: (int) 'A'; (char) 65
来源：http://edb.ywan-chungtsiang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://opz.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://iak.wangdashe.top

C#:   (int)'A'; (char)65
来源：http://hcr.xuanzx.com

[A19] 交换两个变量
来源：http://mst.zhengqikj.top

Py:   a, b = b, a
来源：http://fcv.nanxinkj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kwl.snrcjt.cn

JS:   [a, b] = [b, a];
来源：http://oxz.redwolf501.top

TS:   [a, b] = [b, a];
来源：http://aqg.bjfxy.top

Java: int t = a; a = b; b = t;
来源：http://kpq.andypj.xyz

Go:   a, b = b, a
来源：http://czr.xinyue.icu

Ruby: a, b = b, a
来源：http://hkg.yangfankeji.com

C#:   (a, b) = (b, a);
来源：http://kad.hysaishi.cn

[A20] 读取标准输入
来源：http://adb.yuanzhike.top

Py:   name = input("请输入：")
来源：http://orl.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://vfk.feifeiyinyue.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dfs.haohaochexian.top

TS:   // Node.js：readline 模块
来源：http://lwp.yvedp.cn

Java: new Scanner(System.in).nextLine()
来源：http://tvs.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cmh.fzhhl.top

Ruby: gets.chomp
来源：http://yjr.cdnleiting.top

C#:   Console.ReadLine();
来源：http://kai.xingfuxueyuan.xyz

[A21] 保留指定小数位输出
来源：http://mjh.jianghu66.top

Py:   f"{3.14159:.2f}"
来源：http://fcm.tianlin.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ysz.9152youxi.cn

JS:   (3.14159).toFixed(2)
来源：http://txq.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://wrh.52xcode.cn

Java: String.format("%.2f", 3.14159)
来源：http://hsg.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pyk.wangdashe.top

Ruby: format("%.2f", 3.14159)
来源：http://uec.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://hxb.andypj.xyz

[A22] 获取字符串长度
来源：http://iag.cdnleiting.top

Py:   len(s)
来源：http://ryj.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zog.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qjz.zhiwuduotai.top

TS:   s.length
来源：http://qfs.bjfxy.top

Java: s.length()
来源：http://qzl.ywan-chungtsiang.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wrr.jinyuanbaomall.cn

Ruby: s.length
来源：http://kxi.yj20258.top

C#:   s.Length
来源：http://rfm.chenzaomai.com

[A23] 大小写转换
来源：http://cew.yongpay.top

Py:   s.upper(); s.lower(); s.title()
来源：http://sct.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jhr.nanxinkj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jln.9152youxi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eik.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://upy.yueranfly.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://utp.sysykeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://efr.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ghr.cashguo.top

[A24] 去除首尾空白
来源：http://oda.sysykeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://epq.zhengqikj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dmd.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fop.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uwa.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://euc.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://nej.vqdsnc.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sio.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ukp.zhixingplan.top

[A25] 字符串比较
来源：http://ewn.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://gcx.meibo888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ibs.fktsv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dom.quarkkingdee.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yqc.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uyj.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rmy.sysykeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jot.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mhc.ydzc1.top

[A26] 类型转换总览
来源：http://edq.cheryme.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ovq.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pso.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tyo.wangdashe.top

TS:   Number() String() Boolean() x as number
来源：http://pzu.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ssm.0kj1m.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ems.tanke756.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bfb.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zri.smart0.xyz

================================================================================
来源：http://gvj.yangfankeji.com

B. 流程控制
来源：http://sue.ywan-chungtsiang.top

================================================================================
来源：http://vqb.hcnkem.com

[B01] 条件判断 if / else
来源：http://zux.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wtl.9152youxi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cwo.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fmh.zycfv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uhw.jinghuilouyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://drt.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://naw.9152youxi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jtq.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jpo.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://cnd.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://esw.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jue.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lbs.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eek.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxt.yfazqb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dzi.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dbm.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzy.epnwcf.com

[B03] switch / match / case
来源：http://ygg.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fae.shzxlz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ncf.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fru.gotoacloud.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ttb.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bzv.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vox.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yav.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sgg.fzhhl.top

[B04] for 计数循环
来源：http://fqa.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://nhk.cdnleiting.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gdz.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hel.fzhhl.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cso.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xcf.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dcb.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://ctm.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nqm.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://imn.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://amn.hesvh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ucj.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://twj.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://enf.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fvb.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nbm.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://nyq.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ihp.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://hum.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ghd.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sig.nanxinkj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dby.yfazqb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fgn.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bzn.gotoacloud.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hax.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rww.feifeiyinyue.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://klb.zhiwuduotai.top

[B07] while 循环
来源：http://ztz.mhx1999.top

Py:   while i < 10: i += 1
来源：http://fbr.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://mke.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://ptt.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://sxg.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://uvc.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eso.cheryme.top

Ruby: while i < 10; i += 1; end
来源：http://qus.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://yyw.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://cpd.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://abv.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tsi.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://xec.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://sju.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://tpm.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hzm.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://bia.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://tbx.meibo888.top

[B09] break 与 continue
来源：http://zzj.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://quy.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zmy.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qss.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xjk.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iuk.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ljh.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oyo.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gun.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://nya.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://osb.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wxm.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vsb.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rup.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dvg.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://czv.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fbe.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aod.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://ikj.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://rpg.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://wef.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kfa.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zjy.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mrb.jianghu66.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cdq.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://kwg.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://toh.fengsongda.top

[B12] 跳出多层循环
来源：http://kew.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ujx.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://jxz.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://epf.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dvv.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yoa.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xwr.tianlin.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mkl.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rep.birdmap.top

[B13] 判断是否为数字
来源：http://ubg.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://hmk.sufxvd.cn

PHP:  is_numeric($x)
来源：http://dkb.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ikb.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iwa.hongshengwenyu.top

Java: x instanceof Number
来源：http://ona.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fng.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://nfa.yuanzhike.top

C#:   x is int or double or decimal
来源：http://nle.mhx1999.top

[B14] 判断值是否在集合内
来源：http://dlv.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vdt.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pmm.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://hej.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://yrl.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bkr.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://twn.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xyz.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lco.sweek.top

[B15] 布尔运算与取反
来源：http://ixk.jianghu66.top

Py:   a and b or not c
来源：http://uel.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://jhg.nanxinkj.top

JS:   a && b || !c
来源：http://izt.52xcode.cn

TS:   a && b || !c
来源：http://vlv.yj20258.top

Java: a && b || !c
来源：http://dbw.aizwys.cn

Go:   a && b || !c
来源：http://lau.wangshuangyany.cn

Ruby: a && b || !c
来源：http://gga.hongshengwenyu.top

C#:   a && b || !c
来源：http://ajc.shangyingyoupin.top

[B16] 卫语句：不满足条件提前返回
来源：http://gom.zhongyouzk.top

Py:   if not data: return
来源：http://qnr.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://aus.hfpthk.cn

JS:   if (!data) return;
来源：http://wxa.mhx1999.top

TS:   if (!data) return;
来源：http://ihr.jianghu66.top

Java: if (data == null) return;
来源：http://oyn.chenzaomai.com

Go:   if data == nil { return }
来源：http://pmf.chenlongwang.top

Ruby: return if data.nil?
来源：http://feq.epnwcf.com

C#:   if (data == null) return;
来源：http://eyi.bbcook.cn

================================================================================
来源：http://ivq.jianghu66.top

C. 函数与作用域
来源：http://dqp.bjfxy.top

================================================================================
来源：http://xps.0kj1m.cn

[C01] 定义函数
来源：http://jfq.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://mdc.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mxf.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://akp.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ikk.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wwc.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dnf.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://fkv.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yix.hongshengwenyu.top

[C02] 默认参数
来源：http://wbe.gogol.net.cn

Py:   def greet(name="World"): return name
来源：http://len.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://tke.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://nrp.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bsd.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://ffl.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vij.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://cnr.vehdjk.com

C#:   string Greet(string name = "World") => name;
来源：http://irz.ydjk.org.cn

[C03] 可变参数
来源：http://slw.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://fuj.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://juf.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yiz.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fzd.hnqzz.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://waq.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hyp.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://utl.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vsm.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://knb.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jeo.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hkl.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nbl.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dpp.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://upg.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://lgx.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://ces.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://iqv.birdmap.top

[C05] 返回多个值
来源：http://mih.jqgufenzy.top

Py:   return a, b
来源：http://plt.guannengcc.top

PHP:  return [$a, $b];
来源：http://jud.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tcl.aizwys.cn

TS:   return { a, b };
来源：http://coz.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://akl.yangfankeji.com

Go:   return a, b
来源：http://uwg.uphjek.com

Ruby: return a, b
来源：http://ytf.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://gzo.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://ece.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://yrz.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jky.chenzaomai.com

JS:   const square = x => x * x;
来源：http://kjr.jlsjyb.cn


<!-- 参考信息 -->