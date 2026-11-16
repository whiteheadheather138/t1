代发 wailian999

[A14] 注释写法
来源：http://gkc.havefunace.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kvo.tianlin.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://gdy.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://iqj.guannengcc.top

TS:   // 单行；/* 多行 */
来源：http://vtg.smart0.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hxp.hcnkem.com

Go:   // 单行；/* 多行 */
来源：http://sev.haohaochexian.top

Ruby: # 单行；=begin 多行 =end
来源：http://cpa.daxiang520.top

C#:   // 单行；/* 多行 */
来源：http://biq.c1oappe.top

[A15] 空值判断与默认值
来源：http://kxq.zhoulong.xyz

Py:   value = data or "默认值"
来源：http://wts.yongpay.top

PHP:  $value = $data ?? "默认值";
来源：http://gpl.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://liw.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://njz.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://myi.zhiwuduotai.top

Go:   if data == "" { data = "默认值" }
来源：http://psp.zhijiandao.cn

Ruby: value = data || "默认值"
来源：http://nqh.hnqzz.top

C#:   var value = data ?? "默认值";
来源：http://jgq.aibaodan.cn

[A16] 真假值判断规则
来源：http://zhn.hesvh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nxs.yuxming.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ekj.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xyf.cashguo.top

TS:   if (!x) {}
来源：http://bci.sufxvd.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nil.316326.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tuf.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qeq.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ybg.shzxlz.cn

[A17] 位运算
来源：http://akn.zhongyouzk.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://imr.chenzaomai.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hrq.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hgq.ctjpmb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sng.birdmap.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eto.yuxming.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zto.xziqi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dop.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rsl.hysaishi.cn

[A18] 字符与 ASCII 码互转
来源：http://nnh.haohaochexian.top

Py:   ord("A"); chr(65)
来源：http://adj.guowangkeji.top

PHP:  ord("A"); chr(65)
来源：http://kjo.tarul.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hcf.fehbvm.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yzn.tarul.cn

Java: (int) 'A'; (char) 65
来源：http://jxx.fzhhl.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ukp.nwbrower.top

Ruby: "A".ord; 65.chr
来源：http://nov.9152youxi.cn

C#:   (int)'A'; (char)65
来源：http://hav.hysaishi.cn

[A19] 交换两个变量
来源：http://tzn.ydjk.org.cn

Py:   a, b = b, a
来源：http://hgi.aibaodan.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bdo.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://tqg.kuanghao11.cn

TS:   [a, b] = [b, a];
来源：http://jhg.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://sgv.fktsv.cn

Go:   a, b = b, a
来源：http://kuc.hcnkem.com

Ruby: a, b = b, a
来源：http://lnq.yuanzhike.top

C#:   (a, b) = (b, a);
来源：http://nxy.shanyushiyangkeji.top

[A20] 读取标准输入
来源：http://xqv.hongshengwenyu.top

Py:   name = input("请输入：")
来源：http://ucp.tanke756.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lsl.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://elk.hesvh.cn

TS:   // Node.js：readline 模块
来源：http://aji.yanxiufei.cn

Java: new Scanner(System.in).nextLine()
来源：http://ics.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vvb.sweek.top

Ruby: gets.chomp
来源：http://ygw.uphjek.com

C#:   Console.ReadLine();
来源：http://aug.daxiang520.top

[A21] 保留指定小数位输出
来源：http://reu.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://lcm.haohaochexian.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uxd.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://zoe.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://wmp.yangfankeji.com

Java: String.format("%.2f", 3.14159)
来源：http://bqz.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cpz.xuanzx.com

Ruby: format("%.2f", 3.14159)
来源：http://pph.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://bgy.meibo888.top

[A22] 获取字符串长度
来源：http://uvk.wangdashe.top

Py:   len(s)
来源：http://dmj.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sns.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dnw.gogol.net.cn

TS:   s.length
来源：http://zzf.cashguo.top

Java: s.length()
来源：http://dms.meibo888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ozo.chenjidiqi.icu

Ruby: s.length
来源：http://usb.shzxlz.cn

C#:   s.Length
来源：http://vrm.zhongyouzk.top

[A23] 大小写转换
来源：http://wqw.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://msg.sjlbkw.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ywy.snrcjt.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kri.shanyushiyangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vfb.gotoacloud.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ifr.yonumen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://etu.zhongyouzk.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ywc.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://ylh.pengpengdd.cyou

[A24] 去除首尾空白
来源：http://uzq.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ory.redwolf501.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://guj.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jsj.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://laj.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fcd.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://qvy.xingfuxueyuan.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wuw.cashguo.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ngq.yj20258.top

[A25] 字符串比较
来源：http://siz.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://lxs.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bah.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jan.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dge.xuanzx.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ukx.ywan-chungtsiang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lnj.yj202588.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xgg.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dga.haohaochexian.top

[A26] 类型转换总览
来源：http://sku.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zrh.nwbrower.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mrc.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://klc.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://wvq.vehdjk.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qnn.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qou.yj20258.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ofv.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oha.yonumen.top

================================================================================
来源：http://bej.yj202588.top

B. 流程控制
来源：http://avp.nanxinkj.top

================================================================================
来源：http://kvm.tanke756.top

[B01] 条件判断 if / else
来源：http://bov.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mdt.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nks.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://maz.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ulc.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://ibr.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rwr.pycfn.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zyd.ydzc1.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rsb.jianghu66.top

[B02] 多分支 else if / elif
来源：http://ksx.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tgh.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rse.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgh.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lgl.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oce.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xgs.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wkh.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ads.redwolf501.top

[B03] switch / match / case
来源：http://eok.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lul.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fof.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gql.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hog.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bto.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uxn.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kzv.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rso.snrcjt.cn

[B04] for 计数循环
来源：http://aql.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://lkn.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bep.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mip.yonumen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mxb.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eba.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wpr.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://pqz.nanxuanxn.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fmu.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://jwv.sxryk.cn

Py:   for item in arr: print(item)
来源：http://fyn.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qqu.fzhhl.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bvm.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://azx.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lxw.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ihx.ybcxt.top

Ruby: arr.each { |item| puts item }
来源：http://uqs.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vqm.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://map.jqgufenzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jvv.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jtv.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yid.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tkv.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mog.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lou.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cyw.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://prp.andypj.xyz

[B07] while 循环
来源：http://kdj.feifeiyinyue.top

Py:   while i < 10: i += 1
来源：http://tdx.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yxm.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://ovz.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://swi.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://khp.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jjy.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://tpp.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://bsu.birdmap.top

[B08] do-while（至少执行一次）
来源：http://dii.svipenyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://zmk.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dwb.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://qxi.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://cjx.xylfe.cn

Java: do { i++; } while (i < 10);
来源：http://eet.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qvi.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ooq.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://ozm.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://dik.dianchejie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://spi.jqgufenzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cqe.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgc.sjlbkw.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ead.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfq.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kwo.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vel.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewk.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://xqp.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wbk.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xcy.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jpm.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bdm.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rfd.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ibi.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bey.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hfe.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://ktx.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://dmn.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://upt.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mnb.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hlb.tarul.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://air.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tsr.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://pnh.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kub.ydjk.org.cn

[B12] 跳出多层循环
来源：http://kht.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uld.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qen.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sxd.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ivm.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sql.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://onk.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fff.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yro.9152youxi.cn

[B13] 判断是否为数字
来源：http://pft.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://zrc.aibaodan.cn

PHP:  is_numeric($x)
来源：http://tye.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dhg.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yib.hysaishi.cn

Java: x instanceof Number
来源：http://izb.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tka.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://pzp.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://dxw.yuxming.cn

[B14] 判断值是否在集合内
来源：http://feq.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ngw.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bpo.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://qtd.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://jew.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cei.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rkf.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dpw.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kcy.sxryk.cn

[B15] 布尔运算与取反
来源：http://hig.0kj1m.cn

Py:   a and b or not c
来源：http://apr.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://qtj.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://lbr.xuetiantiany.cn

TS:   a && b || !c
来源：http://pul.jinqigufen.top

Java: a && b || !c
来源：http://uhq.yangfankeji.com

Go:   a && b || !c
来源：http://zyc.fktsv.cn

Ruby: a && b || !c
来源：http://tus.chenzaomai.com

C#:   a && b || !c
来源：http://pyj.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://kea.zhaomingkeji.xyz

Py:   if not data: return
来源：http://xhl.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://owl.zhengqikj.top

JS:   if (!data) return;
来源：http://wjo.52xcode.cn

TS:   if (!data) return;
来源：http://urn.jianghu66.top

Java: if (data == null) return;
来源：http://lph.yj202588.top

Go:   if data == nil { return }
来源：http://xkz.hfpthk.cn

Ruby: return if data.nil?
来源：http://jfx.hesvh.cn

C#:   if (data == null) return;
来源：http://fkw.birdmap.top

================================================================================
来源：http://gxv.gogol.net.cn

C. 函数与作用域
来源：http://pmp.ehwqpu.com

================================================================================
来源：http://egm.tarul.cn

[C01] 定义函数
来源：http://usv.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://eyx.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xyc.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://xcs.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gdf.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hdi.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xhs.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://jxr.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xzy.ydzc1.top

[C02] 默认参数
来源：http://pqq.jyoumei.cn

Py:   def greet(name="World"): return name
来源：http://jvx.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lzg.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://yeg.shanyushiyangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hxi.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gcc.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://weg.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://yti.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://bth.nwbrower.top

[C03] 可变参数
来源：http://lkx.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://dbp.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dos.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aln.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dyr.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mem.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://asp.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://wnx.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hrb.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://dul.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dzs.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hog.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mat.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://egu.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://xpg.smart0.xyz


<!-- 参考信息 -->