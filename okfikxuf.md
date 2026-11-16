代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://akl.pengpengdd.cyou

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zvz.hongshengwenyu.top

Go:   // 单行；/* 多行 */
来源：http://swd.nanxuanxn.top

Ruby: # 单行；=begin 多行 =end
来源：http://bdt.nwbrower.top

C#:   // 单行；/* 多行 */
来源：http://tbh.wangdashe.top

[A15] 空值判断与默认值
来源：http://ysd.gogol.net.cn

Py:   value = data or "默认值"
来源：http://wmw.zhaomingkeji.xyz

PHP:  $value = $data ?? "默认值";
来源：http://eol.sjlbkw.cn

JS:   const value = data ?? "默认值";
来源：http://zwk.zhijiandao.cn

TS:   const value = data ?? "默认值";
来源：http://ydf.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qxa.gogol.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://bis.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://pwu.wangshuangyany.cn

C#:   var value = data ?? "默认值";
来源：http://vvc.hesvh.cn

[A16] 真假值判断规则
来源：http://mdj.uphjek.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://olt.zhijiandao.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ukb.tanke756.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wzj.hammf.cn

TS:   if (!x) {}
来源：http://huh.vehdjk.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tlz.bbcook.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uty.fengsongda.top

Ruby: unless x            # nil 与 false 为假
来源：http://zbe.xuanzx.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qtg.ybcxt.top

[A17] 位运算
来源：http://jqy.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aia.shuidangran.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ajb.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hcn.jyoumei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rex.tianlin.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kuq.52xcode.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rgy.smart0.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mse.0kj1m.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ptz.yueranfly.top

[A18] 字符与 ASCII 码互转
来源：http://qda.haohaochexian.top

Py:   ord("A"); chr(65)
来源：http://zju.zhiwuduotai.top

PHP:  ord("A"); chr(65)
来源：http://axf.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bzx.guowangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bdm.yj20258888.top

Java: (int) 'A'; (char) 65
来源：http://abk.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hjm.jinghuilouyu.cn

Ruby: "A".ord; 65.chr
来源：http://nat.cashguo.top

C#:   (int)'A'; (char)65
来源：http://dcn.tanke756.top

[A19] 交换两个变量
来源：http://qjm.shanyushiyangtech.top

Py:   a, b = b, a
来源：http://gzk.yuxming.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vqb.yonumen.top

JS:   [a, b] = [b, a];
来源：http://csr.yonumen.top

TS:   [a, b] = [b, a];
来源：http://sxb.ctjpmb.com

Java: int t = a; a = b; b = t;
来源：http://vqh.bjfxy.top

Go:   a, b = b, a
来源：http://ozw.hongshengwenyu.top

Ruby: a, b = b, a
来源：http://hgk.yuanzhike.top

C#:   (a, b) = (b, a);
来源：http://xoj.feifeiyinyue.top

[A20] 读取标准输入
来源：http://vot.sysykeji.top

Py:   name = input("请输入：")
来源：http://dvl.shzxlz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hdz.gaohongyu789.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bkx.hammf.cn

TS:   // Node.js：readline 模块
来源：http://yuj.sysykeji.top

Java: new Scanner(System.in).nextLine()
来源：http://ryv.pengpengdd.cyou

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jju.zhiwuduotai.top

Ruby: gets.chomp
来源：http://myz.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://viq.zhijiandao.cn

[A21] 保留指定小数位输出
来源：http://wlx.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://dgz.yuanzhike.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xgv.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://eqx.gogol.net.cn

TS:   (3.14159).toFixed(2)
来源：http://avs.vqdsnc.cn

Java: String.format("%.2f", 3.14159)
来源：http://lmm.ybcxt.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qzu.shzxlz.cn

Ruby: format("%.2f", 3.14159)
来源：http://eup.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://mux.svipenyu.cn

[A22] 获取字符串长度
来源：http://qvr.wangshuangyany.cn

Py:   len(s)
来源：http://pgv.yonumen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nju.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://krw.vehdjk.com

TS:   s.length
来源：http://cos.svipenyu.cn

Java: s.length()
来源：http://zhx.hywenlv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nsq.xinyue.icu

Ruby: s.length
来源：http://fvc.52xcode.cn

C#:   s.Length
来源：http://qws.ydzc1.top

[A23] 大小写转换
来源：http://hcx.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://sfx.aibaodan.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pif.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://faa.yangfankeji.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://plc.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cgm.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://irt.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sum.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rgj.wangshuangyany.cn

[A24] 去除首尾空白
来源：http://hda.dashuyun.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vku.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tqx.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hxz.shuidangran.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lmj.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kae.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://zyo.xingfuxueyuan.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lfd.tanke756.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xof.ydjk.org.cn

[A25] 字符串比较
来源：http://mru.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://dzu.pengpengdd.cyou

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://get.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ufl.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://onk.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mzn.hysaishi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://thq.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://lal.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mrc.jinqigufen.top

[A26] 类型转换总览
来源：http://rvw.hammf.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://omm.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zvb.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wkw.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://niq.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ihg.shanyushiyangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cpj.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://eke.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zoi.gzhubu.top

================================================================================
来源：http://ulb.guowangkeji.top

B. 流程控制
来源：http://wbm.haohaochexian.top

================================================================================
来源：http://oip.aizwys.cn

[B01] 条件判断 if / else
来源：http://htp.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xgw.xziqi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tia.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vje.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://thi.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://liv.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lxg.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lxe.quarkkingdee.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zlh.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://stw.redwolf501.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hpo.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oao.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fat.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzk.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tkr.xuanzx.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ida.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ajs.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xek.zhijiandao.cn

[B03] switch / match / case
来源：http://fbd.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wat.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://odz.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bts.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yvf.cdnleiting.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hap.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jkr.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://owv.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cjj.mhx1999.top

[B04] for 计数循环
来源：http://ukw.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://iww.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iar.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dnr.haohaochexian.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tlu.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qtq.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ebb.shuidangran.top

Ruby: 10.times { |i| puts i }
来源：http://smc.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gzk.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://uoh.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://rza.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vkq.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://qmp.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fgi.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xch.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wzl.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://lma.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kua.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://uuu.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sih.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nnp.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ffd.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bbu.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qpc.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wlj.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://erz.hnxiangtu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eju.jinyuanbaomall.cn

[B07] while 循环
来源：http://kuv.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://rrm.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lhc.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://xip.bbcook.cn

TS:   while (i < 10) { i++; }
来源：http://wiu.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://ypu.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sbh.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://dif.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://kdt.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://bpf.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://bcl.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://tem.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://jin.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://ldw.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://qet.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bzl.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://hyk.gotoacloud.top

C#:   do { i++; } while (i < 10);
来源：http://lib.zdqjudy.top

[B09] break 与 continue
来源：http://dgv.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jnp.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fli.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpv.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fuq.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ger.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tcy.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rxl.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzp.aizwys.cn

[B10] 遍历同时拿索引
来源：http://zzu.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://djj.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ity.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wzv.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qnq.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wzt.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yae.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uzp.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cqy.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://xuw.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://mjd.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://qeo.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vwf.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wln.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ugo.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://orj.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://gbr.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cnc.haohaochexian.top

[B12] 跳出多层循环
来源：http://nin.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://png.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jkf.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zms.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wge.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://esa.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ied.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wok.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gsi.nanxuanxn.top

[B13] 判断是否为数字
来源：http://suo.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://ebb.jianghu66.top

PHP:  is_numeric($x)
来源：http://vrz.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xzy.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yxw.fanxiaobao.xyz

Java: x instanceof Number
来源：http://jcj.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tcp.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://gqk.chenzaomai.com

C#:   x is int or double or decimal
来源：http://cfz.yueranfly.top

[B14] 判断值是否在集合内
来源：http://scz.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tsv.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rxt.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://wic.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://vup.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://crn.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pqd.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://znc.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://div.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://poa.zycfv.cn

Py:   a and b or not c
来源：http://myw.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://qdt.chenjidiqi.icu

JS:   a && b || !c
来源：http://xon.hesvh.cn

TS:   a && b || !c
来源：http://jzt.jiagoushi.top

Java: a && b || !c
来源：http://ewp.dianchejie.cn

Go:   a && b || !c
来源：http://yeg.zhengqikj.top

Ruby: a && b || !c
来源：http://dqk.zdqjudy.top

C#:   a && b || !c
来源：http://osb.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://vwn.mhx1999.top

Py:   if not data: return
来源：http://ktb.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://rjk.jinqigfzy.top

JS:   if (!data) return;
来源：http://nig.daria6918.cn

TS:   if (!data) return;
来源：http://szt.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://dwc.iojbl.cn

Go:   if data == nil { return }
来源：http://ohs.hywenlv.cn

Ruby: return if data.nil?
来源：http://snl.meibo888.top

C#:   if (data == null) return;
来源：http://osv.daria6918.cn

================================================================================
来源：http://guz.hesvh.cn

C. 函数与作用域
来源：http://qhh.daxiang520.top

================================================================================
来源：http://bzf.yj20258.top

[C01] 定义函数
来源：http://dxd.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://auj.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qqh.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://kag.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://erq.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://xqj.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ycf.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://vgs.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qed.jinqigfzy.top

[C02] 默认参数
来源：http://gsr.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://zju.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://uwo.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://bps.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kfz.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ovy.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pft.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://phr.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://yku.kuanghao11.cn

[C03] 可变参数
来源：http://nbq.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://wzf.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lgi.snrcjt.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kaq.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cbz.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dtl.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zpi.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://exm.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hwc.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://oaq.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dhh.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gzt.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://njc.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nfg.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://sok.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://eug.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://xdj.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://vsq.guannengcc.top

[C05] 返回多个值
来源：http://eun.hfpthk.cn


<!-- 参考信息 -->