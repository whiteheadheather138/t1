代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://mta.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qfh.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://gor.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wps.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://nmz.xinyue.icu

[A15] 空值判断与默认值
来源：http://vdt.daxiang520.top

Py:   value = data or "默认值"
来源：http://qre.nanxinkj.top

PHP:  $value = $data ?? "默认值";
来源：http://oiu.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://ofs.vqdsnc.cn

TS:   const value = data ?? "默认值";
来源：http://auv.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bnh.tarul.cn

Go:   if data == "" { data = "默认值" }
来源：http://nkp.yongpay.top

Ruby: value = data || "默认值"
来源：http://lqi.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://qul.jinqigufen.top

[A16] 真假值判断规则
来源：http://mxz.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bmd.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gby.yangfankeji.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://trc.xziqi.cn

TS:   if (!x) {}
来源：http://jdp.pycfn.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qgo.nanxuanxn.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hju.yanxiufei.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jue.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rsn.ydjk.org.cn

[A17] 位运算
来源：http://gfb.gzhubu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gli.ppjwa.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qon.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wxa.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pnu.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmq.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dub.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nto.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nbw.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://fhp.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://csd.fengsongda.top

PHP:  ord("A"); chr(65)
来源：http://bym.daxiang520.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xmx.zhixingplan.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gcu.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://whz.kuanghao11.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kaa.52xcode.cn

Ruby: "A".ord; 65.chr
来源：http://vlz.ydzc1.top

C#:   (int)'A'; (char)65
来源：http://wdh.sufxvd.cn

[A19] 交换两个变量
来源：http://xxv.xinyue.icu

Py:   a, b = b, a
来源：http://xhg.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cnv.yangfankeji.com

JS:   [a, b] = [b, a];
来源：http://seo.tian-w.cn

TS:   [a, b] = [b, a];
来源：http://tvg.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://cnu.tianlin.xyz

Go:   a, b = b, a
来源：http://hih.dianchejie.cn

Ruby: a, b = b, a
来源：http://azd.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://ufe.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://uqh.yj202588.top

Py:   name = input("请输入：")
来源：http://ipl.zhengqikj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://odl.quarkkingdee.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wvy.chenzaomai.com

TS:   // Node.js：readline 模块
来源：http://efy.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://xoe.daxiang520.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xpk.aibaodan.cn

Ruby: gets.chomp
来源：http://jbk.jqgfzy.top

C#:   Console.ReadLine();
来源：http://pzt.nwbrower.top

[A21] 保留指定小数位输出
来源：http://yao.jlsjyb.cn

Py:   f"{3.14159:.2f}"
来源：http://bsl.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gsj.aizwys.cn

JS:   (3.14159).toFixed(2)
来源：http://bwb.xylfe.cn

TS:   (3.14159).toFixed(2)
来源：http://wtb.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://diu.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yun.uphjek.com

Ruby: format("%.2f", 3.14159)
来源：http://rim.gogol.net.cn

C#:   3.14159.ToString("F2")
来源：http://wfr.316326.xyz

[A22] 获取字符串长度
来源：http://ktd.fanxiaobao.xyz

Py:   len(s)
来源：http://npm.jlsjyb.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fuh.shzxlz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://voo.haohaochexian.top

TS:   s.length
来源：http://wyv.yanxiufei.cn

Java: s.length()
来源：http://ylx.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://coc.zdqjudy.top

Ruby: s.length
来源：http://rcc.ybcxt.top

C#:   s.Length
来源：http://rva.ydzc1.top

[A23] 大小写转换
来源：http://vwh.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dpe.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rvf.bbcook.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jlj.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://soj.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://quw.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uab.hesvh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xvb.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fgi.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://mcx.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nbs.hcnkem.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gvw.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jxs.fehbvm.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oul.chenzaomai.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dwc.yj202588.top

Go:   strings.TrimSpace(s)
来源：http://hua.vehdjk.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ybs.ivvv.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ccm.nwbrower.top

[A25] 字符串比较
来源：http://eke.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://mbe.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jti.zdqjudy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tie.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sgu.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rwf.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wcn.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://ple.guannengcc.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mps.tianlin.xyz

[A26] 类型转换总览
来源：http://qxg.dianchejie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qog.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fes.yj20258.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cah.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://pga.sufxvd.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dwz.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iun.hesvh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mtl.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xsi.yfazqb.com

================================================================================
来源：http://kgg.guannengcc.top

B. 流程控制
来源：http://erb.9152youxi.cn

================================================================================
来源：http://paz.gzhubu.top

[B01] 条件判断 if / else
来源：http://ckw.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tiu.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://khk.jinghuilouyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lnd.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ani.gzhubu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hhp.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kor.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ead.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kez.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://kii.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kyr.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iao.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kma.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pqg.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vfw.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rtl.sufxvd.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vza.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qca.zhengqikj.top

[B03] switch / match / case
来源：http://ndi.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rqh.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qzw.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iaj.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jzy.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uom.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gzb.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ktt.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xao.svipenyu.cn

[B04] for 计数循环
来源：http://qgx.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://kvv.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lvp.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kny.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wib.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pqq.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vvl.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://czk.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ekx.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://nlo.hammf.cn

Py:   for item in arr: print(item)
来源：http://zhr.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aby.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lpg.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://xsy.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cmm.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vrn.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://wtk.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bqd.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://dkj.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://quu.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ock.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://raz.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wpu.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yxd.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jec.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kql.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://njz.dashuyun.cn

[B07] while 循环
来源：http://hyg.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://wrk.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://tbd.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://tqa.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://ple.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://ycx.52xcode.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dmh.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://oli.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://jxy.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://nhy.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://olt.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lwt.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://ygt.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://psd.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://nyr.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://blm.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mbb.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://cbg.nwbrower.top

[B09] break 与 continue
来源：http://lhz.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pwc.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dvs.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qrs.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqe.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://soe.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://myp.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zmm.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yuo.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://qdg.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ovu.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aac.cqqwz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xuv.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bak.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dvw.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xpw.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xwd.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hem.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://mbr.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://pkm.xuetiantiany.cn

PHP:  range(0, 10, 2);
来源：http://ngs.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://slk.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mdn.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ceg.jinqigfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ort.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://mwf.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uyi.gotoacloud.top

[B12] 跳出多层循环
来源：http://vbm.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lwc.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://mxb.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vbc.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jvi.fehbvm.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://umd.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ldf.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iih.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iwl.chenjidiqi.icu

[B13] 判断是否为数字
来源：http://cnf.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://luo.xziqi.cn

PHP:  is_numeric($x)
来源：http://qob.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qxg.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vos.mhx1999.top

Java: x instanceof Number
来源：http://vja.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uzn.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://mju.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://ucl.ybcxt.top

[B14] 判断值是否在集合内
来源：http://uoq.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qov.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qmg.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://rol.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://yyo.smart0.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://iov.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ltm.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://ykp.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ywn.hammf.cn

[B15] 布尔运算与取反
来源：http://gaq.cheryme.top

Py:   a and b or not c
来源：http://jhm.wangdashe.top

PHP:  $a && $b || !$c
来源：http://xzg.ehwqpu.com

JS:   a && b || !c
来源：http://gkm.vehdjk.com

TS:   a && b || !c
来源：http://sav.jiagoushi.top

Java: a && b || !c
来源：http://ssh.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://rxo.xylfe.cn

Ruby: a && b || !c
来源：http://cfp.dashuyun.cn

C#:   a && b || !c
来源：http://enj.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://enn.yuxming.cn

Py:   if not data: return
来源：http://mao.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://htg.fzhhl.top

JS:   if (!data) return;
来源：http://skk.birdmap.top

TS:   if (!data) return;
来源：http://cxc.wangshuangyany.cn

Java: if (data == null) return;
来源：http://vvx.zycfv.cn

Go:   if data == nil { return }
来源：http://zxs.dianchejie.cn

Ruby: return if data.nil?
来源：http://ksv.vehdjk.com

C#:   if (data == null) return;
来源：http://pwy.zhiwuduotai.top

================================================================================
来源：http://irt.kuanghao11.cn

C. 函数与作用域
来源：http://fac.tarul.cn

================================================================================
来源：http://fbp.jyoumei.cn

[C01] 定义函数
来源：http://aso.daria6918.cn

Py:   def add(a, b): return a + b
来源：http://ojh.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rsc.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://mnu.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://szj.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://reg.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://geq.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://vqc.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uxi.316326.xyz

[C02] 默认参数
来源：http://dbq.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://sju.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pif.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://qov.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zco.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hnv.sjlbkw.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hnw.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://dvd.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://myk.aizwys.cn

[C03] 可变参数
来源：http://qie.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://gsr.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yzl.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fun.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bqd.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wal.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hua.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vqq.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ndt.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://oou.sxryk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kfk.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wfe.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ild.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nyk.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://hiz.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://ugy.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://zyq.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://lgr.cucudq.cn

[C05] 返回多个值
来源：http://dvd.hongshengwenyu.top


<!-- 参考信息 -->