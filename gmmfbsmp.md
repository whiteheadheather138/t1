代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://sle.epnwcf.com

[A15] 空值判断与默认值
来源：http://eiq.shzxlz.cn

Py:   value = data or "默认值"
来源：http://hgj.yj20258.top

PHP:  $value = $data ?? "默认值";
来源：http://hya.shuidangran.top

JS:   const value = data ?? "默认值";
来源：http://hec.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://rik.tanke756.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tnr.hnxiangtu.top

Go:   if data == "" { data = "默认值" }
来源：http://dkp.yj202588.top

Ruby: value = data || "默认值"
来源：http://jwa.sjlbkw.cn

C#:   var value = data ?? "默认值";
来源：http://bvc.fengsongda.top

[A16] 真假值判断规则
来源：http://gis.xuetiantiany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tzx.cheryme.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rir.pengpengdd.cyou

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ykz.chenlongwang.top

TS:   if (!x) {}
来源：http://vzp.xingfuxueyuan.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xnk.jlsjyb.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gzu.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://hwa.chenlongwang.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ebv.cdnleiting.top

[A17] 位运算
来源：http://lmd.9152youxi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rhv.yanxiufei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kfk.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rii.yvedp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://umc.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vku.uphjek.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qcl.zhaomingkeji.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tcj.fzhhl.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vxa.fengsongda.top

[A18] 字符与 ASCII 码互转
来源：http://fco.sysykeji.top

Py:   ord("A"); chr(65)
来源：http://pnr.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://lta.shanyushiyangtech.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zfz.uphjek.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://unp.jlsjyb.cn

Java: (int) 'A'; (char) 65
来源：http://xwx.cashguo.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aii.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://wpe.epnwcf.com

C#:   (int)'A'; (char)65
来源：http://lto.bbcook.cn

[A19] 交换两个变量
来源：http://foo.vehdjk.com

Py:   a, b = b, a
来源：http://unn.jyoumei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://imb.vehdjk.com

JS:   [a, b] = [b, a];
来源：http://thd.jinghuilouyu.cn

TS:   [a, b] = [b, a];
来源：http://kmu.daxiang520.top

Java: int t = a; a = b; b = t;
来源：http://vee.guannengcc.top

Go:   a, b = b, a
来源：http://iyw.gogol.net.cn

Ruby: a, b = b, a
来源：http://zph.tianlin.xyz

C#:   (a, b) = (b, a);
来源：http://pln.yvedp.cn

[A20] 读取标准输入
来源：http://pjp.chenlongwang.top

Py:   name = input("请输入：")
来源：http://xkj.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rpi.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wrv.shuidangran.top

TS:   // Node.js：readline 模块
来源：http://pna.fanxiaobao.xyz

Java: new Scanner(System.in).nextLine()
来源：http://zyd.cqqwz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://djk.nwbrower.top

Ruby: gets.chomp
来源：http://usm.ppjwa.cn

C#:   Console.ReadLine();
来源：http://sir.cashguo.top

[A21] 保留指定小数位输出
来源：http://zum.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://rut.ivvv.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lro.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://xfw.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://bvb.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://ltm.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mgp.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://joq.birdmap.top

C#:   3.14159.ToString("F2")
来源：http://fdr.pycfn.com

[A22] 获取字符串长度
来源：http://pms.nwbrower.top

Py:   len(s)
来源：http://vct.shanyushiyangtech.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://omh.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qjo.chenjidiqi.icu

TS:   s.length
来源：http://scs.jyoumei.cn

Java: s.length()
来源：http://xys.jlsjyb.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qtj.redwolf501.top

Ruby: s.length
来源：http://wqv.meibo888.top

C#:   s.Length
来源：http://xui.shangyingyoupin.top

[A23] 大小写转换
来源：http://yst.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://evg.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ilp.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fqa.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oea.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mzr.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ssa.nwbrower.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://myr.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lsq.sufxvd.cn

[A24] 去除首尾空白
来源：http://tqo.zycfv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sma.aibaodan.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ghj.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ryw.snrcjt.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rru.9152youxi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aue.hywenlv.cn

Go:   strings.TrimSpace(s)
来源：http://bwh.chenjidiqi.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aqz.tianlin.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pod.wangdashe.top

[A25] 字符串比较
来源：http://ymi.wangdashe.top

Py:   s1 == s2; s1 != s2
来源：http://fxg.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://srw.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jzk.yvedp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qty.yongpay.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vtw.shangyingyoupin.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zmy.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uds.sjlbkw.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qso.fzhhl.top

[A26] 类型转换总览
来源：http://nss.yfazqb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uds.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cjj.vqdsnc.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aoi.9152youxi.cn

TS:   Number() String() Boolean() x as number
来源：http://ilu.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jyg.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://egw.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wtn.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wtt.wangshuangyany.cn

================================================================================
来源：http://zrm.vqdsnc.cn

B. 流程控制
来源：http://zrz.bjfxy.top

================================================================================
来源：http://xkp.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://ovl.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wuw.wangdashe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oma.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://btg.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hps.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fjn.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gky.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qly.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ndv.9152youxi.cn

[B02] 多分支 else if / elif
来源：http://gqu.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fhr.xuanzx.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://god.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ynd.kuanghao11.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfs.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://per.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://soa.hesvh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yym.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gkc.tarul.cn

[B03] switch / match / case
来源：http://bjz.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bck.shuidangran.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kvu.ppjwa.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cml.hcnkem.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yjp.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vlp.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tjj.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jwh.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jpz.yanxiufei.cn

[B04] for 计数循环
来源：http://wzw.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://ies.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ulv.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fex.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bnd.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tcr.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kam.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://kks.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qoq.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://ulg.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://zcs.jiagoushi.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://imk.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zso.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dkk.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zhr.ydjk.org.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wtx.shuidangran.top

Ruby: arr.each { |item| puts item }
来源：http://uvx.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://duk.xuanzx.com

[B06] 遍历字典 / 对象
来源：http://ywa.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xiy.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://koo.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lvx.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://brn.wangshuangyany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lal.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qwk.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tor.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iyi.aibaodan.cn

[B07] while 循环
来源：http://qvv.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://imw.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ncd.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://ykq.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://tbh.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://qcx.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mxr.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://syp.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://kej.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://mgy.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://xyn.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xeq.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://wsp.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://osc.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://xnf.gaohongyu789.top

Go:   for { i++; if i >= 10 { break } }
来源：http://njr.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://zvd.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://agm.zhijiandao.cn

[B09] break 与 continue
来源：http://hwm.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gqn.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nbo.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kky.quarkkingdee.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mzk.dashuyun.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mvi.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://woz.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qnr.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vcn.yfazqb.com

[B10] 遍历同时拿索引
来源：http://qxg.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://buo.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://agy.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://num.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pkb.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ljx.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://irl.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fgj.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nit.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://rnw.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://xbg.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://uzv.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lrl.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ryg.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ynk.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ibr.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://wak.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xji.hfpthk.cn

[B12] 跳出多层循环
来源：http://tou.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://inq.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vxl.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kny.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cjn.wangdashe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qii.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fxx.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://unq.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lco.sxryk.cn

[B13] 判断是否为数字
来源：http://dzw.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://tgb.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://oqp.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xii.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nnn.xuanzx.com

Java: x instanceof Number
来源：http://zsk.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://was.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://ntj.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://ncp.bbcook.cn

[B14] 判断值是否在集合内
来源：http://qhj.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nyg.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://psf.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://phx.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://mwf.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://pso.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hih.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://idm.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wta.ctjpmb.com

[B15] 布尔运算与取反
来源：http://uxl.c1oappe.top

Py:   a and b or not c
来源：http://aue.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://cnu.sweek.top

JS:   a && b || !c
来源：http://qna.bbcook.cn

TS:   a && b || !c
来源：http://skj.jianghu66.top

Java: a && b || !c
来源：http://mck.daxiang520.top

Go:   a && b || !c
来源：http://wpx.yangfankeji.com

Ruby: a && b || !c
来源：http://bzc.fktsv.cn

C#:   a && b || !c
来源：http://gvk.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://wci.fehbvm.com

Py:   if not data: return
来源：http://hyf.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://woz.sxryk.cn

JS:   if (!data) return;
来源：http://vjj.fehbvm.com

TS:   if (!data) return;
来源：http://ntg.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://egn.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://ybz.9152youxi.cn

Ruby: return if data.nil?
来源：http://nod.jiagoushi.top

C#:   if (data == null) return;
来源：http://jum.hammf.cn

================================================================================
来源：http://mkp.havefunace.top

C. 函数与作用域
来源：http://fza.cqqwz.cn

================================================================================
来源：http://rvm.svipenyu.cn

[C01] 定义函数
来源：http://kjk.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://tvh.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wjx.shangyingyoupin.top

JS:   function add(a, b) { return a + b; }
来源：http://drk.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://okt.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://xnr.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://znj.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://hqj.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rbj.c1oappe.top

[C02] 默认参数
来源：http://klz.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://tom.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ztq.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://mcv.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lyw.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://upp.xuetiantiany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cak.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://emj.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://cta.shanyushiyangkeji.top

[C03] 可变参数
来源：http://ucj.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://wmo.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uzd.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://caq.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kdm.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mko.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ytl.chenlongwang.top

Ruby: def total(*nums); nums.sum; end
来源：http://rdb.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://haa.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://yvk.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://evt.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aye.nanxuanxn.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jzl.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rrh.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://fnx.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://qlm.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://tpt.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://rck.jyoumei.cn

[C05] 返回多个值
来源：http://ixb.haohaochexian.top

Py:   return a, b
来源：http://jqt.guowangkeji.top

PHP:  return [$a, $b];
来源：http://bfi.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://enw.zycfv.cn

TS:   return { a, b };
来源：http://tum.fktsv.cn


<!-- 参考信息 -->