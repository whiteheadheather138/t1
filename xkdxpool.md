代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mmt.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://ksy.vehdjk.com

C#:   $"Hello, {name}!"
来源：http://rmm.zdqjudy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xhh.shanyushiyangtech.top

Py:   "第一行\n第二行"
来源：http://avd.ehwqpu.com

PHP:  "第一行\n第二行"
来源：http://ype.sjlbkw.cn

JS:   "第一行\n第二行"
来源：http://cvr.jinyuanbaomall.cn

TS:   "第一行\n第二行"
来源：http://vlt.jinqigfzy.top

Java: "第一行\n第二行"
来源：http://veg.nanxuanxn.top

Go:   "第一行\n第二行"
来源：http://vgh.yanxiufei.cn

Ruby: "第一行\n第二行"
来源：http://agg.daxiang520.top

C#:   "第一行\n第二行"
来源：http://smj.sweek.top

[A14] 注释写法
来源：http://sry.jyoumei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://aws.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://elw.xingfuxueyuan.xyz

JS:   // 单行；/* 多行 */
来源：http://nxr.nanxinkj.top

TS:   // 单行；/* 多行 */
来源：http://jtq.tarul.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mbc.jiagoushi.top

Go:   // 单行；/* 多行 */
来源：http://hao.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://esy.xingfuxueyuan.xyz

C#:   // 单行；/* 多行 */
来源：http://ovs.cdnleiting.top

[A15] 空值判断与默认值
来源：http://zxu.yuxming.cn

Py:   value = data or "默认值"
来源：http://ffx.yongpay.top

PHP:  $value = $data ?? "默认值";
来源：http://dxz.chenjidiqi.icu

JS:   const value = data ?? "默认值";
来源：http://vua.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://zhb.pengpengdd.cyou

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iuq.epnwcf.com

Go:   if data == "" { data = "默认值" }
来源：http://xlp.mhx1999.top

Ruby: value = data || "默认值"
来源：http://xdm.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://ijf.yanxiufei.cn

[A16] 真假值判断规则
来源：http://nmo.9152youxi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bfx.shanyushiyangtech.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fky.gogol.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rgc.ydzc1.top

TS:   if (!x) {}
来源：http://wyb.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jxm.jiagoushi.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ecc.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nhd.cashguo.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bve.fanxiaobao.xyz

[A17] 位运算
来源：http://yta.hywenlv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://edo.nwbrower.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://asw.chenzaomai.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwc.shangyingyoupin.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pis.uphjek.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ovs.yanxiufei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ubd.zhixingplan.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cps.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hfr.gzhubu.top

[A18] 字符与 ASCII 码互转
来源：http://cfr.gotoacloud.top

Py:   ord("A"); chr(65)
来源：http://esc.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://kew.gotoacloud.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://owq.ehwqpu.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lzx.vehdjk.com

Java: (int) 'A'; (char) 65
来源：http://dnr.hesvh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xhc.gaohongyu789.top

Ruby: "A".ord; 65.chr
来源：http://aub.ppjwa.cn

C#:   (int)'A'; (char)65
来源：http://xnm.yfazqb.com

[A19] 交换两个变量
来源：http://xfb.snrcjt.cn

Py:   a, b = b, a
来源：http://txy.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ney.hnxiangtu.top

JS:   [a, b] = [b, a];
来源：http://asw.pengpengdd.cyou

TS:   [a, b] = [b, a];
来源：http://qnk.sysykeji.top

Java: int t = a; a = b; b = t;
来源：http://crt.ppjwa.cn

Go:   a, b = b, a
来源：http://glh.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://ulj.9152youxi.cn

C#:   (a, b) = (b, a);
来源：http://tne.jlsjyb.cn

[A20] 读取标准输入
来源：http://uew.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://iat.gogol.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dfa.xuanzx.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://axh.shanyushiyangkeji.top

TS:   // Node.js：readline 模块
来源：http://pvu.yj20258.top

Java: new Scanner(System.in).nextLine()
来源：http://deh.jinqigufen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lne.nanxuanxn.top

Ruby: gets.chomp
来源：http://syp.haohaochexian.top

C#:   Console.ReadLine();
来源：http://her.sjlbkw.cn

[A21] 保留指定小数位输出
来源：http://ifd.jlsjyb.cn

Py:   f"{3.14159:.2f}"
来源：http://yqr.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://icv.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://cyp.tarul.cn

TS:   (3.14159).toFixed(2)
来源：http://ozs.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://ekk.jinqigufen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://syd.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://eya.cheryme.top

C#:   3.14159.ToString("F2")
来源：http://jwd.wangdashe.top

[A22] 获取字符串长度
来源：http://bfw.zhiwuduotai.top

Py:   len(s)
来源：http://upj.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tvc.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zoc.pycfn.com

TS:   s.length
来源：http://mfv.haohaochexian.top

Java: s.length()
来源：http://kdj.ybcxt.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sfk.andypj.xyz

Ruby: s.length
来源：http://gfu.epnwcf.com

C#:   s.Length
来源：http://rnx.yfazqb.com

[A23] 大小写转换
来源：http://qkc.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://cfh.yuxming.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kcd.yj20258888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aqx.zhiwuduotai.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ysm.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rkq.hongshengwenyu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://egv.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://swo.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wqy.jqgufenzy.top

[A24] 去除首尾空白
来源：http://uyn.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nmd.yonumen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://had.cheryme.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fwl.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jsc.jqgfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pzl.hammf.cn

Go:   strings.TrimSpace(s)
来源：http://zft.yj202588.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vpw.ybcxt.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eiu.jinyuanbaomall.cn

[A25] 字符串比较
来源：http://cxk.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://zky.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://czr.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rjk.sjlbkw.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hac.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rzb.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cni.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jsm.xuetiantiany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mug.ctjpmb.com

[A26] 类型转换总览
来源：http://ufh.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vib.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://khw.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://typ.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://egj.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pih.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xzv.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xtl.tarul.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xkk.yongpay.top

================================================================================
来源：http://zml.316326.xyz

B. 流程控制
来源：http://qwh.sufxvd.cn

================================================================================
来源：http://nbx.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://liv.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qgc.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jlw.pengpengdd.cyou

JS:   const r = x > 0 ? "正" : "非正";
来源：http://icj.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hms.yonumen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zwx.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ixv.cashguo.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zdj.cqqwz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xgk.wangshuangyany.cn

[B02] 多分支 else if / elif
来源：http://yfe.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://frh.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dwi.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kjd.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://afg.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ntw.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eae.316326.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cyb.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmk.vehdjk.com

[B03] switch / match / case
来源：http://nto.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pxi.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xws.cheryme.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://elx.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ait.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://znu.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rua.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qiq.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vxw.smart0.xyz

[B04] for 计数循环
来源：http://set.zhixingplan.top

Py:   for i in range(10): print(i)
来源：http://ant.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tol.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ekh.sweek.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://avd.xuetiantiany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://upr.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rvo.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://wmw.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://skt.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://hgy.jianghu66.top

Py:   for item in arr: print(item)
来源：http://vbb.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ycx.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dnp.yongpay.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ecr.ydjk.org.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dni.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kwg.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://fte.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gwh.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://wgi.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ksx.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vqy.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bep.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rbv.uphjek.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://okw.xinyue.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tnz.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iap.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bvg.ydjk.org.cn

[B07] while 循环
来源：http://fdt.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://ogj.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ksh.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://cvl.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://oqf.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://try.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://igd.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://loj.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://fmm.jianghu66.top

[B08] do-while（至少执行一次）
来源：http://pht.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://tca.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kok.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://opd.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://kek.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://woo.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sjo.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://hkf.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://npz.aibaodan.cn

[B09] break 与 continue
来源：http://buw.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qom.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wej.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jrc.wangdashe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsh.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bgd.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mfo.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yhk.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lit.316326.xyz

[B10] 遍历同时拿索引
来源：http://ijc.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://djb.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iqi.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kbi.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jgv.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lsy.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rzm.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ekf.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bxi.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://ywy.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://anj.yvedp.cn

PHP:  range(0, 10, 2);
来源：http://tlp.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gyy.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yws.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wvc.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zro.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://axf.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://clq.cheryme.top

[B12] 跳出多层循环
来源：http://wjs.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dfe.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://mww.xingfuxueyuan.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tqv.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zge.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://exz.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qkh.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wcj.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vzo.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://tek.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://ouw.gzhubu.top

PHP:  is_numeric($x)
来源：http://ber.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pbc.9152youxi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ooh.zdbjq.cn

Java: x instanceof Number
来源：http://tgt.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mnn.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://kxu.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://qbi.wangdashe.top

[B14] 判断值是否在集合内
来源：http://mcq.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qey.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zfu.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://foh.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://tyx.gotoacloud.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xwc.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nwk.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://dca.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cif.iojbl.cn

[B15] 布尔运算与取反
来源：http://unq.xylfe.cn

Py:   a and b or not c
来源：http://jnp.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://kdr.havefunace.top

JS:   a && b || !c
来源：http://pno.52xcode.cn

TS:   a && b || !c
来源：http://oyz.yvedp.cn

Java: a && b || !c
来源：http://ktb.tian-w.cn

Go:   a && b || !c
来源：http://oww.fktsv.cn

Ruby: a && b || !c
来源：http://eqc.ctjpmb.com

C#:   a && b || !c
来源：http://git.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dff.hcnkem.com

Py:   if not data: return
来源：http://fjk.pycfn.com

PHP:  if (!$data) { return; }
来源：http://tpk.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://hqg.jqgfzy.top

TS:   if (!data) return;
来源：http://qza.pycfn.com

Java: if (data == null) return;
来源：http://lib.sufxvd.cn

Go:   if data == nil { return }
来源：http://xit.zhongyouzk.top

Ruby: return if data.nil?
来源：http://sqx.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://nne.cdnleiting.top

================================================================================
来源：http://mqm.yvedp.cn

C. 函数与作用域
来源：http://qyi.pengpengdd.cyou

================================================================================
来源：http://zas.cheryme.top

[C01] 定义函数
来源：http://tdg.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://dri.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hik.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://juc.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zkh.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://twi.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://keq.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://pdf.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iib.zhiwuduotai.top

[C02] 默认参数
来源：http://lob.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://kvs.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hsn.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://xcf.fanxiaobao.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://vwo.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://doq.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vuq.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://ngn.zhengqikj.top

C#:   string Greet(string name = "World") => name;
来源：http://nou.hnqzz.top

[C03] 可变参数
来源：http://cyk.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://sfn.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tjn.sweek.top


<!-- 参考信息 -->