代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iho.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://txc.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://gfz.xuetiantiany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xgu.ivvv.top

Py:   "第一行\n第二行"
来源：http://geo.zhixingplan.top

PHP:  "第一行\n第二行"
来源：http://xko.cdnleiting.top

JS:   "第一行\n第二行"
来源：http://vte.fengsongda.top

TS:   "第一行\n第二行"
来源：http://zvr.shangyingyoupin.top

Java: "第一行\n第二行"
来源：http://kum.tanke756.top

Go:   "第一行\n第二行"
来源：http://zse.havefunace.top

Ruby: "第一行\n第二行"
来源：http://yeo.chenzaomai.com

C#:   "第一行\n第二行"
来源：http://mnr.fktsv.cn

[A14] 注释写法
来源：http://siv.xylfe.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ssq.wangdashe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://whr.0kj1m.cn

JS:   // 单行；/* 多行 */
来源：http://yjz.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://eug.xziqi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wjk.havefunace.top

Go:   // 单行；/* 多行 */
来源：http://fej.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://cwb.tian-w.cn

C#:   // 单行；/* 多行 */
来源：http://zkg.birdmap.top

[A15] 空值判断与默认值
来源：http://ruq.gotoacloud.top

Py:   value = data or "默认值"
来源：http://xex.xuetiantiany.cn

PHP:  $value = $data ?? "默认值";
来源：http://gww.jiagoushi.top

JS:   const value = data ?? "默认值";
来源：http://gqu.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://zjp.yuanzhike.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ikn.ctjpmb.com

Go:   if data == "" { data = "默认值" }
来源：http://xdm.wangshuangyany.cn

Ruby: value = data || "默认值"
来源：http://xyw.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://pfo.ctjpmb.com

[A16] 真假值判断规则
来源：http://pow.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eqh.yangfankeji.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ydn.bjfxy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ojx.xziqi.cn

TS:   if (!x) {}
来源：http://uus.fanxiaobao.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ijm.zhongyouzk.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yev.xylfe.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sii.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nuf.cdnleiting.top

[A17] 位运算
来源：http://gfo.ywan-chungtsiang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hes.yuanzhike.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pkj.sweek.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pbm.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bof.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ywt.yj20258.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ems.bjfxy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ojn.fanxiaobao.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yvr.ctjpmb.com

[A18] 字符与 ASCII 码互转
来源：http://tyw.aibaodan.cn

Py:   ord("A"); chr(65)
来源：http://dlu.zhiwuduotai.top

PHP:  ord("A"); chr(65)
来源：http://fea.iojbl.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vmr.chenzaomai.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wqw.yuanzhike.top

Java: (int) 'A'; (char) 65
来源：http://dgv.guowangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bkk.jiagoushi.top

Ruby: "A".ord; 65.chr
来源：http://rpw.hywenlv.cn

C#:   (int)'A'; (char)65
来源：http://pgx.fktsv.cn

[A19] 交换两个变量
来源：http://nnn.zhiwuduotai.top

Py:   a, b = b, a
来源：http://tnk.svipenyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rgi.fktsv.cn

JS:   [a, b] = [b, a];
来源：http://vle.yonumen.top

TS:   [a, b] = [b, a];
来源：http://svw.jinqigufen.top

Java: int t = a; a = b; b = t;
来源：http://jvi.sweek.top

Go:   a, b = b, a
来源：http://dvq.vehdjk.com

Ruby: a, b = b, a
来源：http://qyf.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://qkx.dianchejie.cn

[A20] 读取标准输入
来源：http://pol.zhengqikj.top

Py:   name = input("请输入：")
来源：http://pft.vqdsnc.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://idv.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vsg.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://pzl.xziqi.cn

Java: new Scanner(System.in).nextLine()
来源：http://qsm.yfazqb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rfa.jlsjyb.cn

Ruby: gets.chomp
来源：http://tux.ehwqpu.com

C#:   Console.ReadLine();
来源：http://rur.aizwys.cn

[A21] 保留指定小数位输出
来源：http://nti.xylfe.cn

Py:   f"{3.14159:.2f}"
来源：http://nsb.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wvv.yueranfly.top

JS:   (3.14159).toFixed(2)
来源：http://iee.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://saq.ywan-chungtsiang.top

Java: String.format("%.2f", 3.14159)
来源：http://kcm.yonumen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gqm.tian-w.cn

Ruby: format("%.2f", 3.14159)
来源：http://yde.hesvh.cn

C#:   3.14159.ToString("F2")
来源：http://obs.ydjk.org.cn

[A22] 获取字符串长度
来源：http://mpn.zycfv.cn

Py:   len(s)
来源：http://ymq.hywenlv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fgn.zycfv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jyx.yvedp.cn

TS:   s.length
来源：http://skg.jinqigufen.top

Java: s.length()
来源：http://qib.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wqf.ydzc1.top

Ruby: s.length
来源：http://wpk.jinqigfzy.top

C#:   s.Length
来源：http://cmk.aizwys.cn

[A23] 大小写转换
来源：http://dyc.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nkx.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qux.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dvi.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lih.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vti.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bqm.mhx1999.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cki.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gqk.iojbl.cn

[A24] 去除首尾空白
来源：http://pff.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://woe.yuanzhike.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xef.cashguo.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yoh.yj20258.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vrw.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vig.aibaodan.cn

Go:   strings.TrimSpace(s)
来源：http://diw.yangfankeji.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hyv.hcnkem.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zjp.ywan-chungtsiang.top

[A25] 字符串比较
来源：http://jrw.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://hrm.hesvh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uby.ivvv.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kfi.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lzz.xingfuxueyuan.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mgi.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://orn.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tca.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://flw.yfazqb.com

[A26] 类型转换总览
来源：http://gbo.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vnw.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vjp.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://okr.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://mqp.ivvv.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pit.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bsw.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pes.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wdx.cqqwz.cn

================================================================================
来源：http://ewi.gogol.net.cn

B. 流程控制
来源：http://uzi.yfazqb.com

================================================================================
来源：http://saf.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://pdm.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gog.cashguo.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xjt.redwolf501.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dzj.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hde.c1oappe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bgr.zdbjq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ani.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wwt.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ctt.cqqwz.cn

[B02] 多分支 else if / elif
来源：http://wkk.wangshuangyany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rfb.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hyi.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vln.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iup.xinyue.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rso.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xpv.shzxlz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cej.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cty.xylfe.cn

[B03] switch / match / case
来源：http://xfi.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ych.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hfq.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ahp.zhixingplan.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aqc.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hbz.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aoi.aibaodan.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vse.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://web.smart0.xyz

[B04] for 计数循环
来源：http://chs.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://klf.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fxc.yonumen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://drx.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://htu.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://byo.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iac.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://fpv.zhixingplan.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://esh.yonumen.top

[B05] 遍历数组 / 列表
来源：http://qeq.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://bdu.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fpn.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tqz.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hxc.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://jan.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qtw.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://mcj.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ziy.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://zkx.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://yga.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xob.gaohongyu789.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yvl.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yih.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xkf.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fvl.sufxvd.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xkq.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://raa.jinqigfzy.top

[B07] while 循环
来源：http://uwk.aizwys.cn

Py:   while i < 10: i += 1
来源：http://bht.sxryk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rpc.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://zww.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://vpm.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://bxc.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nej.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://xcv.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://amh.uphjek.com

[B08] do-while（至少执行一次）
来源：http://mro.sysykeji.top

Py:   # 无 do-while：用 while True + break
来源：http://zwc.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uxl.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://kel.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://xwp.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://svz.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ddn.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kbi.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://kgn.feifeiyinyue.top

[B09] break 与 continue
来源：http://shk.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cnw.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rho.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqe.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kdl.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nff.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qbk.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gbc.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sds.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://otn.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rrr.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ssy.nwbrower.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nob.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jia.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pde.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jyf.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://moe.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ywb.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://bth.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://okp.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://mjz.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lxg.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qfi.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kyu.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oub.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://mgw.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ycn.vehdjk.com

[B12] 跳出多层循环
来源：http://sem.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://afp.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pox.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xyz.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vhs.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pwu.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ira.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jbc.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nkh.pycfn.com

[B13] 判断是否为数字
来源：http://hui.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://fxk.xinyue.icu

PHP:  is_numeric($x)
来源：http://ouw.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gpz.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://osd.dashuyun.cn

Java: x instanceof Number
来源：http://rdd.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xxd.hcnkem.com

Ruby: x.is_a?(Numeric)
来源：http://fuy.gotoacloud.top

C#:   x is int or double or decimal
来源：http://gzw.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://ovh.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dxy.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://apy.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://ksz.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://kpi.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fbv.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cuh.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rib.wangshuangyany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://slq.birdmap.top

[B15] 布尔运算与取反
来源：http://gre.guowangkeji.top

Py:   a and b or not c
来源：http://khv.jianghu66.top

PHP:  $a && $b || !$c
来源：http://ysn.jyoumei.cn

JS:   a && b || !c
来源：http://ogq.fengsongda.top

TS:   a && b || !c
来源：http://pij.zhongyouzk.top

Java: a && b || !c
来源：http://iyu.zhixingplan.top

Go:   a && b || !c
来源：http://btb.xziqi.cn

Ruby: a && b || !c
来源：http://cvu.fehbvm.com

C#:   a && b || !c
来源：http://kvq.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qbh.zhongyouzk.top

Py:   if not data: return
来源：http://mcs.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://boe.meibo888.top

JS:   if (!data) return;
来源：http://vtr.ivvv.top

TS:   if (!data) return;
来源：http://ose.316326.xyz

Java: if (data == null) return;
来源：http://yjy.jianghu66.top

Go:   if data == nil { return }
来源：http://vmy.kuanghao11.cn

Ruby: return if data.nil?
来源：http://ypa.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://vfy.zdqjudy.top

================================================================================
来源：http://gpj.tanke756.top

C. 函数与作用域
来源：http://sup.hcnkem.com

================================================================================
来源：http://vir.hammf.cn

[C01] 定义函数
来源：http://cth.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://obd.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rml.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://bpq.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://szr.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tnb.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wdg.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://rwz.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://obh.yongpay.top

[C02] 默认参数
来源：http://huj.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://ohn.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://wdp.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://cgz.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vgj.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qhu.fengsongda.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wnk.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://der.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://vxi.uphjek.com

[C03] 可变参数
来源：http://kwt.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://col.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tra.vqdsnc.cn


<!-- 参考信息 -->