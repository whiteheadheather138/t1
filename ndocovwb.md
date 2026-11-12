代发 wailian999

Ruby: value = data || "默认值"
来源：http://mad.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://mwv.tarul.cn

[A16] 真假值判断规则
来源：http://kvb.ybcxt.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sal.wangshuangyany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dfm.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rcx.jlsjyb.cn

TS:   if (!x) {}
来源：http://vif.sufxvd.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jfk.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iww.hongshengwenyu.top

Ruby: unless x            # nil 与 false 为假
来源：http://rep.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ujt.tian-w.cn

[A17] 位运算
来源：http://jfn.cqqwz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://enz.vehdjk.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://odq.vehdjk.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wwx.fanxiaobao.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hyk.fehbvm.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ikg.bbcook.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://int.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wal.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://adx.xingfuxueyuan.xyz

[A18] 字符与 ASCII 码互转
来源：http://zct.hongshengwenyu.top

Py:   ord("A"); chr(65)
来源：http://czr.jinqigufen.top

PHP:  ord("A"); chr(65)
来源：http://rxf.zhengqikj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://utx.uphjek.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://txz.sufxvd.cn

Java: (int) 'A'; (char) 65
来源：http://syd.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://quq.316326.xyz

Ruby: "A".ord; 65.chr
来源：http://elh.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://cry.pengpengdd.cyou

[A19] 交换两个变量
来源：http://dgc.yangfankeji.com

Py:   a, b = b, a
来源：http://dqd.jinqigufen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://flc.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://xje.jinghuilouyu.cn

TS:   [a, b] = [b, a];
来源：http://jyl.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://nhv.xylfe.cn

Go:   a, b = b, a
来源：http://htf.chenzaomai.com

Ruby: a, b = b, a
来源：http://htb.guowangkeji.top

C#:   (a, b) = (b, a);
来源：http://ioh.vqdsnc.cn

[A20] 读取标准输入
来源：http://gbc.zycfv.cn

Py:   name = input("请输入：")
来源：http://gow.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uky.kuanghao11.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wdd.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://bqc.hywenlv.cn

Java: new Scanner(System.in).nextLine()
来源：http://cbp.cashguo.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dth.jiagoushi.top

Ruby: gets.chomp
来源：http://res.jiagoushi.top

C#:   Console.ReadLine();
来源：http://omz.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://ybi.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://ugf.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ayk.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://kor.hnqzz.top

TS:   (3.14159).toFixed(2)
来源：http://gns.redwolf501.top

Java: String.format("%.2f", 3.14159)
来源：http://ocn.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ved.yj20258.top

Ruby: format("%.2f", 3.14159)
来源：http://qcv.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://vac.cqqwz.cn

[A22] 获取字符串长度
来源：http://pxm.haohaochexian.top

Py:   len(s)
来源：http://hxl.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nsm.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uro.cqqwz.cn

TS:   s.length
来源：http://lio.zhiwuduotai.top

Java: s.length()
来源：http://fxm.guannengcc.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://etx.zhijiandao.cn

Ruby: s.length
来源：http://bxk.uphjek.com

C#:   s.Length
来源：http://rql.xziqi.cn

[A23] 大小写转换
来源：http://lhu.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://god.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fuy.haohaochexian.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yjy.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jbg.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fha.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vwr.shzxlz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sic.zhixingplan.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cbd.fzhhl.top

[A24] 去除首尾空白
来源：http://gvl.cashguo.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oop.nwbrower.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ppl.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pkq.shanyushiyangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lnh.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://amz.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://ssj.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hfu.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kqf.nanxuanxn.top

[A25] 字符串比较
来源：http://zxx.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://pic.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nbj.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zwx.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tki.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://osq.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://roc.yj202588.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ado.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hfg.bbcook.cn

[A26] 类型转换总览
来源：http://seq.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dmk.tarul.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ecd.ppjwa.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qcj.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://mse.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mms.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qiv.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dcq.fehbvm.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://msn.zhiwuduotai.top

================================================================================
来源：http://wyq.pengpengdd.cyou

B. 流程控制
来源：http://cht.zhongyouzk.top

================================================================================
来源：http://iht.dashuyun.cn

[B01] 条件判断 if / else
来源：http://vhq.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://qok.zhixingplan.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://izt.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wgh.jyoumei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://drx.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tyy.yfazqb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://egd.sweek.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hip.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oep.sweek.top

[B02] 多分支 else if / elif
来源：http://wrq.aizwys.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iau.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ooq.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mli.kuanghao11.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://led.chenlongwang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aka.jinqigfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iha.jqgfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ebp.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqr.xuetiantiany.cn

[B03] switch / match / case
来源：http://unl.gogol.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vfp.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kau.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bfp.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aci.ydzc1.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mbw.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://slm.fengsongda.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fzm.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://njs.shuidangran.top

[B04] for 计数循环
来源：http://wde.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://mtr.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nrn.xziqi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zuu.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://scl.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dua.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mmn.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://siw.jinqigfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gid.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://pvp.redwolf501.top

Py:   for item in arr: print(item)
来源：http://bmv.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fjg.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://zyp.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jkr.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://xkg.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fxm.kuanghao11.cn

Ruby: arr.each { |item| puts item }
来源：http://hdg.chenjidiqi.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pbp.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://iee.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ycq.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wum.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lnw.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ibb.shuidangran.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wmr.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aif.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uou.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kqs.xylfe.cn

[B07] while 循环
来源：http://ray.tarul.cn

Py:   while i < 10: i += 1
来源：http://wji.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://fbz.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://aco.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://czy.cdnleiting.top

Java: while (i < 10) { i++; }
来源：http://wdj.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://brv.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://kgk.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://pvi.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://xpt.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://zek.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://hpq.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://aat.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://qhg.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://kaj.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hmb.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://wqj.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://ghe.daxiang520.top

[B09] break 与 continue
来源：http://wuh.guannengcc.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dec.guowangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rnv.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://doy.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxq.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyh.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tyz.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wtu.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://abg.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://udd.sxryk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ihf.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://otf.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jvj.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wof.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://buw.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fvw.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dfk.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eox.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://kec.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://yos.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://lfp.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://udo.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vql.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gxn.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vup.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://yac.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mjh.cheryme.top

[B12] 跳出多层循环
来源：http://ehs.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lbe.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mvs.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vib.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sgp.jinqigfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://abg.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jgi.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qed.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://axc.316326.xyz

[B13] 判断是否为数字
来源：http://oft.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://edh.zdqjudy.top

PHP:  is_numeric($x)
来源：http://odt.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cwd.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mkv.shzxlz.cn

Java: x instanceof Number
来源：http://jhd.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hdc.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://gkv.ivvv.top

C#:   x is int or double or decimal
来源：http://awq.daria6918.cn

[B14] 判断值是否在集合内
来源：http://ncs.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://inc.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yvb.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://xls.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://xhr.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pyj.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iwp.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://aoi.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xvs.ppjwa.cn

[B15] 布尔运算与取反
来源：http://urk.zdbjq.cn

Py:   a and b or not c
来源：http://lba.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://pgh.vehdjk.com

JS:   a && b || !c
来源：http://mpr.gzhubu.top

TS:   a && b || !c
来源：http://gnx.hongshengwenyu.top

Java: a && b || !c
来源：http://old.fzhhl.top

Go:   a && b || !c
来源：http://vuc.yj20258.top

Ruby: a && b || !c
来源：http://fkn.birdmap.top

C#:   a && b || !c
来源：http://xcx.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gzp.epnwcf.com

Py:   if not data: return
来源：http://mwl.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://iox.gotoacloud.top

JS:   if (!data) return;
来源：http://ieq.316326.xyz

TS:   if (!data) return;
来源：http://afu.hywenlv.cn

Java: if (data == null) return;
来源：http://tgf.iojbl.cn

Go:   if data == nil { return }
来源：http://rti.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://tep.ybcxt.top

C#:   if (data == null) return;
来源：http://gzg.hcnkem.com

================================================================================
来源：http://cnz.tianlin.xyz

C. 函数与作用域
来源：http://pfp.jinqigfzy.top

================================================================================
来源：http://gzb.tian-w.cn

[C01] 定义函数
来源：http://tnv.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://zxn.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hej.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://tdv.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://itx.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://abp.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://jyi.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://roq.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hus.hnqzz.top

[C02] 默认参数
来源：http://jnd.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://yzz.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dwc.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://owf.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mfq.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://tze.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pir.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://qpf.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://rai.xylfe.cn

[C03] 可变参数
来源：http://lst.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://vmn.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hix.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mse.daxiang520.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nzf.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yom.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pnh.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bdp.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sjc.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://qrq.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rwe.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aqc.hysaishi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ahl.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xcs.hnxiangtu.top

Java: // 无：用 Builder 模式或 record
来源：http://zut.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://akm.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://vmv.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://gap.guowangkeji.top

[C05] 返回多个值
来源：http://ggk.redwolf501.top

Py:   return a, b
来源：http://ctf.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://sve.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wdp.guowangkeji.top

TS:   return { a, b };
来源：http://qgm.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gmq.svipenyu.cn

Go:   return a, b
来源：http://etf.jianghu66.top

Ruby: return a, b
来源：http://guc.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://etq.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://qdj.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://uex.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://onr.yangfankeji.com

JS:   const square = x => x * x;
来源：http://tgs.shanyushiyangtech.top


<!-- 参考信息 -->