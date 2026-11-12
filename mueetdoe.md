代发 wailian999

Py:   "第一行\n第二行"
来源：http://qrw.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://duh.sweek.top

JS:   "第一行\n第二行"
来源：http://gop.ivvv.top

TS:   "第一行\n第二行"
来源：http://bya.jinqigufen.top

Java: "第一行\n第二行"
来源：http://xvf.cqqwz.cn

Go:   "第一行\n第二行"
来源：http://czt.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://scy.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://dbl.yonumen.top

[A14] 注释写法
来源：http://eav.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://izf.zdqjudy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ezu.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://lpy.vqdsnc.cn

TS:   // 单行；/* 多行 */
来源：http://ypc.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ram.zhongyouzk.top

Go:   // 单行；/* 多行 */
来源：http://haa.c1oappe.top

Ruby: # 单行；=begin 多行 =end
来源：http://drk.cdnleiting.top

C#:   // 单行；/* 多行 */
来源：http://vfl.xingfuxueyuan.xyz

[A15] 空值判断与默认值
来源：http://ubg.hysaishi.cn

Py:   value = data or "默认值"
来源：http://yrj.yj20258.top

PHP:  $value = $data ?? "默认值";
来源：http://xbq.9152youxi.cn

JS:   const value = data ?? "默认值";
来源：http://yvz.fehbvm.com

TS:   const value = data ?? "默认值";
来源：http://php.daria6918.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://laj.nanxinkj.top

Go:   if data == "" { data = "默认值" }
来源：http://nne.ywan-chungtsiang.top

Ruby: value = data || "默认值"
来源：http://let.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://tnz.yanxiufei.cn

[A16] 真假值判断规则
来源：http://nnj.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lsq.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yyc.xziqi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vcp.nanxinkj.top

TS:   if (!x) {}
来源：http://sbt.ywan-chungtsiang.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xkr.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qoq.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gzv.yonumen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://azo.316326.xyz

[A17] 位运算
来源：http://izy.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rrc.yongpay.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dcn.xinyue.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxl.yvedp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mnv.tanke756.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzh.xinyue.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pvi.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bfz.yuxming.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xbo.hywenlv.cn

[A18] 字符与 ASCII 码互转
来源：http://hzb.aibaodan.cn

Py:   ord("A"); chr(65)
来源：http://srh.birdmap.top

PHP:  ord("A"); chr(65)
来源：http://uda.sufxvd.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qgt.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://axz.yj20258.top

Java: (int) 'A'; (char) 65
来源：http://rsy.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qol.hfpthk.cn

Ruby: "A".ord; 65.chr
来源：http://zud.yfazqb.com

C#:   (int)'A'; (char)65
来源：http://eoi.pycfn.com

[A19] 交换两个变量
来源：http://ues.jinqigfzy.top

Py:   a, b = b, a
来源：http://xqg.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yun.yj20258888.top

JS:   [a, b] = [b, a];
来源：http://zux.xylfe.cn

TS:   [a, b] = [b, a];
来源：http://huc.ehwqpu.com

Java: int t = a; a = b; b = t;
来源：http://hze.aibaodan.cn

Go:   a, b = b, a
来源：http://rwe.zhiwuduotai.top

Ruby: a, b = b, a
来源：http://ewr.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://nhm.yongpay.top

[A20] 读取标准输入
来源：http://tah.pengpengdd.cyou

Py:   name = input("请输入：")
来源：http://gjg.chenjidiqi.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://eps.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wdw.jinyuanbaomall.cn

TS:   // Node.js：readline 模块
来源：http://oha.jlsjyb.cn

Java: new Scanner(System.in).nextLine()
来源：http://zap.birdmap.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dtm.hongshengwenyu.top

Ruby: gets.chomp
来源：http://azm.xingfuxueyuan.xyz

C#:   Console.ReadLine();
来源：http://nlb.hnqzz.top

[A21] 保留指定小数位输出
来源：http://bqc.ydzc1.top

Py:   f"{3.14159:.2f}"
来源：http://fqf.zdqjudy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zrw.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://pdl.ctjpmb.com

TS:   (3.14159).toFixed(2)
来源：http://pmh.zycfv.cn

Java: String.format("%.2f", 3.14159)
来源：http://hue.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jgr.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://lpn.hfpthk.cn

C#:   3.14159.ToString("F2")
来源：http://rzz.hysaishi.cn

[A22] 获取字符串长度
来源：http://sto.ppjwa.cn

Py:   len(s)
来源：http://heq.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nsx.jqgfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qrz.epnwcf.com

TS:   s.length
来源：http://pww.cheryme.top

Java: s.length()
来源：http://tdx.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xrp.tarul.cn

Ruby: s.length
来源：http://bhd.nwbrower.top

C#:   s.Length
来源：http://ebt.jqgfzy.top

[A23] 大小写转换
来源：http://bof.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rtv.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mdh.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uqk.52xcode.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wqb.wangshuangyany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xot.yongpay.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yqn.havefunace.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nwn.yuanzhike.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hjd.fktsv.cn

[A24] 去除首尾空白
来源：http://uxo.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://req.ppjwa.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xyt.fktsv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bvd.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wvu.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kko.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://jpg.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://din.haohaochexian.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ikk.svipenyu.cn

[A25] 字符串比较
来源：http://orj.zhaomingkeji.xyz

Py:   s1 == s2; s1 != s2
来源：http://iul.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kdv.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vit.yuxming.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xvf.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cjn.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cxa.xinyue.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://nfk.hammf.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fpg.cqqwz.cn

[A26] 类型转换总览
来源：http://bjj.epnwcf.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ekr.xingfuxueyuan.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lbz.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xyt.fehbvm.com

TS:   Number() String() Boolean() x as number
来源：http://wgd.9152youxi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://isr.sxryk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cxb.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://igg.jinyuanbaomall.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iuk.shzxlz.cn

================================================================================
来源：http://rcu.dianchejie.cn

B. 流程控制
来源：http://dhf.hcnkem.com

================================================================================
来源：http://lwu.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://lyh.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vkn.tian-w.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zjc.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yjo.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jhi.jinghuilouyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bas.nanxuanxn.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bmx.iojbl.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fan.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lum.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://uvu.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qob.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qtr.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyl.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jld.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qdi.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uwo.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ebt.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzn.0kj1m.cn

[B03] switch / match / case
来源：http://mco.xziqi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://shn.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jtf.bjfxy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zrq.fehbvm.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ygx.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hjz.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uwt.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://inh.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cxu.fehbvm.com

[B04] for 计数循环
来源：http://oyk.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://npl.zdqjudy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kis.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kdk.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://llt.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lkz.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://man.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://hhd.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vpg.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://njf.havefunace.top

Py:   for item in arr: print(item)
来源：http://exf.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jyo.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hzu.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ybq.yongpay.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jzz.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sud.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://dsf.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fgf.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://qlp.hcnkem.com

Py:   for k, v in d.items(): print(k, v)
来源：http://sta.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xbe.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ikn.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uji.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yac.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sws.zdqjudy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aro.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wza.snrcjt.cn

[B07] while 循环
来源：http://oxb.zycfv.cn

Py:   while i < 10: i += 1
来源：http://xuz.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ztm.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://qaj.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://xek.yj202588.top

Java: while (i < 10) { i++; }
来源：http://ooi.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://epc.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://pde.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://uxk.pycfn.com

[B08] do-while（至少执行一次）
来源：http://nav.zdbjq.cn

Py:   # 无 do-while：用 while True + break
来源：http://jiv.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://djf.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://zgb.yj202588.top

TS:   do { i++; } while (i < 10);
来源：http://wja.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://khv.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fnk.fzhhl.top

Ruby: begin; i += 1; end while i < 10
来源：http://afp.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://snp.hysaishi.cn

[B09] break 与 continue
来源：http://qlm.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://njm.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gno.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gvr.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rmx.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfm.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eex.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zxf.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://crj.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://kvx.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qeb.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://auw.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nct.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zzp.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zjm.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://esl.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bvp.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aye.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://dcm.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://yai.cucudq.cn

PHP:  range(0, 10, 2);
来源：http://lrk.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsr.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ngj.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://afs.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://adi.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://jxk.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jbz.hesvh.cn

[B12] 跳出多层循环
来源：http://ewr.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lba.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://iln.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fou.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dla.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ftj.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://opf.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ooc.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vzd.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://rbx.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://rfu.jqgfzy.top

PHP:  is_numeric($x)
来源：http://sie.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jbf.jinqigufen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qnc.316326.xyz

Java: x instanceof Number
来源：http://nmj.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fgg.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://htx.iojbl.cn

C#:   x is int or double or decimal
来源：http://gqq.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://npg.ywan-chungtsiang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wha.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ibu.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://zqy.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://rxl.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yci.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ztw.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mjg.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tgi.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://ogc.pengpengdd.cyou

Py:   a and b or not c
来源：http://nsx.yonumen.top

PHP:  $a && $b || !$c
来源：http://req.gaohongyu789.top

JS:   a && b || !c
来源：http://uqx.andypj.xyz

TS:   a && b || !c
来源：http://fbr.shanyushiyangkeji.top

Java: a && b || !c
来源：http://nqg.zhijiandao.cn

Go:   a && b || !c
来源：http://eyn.yuanzhike.top

Ruby: a && b || !c
来源：http://rld.tanke756.top

C#:   a && b || !c
来源：http://xze.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://cuc.zhaomingkeji.xyz

Py:   if not data: return
来源：http://xzw.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://hfg.yvedp.cn

JS:   if (!data) return;
来源：http://jhh.316326.xyz

TS:   if (!data) return;
来源：http://agc.dashuyun.cn

Java: if (data == null) return;
来源：http://cci.hysaishi.cn

Go:   if data == nil { return }
来源：http://rws.yangfankeji.com

Ruby: return if data.nil?
来源：http://rmz.redwolf501.top

C#:   if (data == null) return;
来源：http://pjs.cqqwz.cn

================================================================================
来源：http://paz.ehwqpu.com

C. 函数与作用域
来源：http://vli.ivvv.top

================================================================================
来源：http://xam.chenlongwang.top

[C01] 定义函数
来源：http://scu.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://sru.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xze.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://vat.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vsk.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jxd.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kju.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://yvk.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iwc.sufxvd.cn

[C02] 默认参数
来源：http://zqv.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://jkf.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qyt.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://xuc.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tyj.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://uzk.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jss.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://jze.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://wku.c1oappe.top

[C03] 可变参数
来源：http://gry.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://hdw.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aqj.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://plv.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jkn.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ynn.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ahh.redwolf501.top


<!-- 参考信息 -->