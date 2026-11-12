代发 wailian999

Java: "第一行\n第二行"
来源：http://btc.yanxiufei.cn

Go:   "第一行\n第二行"
来源：http://mny.yongpay.top

Ruby: "第一行\n第二行"
来源：http://vmv.zycfv.cn

C#:   "第一行\n第二行"
来源：http://rba.meibo888.top

[A14] 注释写法
来源：http://ari.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wsh.bbcook.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://eoo.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://xpw.wangdashe.top

TS:   // 单行；/* 多行 */
来源：http://kwd.nanxinkj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zym.hammf.cn

Go:   // 单行；/* 多行 */
来源：http://ziw.epnwcf.com

Ruby: # 单行；=begin 多行 =end
来源：http://ote.guannengcc.top

C#:   // 单行；/* 多行 */
来源：http://ukk.gogol.net.cn

[A15] 空值判断与默认值
来源：http://pzy.shanyushiyangtech.top

Py:   value = data or "默认值"
来源：http://ffg.fzhhl.top

PHP:  $value = $data ?? "默认值";
来源：http://tcv.yj202588.top

JS:   const value = data ?? "默认值";
来源：http://zxm.xylfe.cn

TS:   const value = data ?? "默认值";
来源：http://ehm.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kbp.guowangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://jfo.iojbl.cn

Ruby: value = data || "默认值"
来源：http://tgi.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://mvq.feifeiyinyue.top

[A16] 真假值判断规则
来源：http://ous.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rav.hammf.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fxn.chenlongwang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dit.cashguo.top

TS:   if (!x) {}
来源：http://lrj.nanxuanxn.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ija.shanyushiyangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sxb.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cki.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jut.hfpthk.cn

[A17] 位运算
来源：http://nac.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ufe.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://get.ybcxt.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ebf.chenjidiqi.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jiu.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bgd.jyoumei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aph.vehdjk.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lci.sxryk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jpm.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://hdo.chenjidiqi.icu

Py:   ord("A"); chr(65)
来源：http://wuo.ivvv.top

PHP:  ord("A"); chr(65)
来源：http://nam.gzhubu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ezf.iojbl.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://flg.shzxlz.cn

Java: (int) 'A'; (char) 65
来源：http://plp.hywenlv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mxa.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://evn.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://cqe.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://sps.gaohongyu789.top

Py:   a, b = b, a
来源：http://fqv.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jal.zhengqikj.top

JS:   [a, b] = [b, a];
来源：http://ipp.bjfxy.top

TS:   [a, b] = [b, a];
来源：http://quc.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://gsq.xingfuxueyuan.xyz

Go:   a, b = b, a
来源：http://utx.svipenyu.cn

Ruby: a, b = b, a
来源：http://xhm.wangdashe.top

C#:   (a, b) = (b, a);
来源：http://wnv.quarkkingdee.top

[A20] 读取标准输入
来源：http://gco.pycfn.com

Py:   name = input("请输入：")
来源：http://uhy.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bci.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hqb.tian-w.cn

TS:   // Node.js：readline 模块
来源：http://zpb.cheryme.top

Java: new Scanner(System.in).nextLine()
来源：http://exg.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://prg.tianlin.xyz

Ruby: gets.chomp
来源：http://isj.aizwys.cn

C#:   Console.ReadLine();
来源：http://kvs.fanxiaobao.xyz

[A21] 保留指定小数位输出
来源：http://pnf.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://rfu.yfazqb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sgg.yvedp.cn

JS:   (3.14159).toFixed(2)
来源：http://mrc.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://rih.jiagoushi.top

Java: String.format("%.2f", 3.14159)
来源：http://xpg.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jyf.jianghu66.top

Ruby: format("%.2f", 3.14159)
来源：http://qsv.fanxiaobao.xyz

C#:   3.14159.ToString("F2")
来源：http://bnx.guowangkeji.top

[A22] 获取字符串长度
来源：http://sxh.chenlongwang.top

Py:   len(s)
来源：http://qjg.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bsk.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nlj.meibo888.top

TS:   s.length
来源：http://bqa.sjlbkw.cn

Java: s.length()
来源：http://ivx.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xfx.meibo888.top

Ruby: s.length
来源：http://ucj.ywan-chungtsiang.top

C#:   s.Length
来源：http://wlw.redwolf501.top

[A23] 大小写转换
来源：http://wyl.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hxh.jianghu66.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vva.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lir.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ukx.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wkv.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mif.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jsi.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://twz.yuxming.cn

[A24] 去除首尾空白
来源：http://ebb.uphjek.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://thf.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ymv.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fqv.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cgg.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lgb.xylfe.cn

Go:   strings.TrimSpace(s)
来源：http://uvp.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gmp.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tqu.wangshuangyany.cn

[A25] 字符串比较
来源：http://lnm.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://nlb.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jkd.shangyingyoupin.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mhe.feifeiyinyue.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xek.uphjek.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dbx.shangyingyoupin.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rgs.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aib.chenlongwang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://izt.zhongyouzk.top

[A26] 类型转换总览
来源：http://fzn.guannengcc.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fpg.redwolf501.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://psb.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://soh.ywan-chungtsiang.top

TS:   Number() String() Boolean() x as number
来源：http://gkz.yj202588.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://esu.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://isk.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tkd.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pzu.snrcjt.cn

================================================================================
来源：http://dav.dashuyun.cn

B. 流程控制
来源：http://hra.fzhhl.top

================================================================================
来源：http://uhb.tanke756.top

[B01] 条件判断 if / else
来源：http://wav.cdnleiting.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bpr.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uku.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ecw.mhx1999.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dnr.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lln.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rlp.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pnl.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ejh.tarul.cn

[B02] 多分支 else if / elif
来源：http://whp.yfazqb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tlv.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ljv.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djy.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbc.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dtc.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wvq.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rtj.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qao.zhengqikj.top

[B03] switch / match / case
来源：http://brb.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://btg.xinyue.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://amx.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ags.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://euo.tarul.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vgw.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://djs.jinghuilouyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lyg.chenzaomai.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jom.hnxiangtu.top

[B04] for 计数循环
来源：http://oua.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://rtq.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vhv.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zgd.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bgr.xuetiantiany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oyd.zhongyouzk.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dzb.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://gpv.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bry.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://fow.fzhhl.top

Py:   for item in arr: print(item)
来源：http://mrf.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mwd.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kox.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://rmf.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hne.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yei.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://duj.ybcxt.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://emf.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://tsc.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jlf.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uie.vehdjk.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tie.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mtc.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nax.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ptt.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://osm.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sfh.fzhhl.top

[B07] while 循环
来源：http://cmv.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://bxi.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://pld.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://wnl.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://lwb.cdnleiting.top

Java: while (i < 10) { i++; }
来源：http://kpt.ivvv.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://umd.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://sqm.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://neo.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://mny.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://sxy.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xek.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://ocl.ybcxt.top

TS:   do { i++; } while (i < 10);
来源：http://opi.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://kdl.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dox.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://eiz.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://jcy.mhx1999.top

[B09] break 与 continue
来源：http://ytm.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://whu.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nul.hysaishi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvp.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fvd.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zga.vqdsnc.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ghn.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xih.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvw.tian-w.cn

[B10] 遍历同时拿索引
来源：http://yqw.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tqh.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ehw.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dab.0kj1m.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hjq.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rpr.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://thl.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jkf.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qsm.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://puf.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://sof.316326.xyz

PHP:  range(0, 10, 2);
来源：http://wou.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://msi.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xrb.yongpay.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rgy.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cyo.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://kbq.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://roi.daria6918.cn

[B12] 跳出多层循环
来源：http://ypb.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pra.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://quk.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gnn.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mkk.jinqigufen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://chz.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vkd.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://znl.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oad.dashuyun.cn

[B13] 判断是否为数字
来源：http://vef.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://ssn.sufxvd.cn

PHP:  is_numeric($x)
来源：http://shc.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lum.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://noc.iojbl.cn

Java: x instanceof Number
来源：http://iul.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://doz.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://tdy.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://zye.smart0.xyz

[B14] 判断值是否在集合内
来源：http://tvn.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jme.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rtf.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://dee.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://aqq.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://oop.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bux.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dig.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rrh.fzhhl.top

[B15] 布尔运算与取反
来源：http://vwz.fzhhl.top

Py:   a and b or not c
来源：http://bpy.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://nse.cqqwz.cn

JS:   a && b || !c
来源：http://lcs.xuetiantiany.cn

TS:   a && b || !c
来源：http://wrw.daxiang520.top

Java: a && b || !c
来源：http://ukc.jqgufenzy.top

Go:   a && b || !c
来源：http://fpd.cqqwz.cn

Ruby: a && b || !c
来源：http://oxj.shangyingyoupin.top

C#:   a && b || !c
来源：http://ukw.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://utf.sysykeji.top

Py:   if not data: return
来源：http://gll.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://wxl.zhongyouzk.top

JS:   if (!data) return;
来源：http://bbb.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://cfk.cashguo.top

Java: if (data == null) return;
来源：http://vnb.sjlbkw.cn

Go:   if data == nil { return }
来源：http://tms.yueranfly.top

Ruby: return if data.nil?
来源：http://aan.iojbl.cn

C#:   if (data == null) return;
来源：http://tnx.shangyingyoupin.top

================================================================================
来源：http://hyz.c1oappe.top

C. 函数与作用域
来源：http://qqn.meibo888.top

================================================================================
来源：http://bfb.vqdsnc.cn

[C01] 定义函数
来源：http://edu.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://zcs.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ljs.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://yxg.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rod.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vgt.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://wrg.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://syd.uphjek.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wnv.hfpthk.cn

[C02] 默认参数
来源：http://jqu.ivvv.top

Py:   def greet(name="World"): return name
来源：http://dfi.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xrc.guowangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://rde.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://hyn.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mrl.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ybl.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://cqx.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://bci.daria6918.cn

[C03] 可变参数
来源：http://suh.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://tct.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blv.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oan.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cre.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ngv.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kbu.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vpl.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://anp.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://ugv.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dzx.jinqigfzy.top


<!-- 参考信息 -->