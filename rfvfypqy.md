代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fjj.cheryme.top

Ruby: unless x            # nil 与 false 为假
来源：http://oph.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mwl.yongpay.top

[A17] 位运算
来源：http://rkh.aibaodan.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://paa.shanyushiyangtech.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://azt.yueranfly.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yin.ppjwa.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ila.quarkkingdee.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yfl.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wjy.yonumen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://htp.gotoacloud.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hge.tianlin.xyz

[A18] 字符与 ASCII 码互转
来源：http://gfk.andypj.xyz

Py:   ord("A"); chr(65)
来源：http://ozn.nanxuanxn.top

PHP:  ord("A"); chr(65)
来源：http://yjc.zhixingplan.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gjk.ywan-chungtsiang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dcd.yongpay.top

Java: (int) 'A'; (char) 65
来源：http://saf.smart0.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gid.zhiwuduotai.top

Ruby: "A".ord; 65.chr
来源：http://klj.shuidangran.top

C#:   (int)'A'; (char)65
来源：http://ldn.hfpthk.cn

[A19] 交换两个变量
来源：http://onr.shzxlz.cn

Py:   a, b = b, a
来源：http://inj.svipenyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ijc.ivvv.top

JS:   [a, b] = [b, a];
来源：http://jxo.pengpengdd.cyou

TS:   [a, b] = [b, a];
来源：http://rho.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://wii.hcnkem.com

Go:   a, b = b, a
来源：http://ymw.snrcjt.cn

Ruby: a, b = b, a
来源：http://zqc.svipenyu.cn

C#:   (a, b) = (b, a);
来源：http://qva.chenlongwang.top

[A20] 读取标准输入
来源：http://vml.yueranfly.top

Py:   name = input("请输入：")
来源：http://lhe.uphjek.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ryb.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fvv.9152youxi.cn

TS:   // Node.js：readline 模块
来源：http://ybw.jinyuanbaomall.cn

Java: new Scanner(System.in).nextLine()
来源：http://xzg.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://epn.xylfe.cn

Ruby: gets.chomp
来源：http://tuw.jiagoushi.top

C#:   Console.ReadLine();
来源：http://anp.yvedp.cn

[A21] 保留指定小数位输出
来源：http://kwp.jinqigufen.top

Py:   f"{3.14159:.2f}"
来源：http://wli.tianlin.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ckx.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://pgs.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://rjx.meibo888.top

Java: String.format("%.2f", 3.14159)
来源：http://aaq.chenlongwang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://swb.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://umr.shzxlz.cn

C#:   3.14159.ToString("F2")
来源：http://mld.epnwcf.com

[A22] 获取字符串长度
来源：http://jgv.vehdjk.com

Py:   len(s)
来源：http://rkn.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wpg.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://obj.jinqigfzy.top

TS:   s.length
来源：http://wan.gotoacloud.top

Java: s.length()
来源：http://jig.52xcode.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xcq.redwolf501.top

Ruby: s.length
来源：http://lzi.feifeiyinyue.top

C#:   s.Length
来源：http://tln.jinqigfzy.top

[A23] 大小写转换
来源：http://ofw.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hct.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hpa.aibaodan.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wvk.gogol.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gyb.wangdashe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uwb.zhoulong.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kaw.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qqc.tianlin.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://vxn.jinqigufen.top

[A24] 去除首尾空白
来源：http://zkc.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ulo.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ncg.jianghu66.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ejj.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nav.hnqzz.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://izu.hnxiangtu.top

Go:   strings.TrimSpace(s)
来源：http://cte.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dbb.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xkc.xziqi.cn

[A25] 字符串比较
来源：http://gsq.zhixingplan.top

Py:   s1 == s2; s1 != s2
来源：http://fpp.zdbjq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://stx.tianlin.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://djr.jiagoushi.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ehb.chenlongwang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://apv.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://czb.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cdz.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lmg.mhx1999.top

[A26] 类型转换总览
来源：http://buk.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lkh.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://srq.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fwu.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://ecg.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vzu.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://abh.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://avf.ctjpmb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mhw.birdmap.top

================================================================================
来源：http://civ.0kj1m.cn

B. 流程控制
来源：http://yru.shzxlz.cn

================================================================================
来源：http://nct.iojbl.cn

[B01] 条件判断 if / else
来源：http://xww.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gjn.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://stj.epnwcf.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mpo.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://igq.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cos.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xot.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lzj.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mym.uphjek.com

[B02] 多分支 else if / elif
来源：http://jbn.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fav.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wgp.cucudq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oxb.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sgd.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fex.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ecj.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rzb.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yci.mhx1999.top

[B03] switch / match / case
来源：http://pcp.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vli.daxiang520.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iwi.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ydj.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wdm.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dux.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pzf.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kij.52xcode.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ayz.zhongyouzk.top

[B04] for 计数循环
来源：http://pen.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://hek.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wpz.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://haj.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wjl.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kew.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hyn.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://qsj.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kup.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://qwi.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://chp.tian-w.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ugr.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://pxx.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kjh.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://apd.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xxn.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://onn.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gcc.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://zuq.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://uxo.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ylb.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lsm.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://elr.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yrz.iojbl.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sni.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cuw.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fkh.hywenlv.cn

[B07] while 循环
来源：http://pgi.gzhubu.top

Py:   while i < 10: i += 1
来源：http://xoq.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://utc.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://atp.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://nnb.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://gee.yj20258.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tvv.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://ioq.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://lqc.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://siq.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://nzy.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cxm.jiagoushi.top

JS:   do { i++; } while (i < 10);
来源：http://eav.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://lwy.gzhubu.top

Java: do { i++; } while (i < 10);
来源：http://jye.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kwi.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://bmc.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://oqz.sweek.top

[B09] break 与 continue
来源：http://zhb.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://piv.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vvx.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acl.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svu.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://deg.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fsw.hysaishi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kax.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jfr.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://pxe.yonumen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zjo.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uxt.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vqo.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tey.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cqm.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mnk.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uzk.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qzu.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://yle.wangdashe.top

Py:   list(range(0, 10, 2))
来源：http://ofm.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://xzs.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zgs.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yon.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gcg.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dan.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://hqx.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://icc.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://klf.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://igt.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qlg.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kny.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://opp.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lnw.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jpc.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hyt.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ven.fehbvm.com

[B13] 判断是否为数字
来源：http://kfw.ybcxt.top

Py:   isinstance(x, (int, float))
来源：http://ulq.hcnkem.com

PHP:  is_numeric($x)
来源：http://jep.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hqg.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uvf.vqdsnc.cn

Java: x instanceof Number
来源：http://pkn.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jnk.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://dbt.hysaishi.cn

C#:   x is int or double or decimal
来源：http://qoi.0kj1m.cn

[B14] 判断值是否在集合内
来源：http://ffj.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://snw.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rlz.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://mpz.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://ijf.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cjn.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qnt.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://zhn.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uwe.cdnleiting.top

[B15] 布尔运算与取反
来源：http://zir.aizwys.cn

Py:   a and b or not c
来源：http://pas.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://evr.svipenyu.cn

JS:   a && b || !c
来源：http://vxs.yonumen.top

TS:   a && b || !c
来源：http://uzd.snrcjt.cn

Java: a && b || !c
来源：http://mmr.feifeiyinyue.top

Go:   a && b || !c
来源：http://cfj.shangyingyoupin.top

Ruby: a && b || !c
来源：http://grx.andypj.xyz

C#:   a && b || !c
来源：http://xvh.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hea.shangyingyoupin.top

Py:   if not data: return
来源：http://vhx.pycfn.com

PHP:  if (!$data) { return; }
来源：http://lit.zhongyouzk.top

JS:   if (!data) return;
来源：http://pwo.gaohongyu789.top

TS:   if (!data) return;
来源：http://ens.gzhubu.top

Java: if (data == null) return;
来源：http://mvr.bjfxy.top

Go:   if data == nil { return }
来源：http://hep.yfazqb.com

Ruby: return if data.nil?
来源：http://fck.fktsv.cn

C#:   if (data == null) return;
来源：http://lfn.chenzaomai.com

================================================================================
来源：http://tne.redwolf501.top

C. 函数与作用域
来源：http://wkn.hfpthk.cn

================================================================================
来源：http://gmr.shanyushiyangkeji.top

[C01] 定义函数
来源：http://uhi.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://rmw.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kdu.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://bev.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://six.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://vfz.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dai.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://fcj.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yrj.guowangkeji.top

[C02] 默认参数
来源：http://ajg.yongpay.top

Py:   def greet(name="World"): return name
来源：http://qip.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lyt.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://eda.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qyp.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gnu.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mwu.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://ymx.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://hmt.cashguo.top

[C03] 可变参数
来源：http://abb.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://ypt.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xxs.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://err.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eva.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zzo.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xoi.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dba.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nsp.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://ayz.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://had.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rlr.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://psi.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://idr.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://rzw.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://wxl.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://gfk.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://ont.316326.xyz

[C05] 返回多个值
来源：http://vlx.zhijiandao.cn

Py:   return a, b
来源：http://ohl.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://ndw.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://vsy.xylfe.cn

TS:   return { a, b };
来源：http://uac.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ixq.wangdashe.top

Go:   return a, b
来源：http://yic.ywan-chungtsiang.top

Ruby: return a, b
来源：http://qul.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://sge.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://ovt.xinyue.icu

Py:   square = lambda x: x * x
来源：http://gws.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ylf.svipenyu.cn

JS:   const square = x => x * x;
来源：http://tvw.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://vhi.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fmg.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://nmp.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://dnh.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://eeb.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://qvn.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mjq.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://qwd.chenjidiqi.icu


<!-- 参考信息 -->