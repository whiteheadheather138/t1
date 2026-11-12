代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://snp.zhaomingkeji.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kio.vqdsnc.cn

Go:   // 单行；/* 多行 */
来源：http://lld.yanxiufei.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gwr.fanxiaobao.xyz

C#:   // 单行；/* 多行 */
来源：http://fnk.jinghuilouyu.cn

[A15] 空值判断与默认值
来源：http://pfu.cdnleiting.top

Py:   value = data or "默认值"
来源：http://clr.yongpay.top

PHP:  $value = $data ?? "默认值";
来源：http://rxw.cqqwz.cn

JS:   const value = data ?? "默认值";
来源：http://qoy.yj20258.top

TS:   const value = data ?? "默认值";
来源：http://bkj.birdmap.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vcr.yuxming.cn

Go:   if data == "" { data = "默认值" }
来源：http://vdf.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://ouy.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://tvz.aibaodan.cn

[A16] 真假值判断规则
来源：http://bxj.iojbl.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://akx.chenjidiqi.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://var.chenlongwang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fel.fanxiaobao.xyz

TS:   if (!x) {}
来源：http://zhc.guannengcc.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ymt.zhixingplan.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tlc.chenlongwang.top

Ruby: unless x            # nil 与 false 为假
来源：http://bet.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nkl.pycfn.com

[A17] 位运算
来源：http://kig.dashuyun.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sxl.jianghu66.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://icc.ppjwa.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zpc.tianlin.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ryo.jinqigfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hum.fzhhl.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mvu.hcnkem.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wfu.yangfankeji.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jue.yj20258888.top

[A18] 字符与 ASCII 码互转
来源：http://fit.fktsv.cn

Py:   ord("A"); chr(65)
来源：http://qxz.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://xdn.birdmap.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://doi.haohaochexian.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yke.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://gqa.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kys.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://bcn.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://uzp.xziqi.cn

[A19] 交换两个变量
来源：http://evr.vqdsnc.cn

Py:   a, b = b, a
来源：http://wda.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zqz.redwolf501.top

JS:   [a, b] = [b, a];
来源：http://dao.tian-w.cn

TS:   [a, b] = [b, a];
来源：http://jnr.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://unw.smart0.xyz

Go:   a, b = b, a
来源：http://sde.tanke756.top

Ruby: a, b = b, a
来源：http://oqn.c1oappe.top

C#:   (a, b) = (b, a);
来源：http://ydx.ybcxt.top

[A20] 读取标准输入
来源：http://keb.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://auw.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ybi.ehwqpu.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://boa.zhijiandao.cn

TS:   // Node.js：readline 模块
来源：http://twr.xylfe.cn

Java: new Scanner(System.in).nextLine()
来源：http://lko.zhixingplan.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ije.yj20258888.top

Ruby: gets.chomp
来源：http://jzu.shanyushiyangtech.top

C#:   Console.ReadLine();
来源：http://xgl.xuanzx.com

[A21] 保留指定小数位输出
来源：http://wph.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://yww.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lsy.guowangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://pqw.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://ghq.ehwqpu.com

Java: String.format("%.2f", 3.14159)
来源：http://pdr.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wzw.tian-w.cn

Ruby: format("%.2f", 3.14159)
来源：http://azu.bjfxy.top

C#:   3.14159.ToString("F2")
来源：http://fod.yj20258.top

[A22] 获取字符串长度
来源：http://yam.xylfe.cn

Py:   len(s)
来源：http://ice.gaohongyu789.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eww.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://idx.epnwcf.com

TS:   s.length
来源：http://anq.jinyuanbaomall.cn

Java: s.length()
来源：http://gbn.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gos.pycfn.com

Ruby: s.length
来源：http://xif.fanxiaobao.xyz

C#:   s.Length
来源：http://pcv.yj202588.top

[A23] 大小写转换
来源：http://sjm.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://nfv.cheryme.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dbt.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tsc.52xcode.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kvw.xingfuxueyuan.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://okf.sxryk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://quk.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kwu.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://rxa.gaohongyu789.top

[A24] 去除首尾空白
来源：http://kkm.gzhubu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://quf.jinyuanbaomall.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rno.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vpa.zhixingplan.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lbd.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xeu.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://eqp.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ome.fanxiaobao.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ono.havefunace.top

[A25] 字符串比较
来源：http://tvk.bbcook.cn

Py:   s1 == s2; s1 != s2
来源：http://lbo.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wyx.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xuw.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ubm.tian-w.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nqu.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vpq.jqgfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pwf.ppjwa.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ljb.fengsongda.top

[A26] 类型转换总览
来源：http://kzz.jinghuilouyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xry.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://azf.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ycy.uphjek.com

TS:   Number() String() Boolean() x as number
来源：http://uxn.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yxt.fehbvm.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ocw.uphjek.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://fud.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jaa.chenlongwang.top

================================================================================
来源：http://rwq.gotoacloud.top

B. 流程控制
来源：http://yuy.yueranfly.top

================================================================================
来源：http://rwr.daria6918.cn

[B01] 条件判断 if / else
来源：http://sli.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bzy.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aky.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hgh.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jev.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ppi.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ima.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xgt.hywenlv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://skh.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://pup.ywan-chungtsiang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pnr.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qyq.pycfn.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pzy.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgu.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hwp.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nov.sweek.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pcx.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fsw.jinqigfzy.top

[B03] switch / match / case
来源：http://zgm.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fco.nanxinkj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://meh.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://krh.zhixingplan.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yey.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://izb.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rnk.xuanzx.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vtp.kuanghao11.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://elz.yvedp.cn

[B04] for 计数循环
来源：http://fwb.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://gbc.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cuf.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fgx.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yha.52xcode.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wcl.hnxiangtu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dld.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://nbe.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xgp.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://cfz.hammf.cn

Py:   for item in arr: print(item)
来源：http://qha.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pnn.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nvc.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jda.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://nrm.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xbl.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://ujh.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://una.pengpengdd.cyou

[B06] 遍历字典 / 对象
来源：http://jsx.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hrr.daria6918.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://spz.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kve.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gcr.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uit.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tov.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ifs.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eao.wangdashe.top

[B07] while 循环
来源：http://oqo.zycfv.cn

Py:   while i < 10: i += 1
来源：http://ilv.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://dei.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://gvx.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://zck.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://swq.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pzz.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://edi.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://hie.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://tcq.zhaomingkeji.xyz

Py:   # 无 do-while：用 while True + break
来源：http://tub.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://fik.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://cwc.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://mam.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://wix.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lbv.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://zfg.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://zjx.hammf.cn

[B09] break 与 continue
来源：http://pxf.daxiang520.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hfx.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nsj.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzm.jlsjyb.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbk.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tah.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vdp.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vgr.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pdt.bbcook.cn

[B10] 遍历同时拿索引
来源：http://mkv.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jya.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sgc.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ckl.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bhw.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qnn.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://off.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tkm.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nxh.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://fwo.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://cfg.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://wrp.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hkk.gaohongyu789.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://exr.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tgi.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ftq.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://faw.sxryk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eka.yvedp.cn

[B12] 跳出多层循环
来源：http://swr.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rvq.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bvs.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ixu.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nin.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wjj.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ucy.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uaz.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jjo.yueranfly.top

[B13] 判断是否为数字
来源：http://pby.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://ybe.hysaishi.cn

PHP:  is_numeric($x)
来源：http://qct.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zzf.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://voz.ehwqpu.com

Java: x instanceof Number
来源：http://lvx.yangfankeji.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bmm.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://pdp.zhengqikj.top

C#:   x is int or double or decimal
来源：http://bjm.sweek.top

[B14] 判断值是否在集合内
来源：http://ula.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ftc.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nak.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://eyy.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://dcf.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dvn.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pcg.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tln.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jhu.tianlin.xyz

[B15] 布尔运算与取反
来源：http://kpj.uphjek.com

Py:   a and b or not c
来源：http://cdb.52xcode.cn

PHP:  $a && $b || !$c
来源：http://bau.bjfxy.top

JS:   a && b || !c
来源：http://liq.andypj.xyz

TS:   a && b || !c
来源：http://vwf.hywenlv.cn

Java: a && b || !c
来源：http://hby.andypj.xyz

Go:   a && b || !c
来源：http://lrj.9152youxi.cn

Ruby: a && b || !c
来源：http://jec.zhiwuduotai.top

C#:   a && b || !c
来源：http://bkm.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ugl.zhengqikj.top

Py:   if not data: return
来源：http://lgb.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://jzj.zdqjudy.top

JS:   if (!data) return;
来源：http://aqy.pengpengdd.cyou

TS:   if (!data) return;
来源：http://qsm.cucudq.cn

Java: if (data == null) return;
来源：http://gaw.bbcook.cn

Go:   if data == nil { return }
来源：http://xnz.nanxinkj.top

Ruby: return if data.nil?
来源：http://bos.0kj1m.cn

C#:   if (data == null) return;
来源：http://ecq.sufxvd.cn

================================================================================
来源：http://ram.guowangkeji.top

C. 函数与作用域
来源：http://yhn.jianghu66.top

================================================================================
来源：http://cih.nanxinkj.top

[C01] 定义函数
来源：http://qyg.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://ovz.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eyj.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://iha.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odb.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://axj.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://gcs.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://pgo.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pwv.zhixingplan.top

[C02] 默认参数
来源：http://ezl.pycfn.com

Py:   def greet(name="World"): return name
来源：http://cvx.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lym.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://abu.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wkd.havefunace.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lsi.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bzf.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://vmx.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://sku.bjfxy.top

[C03] 可变参数
来源：http://muv.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://adu.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://asv.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bpd.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bkm.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yka.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sca.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://sox.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ckc.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://dlj.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zet.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ncx.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nck.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wjf.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://lta.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://xom.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://fyl.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://ife.shanyushiyangtech.top

[C05] 返回多个值
来源：http://dbl.tanke756.top


<!-- 参考信息 -->