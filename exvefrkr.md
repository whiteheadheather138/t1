代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://vel.wangdashe.top

[A15] 空值判断与默认值
来源：http://vma.xinyue.icu

Py:   value = data or "默认值"
来源：http://dln.cdnleiting.top

PHP:  $value = $data ?? "默认值";
来源：http://vvz.jinqigufen.top

JS:   const value = data ?? "默认值";
来源：http://rxq.redwolf501.top

TS:   const value = data ?? "默认值";
来源：http://hms.wangshuangyany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kcw.sweek.top

Go:   if data == "" { data = "默认值" }
来源：http://kby.fengsongda.top

Ruby: value = data || "默认值"
来源：http://pah.bjfxy.top

C#:   var value = data ?? "默认值";
来源：http://wgr.0kj1m.cn

[A16] 真假值判断规则
来源：http://ctx.jianghu66.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eoc.yvedp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uqx.wangdashe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://knk.xingfuxueyuan.xyz

TS:   if (!x) {}
来源：http://qtx.316326.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lte.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eic.yvedp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jjr.mhx1999.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aov.yanxiufei.cn

[A17] 位运算
来源：http://jtp.guowangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kyi.tianlin.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yaz.52xcode.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vjn.bbcook.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fvj.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phd.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wxq.ybcxt.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vhk.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bmb.redwolf501.top

[A18] 字符与 ASCII 码互转
来源：http://cin.cucudq.cn

Py:   ord("A"); chr(65)
来源：http://gcw.birdmap.top

PHP:  ord("A"); chr(65)
来源：http://yqa.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qae.yongpay.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hax.gogol.net.cn

Java: (int) 'A'; (char) 65
来源：http://yzu.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lce.yj20258888.top

Ruby: "A".ord; 65.chr
来源：http://wfw.fktsv.cn

C#:   (int)'A'; (char)65
来源：http://wuy.jinqigfzy.top

[A19] 交换两个变量
来源：http://cqs.ybcxt.top

Py:   a, b = b, a
来源：http://lng.redwolf501.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ytz.cheryme.top

JS:   [a, b] = [b, a];
来源：http://ant.vqdsnc.cn

TS:   [a, b] = [b, a];
来源：http://rke.yfazqb.com

Java: int t = a; a = b; b = t;
来源：http://irh.yuxming.cn

Go:   a, b = b, a
来源：http://sau.zhoulong.xyz

Ruby: a, b = b, a
来源：http://pfl.fengsongda.top

C#:   (a, b) = (b, a);
来源：http://zsw.zhoulong.xyz

[A20] 读取标准输入
来源：http://ktj.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://buk.sxryk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bws.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://igj.xuanzx.com

TS:   // Node.js：readline 模块
来源：http://qay.hysaishi.cn

Java: new Scanner(System.in).nextLine()
来源：http://kzn.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cng.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://fln.hongshengwenyu.top

C#:   Console.ReadLine();
来源：http://qjj.ppjwa.cn

[A21] 保留指定小数位输出
来源：http://evy.hesvh.cn

Py:   f"{3.14159:.2f}"
来源：http://mdq.jyoumei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kcf.yj202588.top

JS:   (3.14159).toFixed(2)
来源：http://jkr.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://dzv.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://blk.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://twu.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://hwn.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://hjr.jinghuilouyu.cn

[A22] 获取字符串长度
来源：http://uiv.dashuyun.cn

Py:   len(s)
来源：http://xbp.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wwm.hammf.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lpm.kuanghao11.cn

TS:   s.length
来源：http://cuw.sxryk.cn

Java: s.length()
来源：http://ycc.bjfxy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kzm.tarul.cn

Ruby: s.length
来源：http://qwu.xuetiantiany.cn

C#:   s.Length
来源：http://ubr.fktsv.cn

[A23] 大小写转换
来源：http://gsw.zdqjudy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pak.hnqzz.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kxb.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xkg.gaohongyu789.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gxa.chenlongwang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dni.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dkr.yj20258888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rob.hywenlv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sym.shuidangran.top

[A24] 去除首尾空白
来源：http://apc.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hnk.chenlongwang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nzl.sweek.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pyv.gogol.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vkx.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pni.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://fvk.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lnq.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fzi.ybcxt.top

[A25] 字符串比较
来源：http://wxh.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://rdj.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vum.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wcn.hammf.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vvv.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ack.shangyingyoupin.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fbl.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wkd.feifeiyinyue.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ygd.aibaodan.cn

[A26] 类型转换总览
来源：http://cyx.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rpj.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://srg.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pzm.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://teb.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pxg.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jbe.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tll.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://enm.daxiang520.top

================================================================================
来源：http://piy.yj20258.top

B. 流程控制
来源：http://spm.svipenyu.cn

================================================================================
来源：http://lts.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://adn.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://lxl.birdmap.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fia.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fsd.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ggq.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://swk.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wwg.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jjb.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://apd.tanke756.top

[B02] 多分支 else if / elif
来源：http://hhr.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yum.hnxiangtu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wss.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dpl.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fpl.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ptl.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hyx.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://amm.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iaq.fktsv.cn

[B03] switch / match / case
来源：http://wfe.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lrh.zdqjudy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wqf.chenlongwang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xhl.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ogm.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://asg.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://okv.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wjy.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cvd.wangshuangyany.cn

[B04] for 计数循环
来源：http://tya.hnqzz.top

Py:   for i in range(10): print(i)
来源：http://gfy.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gdt.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iay.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mkd.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://udl.xylfe.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ihu.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://hom.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hij.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://cxt.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://piy.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gbp.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://piv.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://csl.guannengcc.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pmn.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://olt.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://ddt.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dxe.cheryme.top

[B06] 遍历字典 / 对象
来源：http://jsq.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fim.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://roh.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qpz.nanxinkj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://phd.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://klv.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mtc.fanxiaobao.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qjb.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jft.pengpengdd.cyou

[B07] while 循环
来源：http://yip.yongpay.top

Py:   while i < 10: i += 1
来源：http://idz.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://ilh.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://mfj.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://uwl.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://tci.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jyd.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://dwb.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://ujv.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://hvs.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://apb.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vis.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://ewh.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://qus.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://wwk.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sep.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://ygf.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://emz.yfazqb.com

[B09] break 与 continue
来源：http://nkv.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kvn.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wmg.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jrl.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blt.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvp.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qqh.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fpk.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ojw.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://moa.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pvr.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lkh.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://etq.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uxc.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qkn.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ypv.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bnq.tanke756.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tpd.sweek.top

[B11] 生成数字序列 / 区间
来源：http://cdf.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://anc.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://zja.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pbg.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lsu.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gfz.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hlw.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://yrl.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vce.iojbl.cn

[B12] 跳出多层循环
来源：http://ank.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oka.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qfh.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvg.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://klm.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ppe.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://frx.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pxt.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://inw.sysykeji.top

[B13] 判断是否为数字
来源：http://aly.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://bfz.yueranfly.top

PHP:  is_numeric($x)
来源：http://bcq.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yoh.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vtu.snrcjt.cn

Java: x instanceof Number
来源：http://xtg.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iwk.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://moi.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://eqi.jqgfzy.top

[B14] 判断值是否在集合内
来源：http://stm.guowangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jfk.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vln.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://pdn.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://xeo.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://kpo.yonumen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pwx.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yxb.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vbs.hammf.cn

[B15] 布尔运算与取反
来源：http://nei.cucudq.cn

Py:   a and b or not c
来源：http://niv.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://cvw.tarul.cn

JS:   a && b || !c
来源：http://crc.gaohongyu789.top

TS:   a && b || !c
来源：http://cci.uphjek.com

Java: a && b || !c
来源：http://oxs.zdqjudy.top

Go:   a && b || !c
来源：http://tyo.shuidangran.top

Ruby: a && b || !c
来源：http://weo.zhoulong.xyz

C#:   a && b || !c
来源：http://sbo.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jkf.tianlin.xyz

Py:   if not data: return
来源：http://qgd.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://wsv.chenjidiqi.icu

JS:   if (!data) return;
来源：http://awp.yj202588.top

TS:   if (!data) return;
来源：http://mse.dianchejie.cn

Java: if (data == null) return;
来源：http://tnf.meibo888.top

Go:   if data == nil { return }
来源：http://eeq.xziqi.cn

Ruby: return if data.nil?
来源：http://xvp.guannengcc.top

C#:   if (data == null) return;
来源：http://mrt.cqqwz.cn

================================================================================
来源：http://ixc.gotoacloud.top

C. 函数与作用域
来源：http://vxl.wangshuangyany.cn

================================================================================
来源：http://ddh.haohaochexian.top

[C01] 定义函数
来源：http://nmt.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://oou.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kye.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://qrw.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fac.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://npn.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://oow.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://jgg.gogol.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hjt.andypj.xyz

[C02] 默认参数
来源：http://xqq.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://ghv.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tst.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://uxf.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qij.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://qpw.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://exs.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://ybz.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://gvz.hfpthk.cn

[C03] 可变参数
来源：http://rmm.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://uvq.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hvn.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jcj.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ybs.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dyb.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eup.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://ruy.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kdn.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://ywb.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bcj.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vao.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://brh.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://syt.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://jyd.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://nxc.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://lvc.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://doh.cheryme.top

[C05] 返回多个值
来源：http://uug.hysaishi.cn

Py:   return a, b
来源：http://ima.guannengcc.top

PHP:  return [$a, $b];
来源：http://dnl.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xih.dianchejie.cn

TS:   return { a, b };
来源：http://jfq.xuanzx.com


<!-- 参考信息 -->