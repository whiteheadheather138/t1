代发 wailian999

Py:   "第一行\n第二行"
来源：http://zkw.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://nlp.hesvh.cn

JS:   "第一行\n第二行"
来源：http://lof.hnxiangtu.top

TS:   "第一行\n第二行"
来源：http://ixk.tarul.cn

Java: "第一行\n第二行"
来源：http://tvi.guannengcc.top

Go:   "第一行\n第二行"
来源：http://wjo.fktsv.cn

Ruby: "第一行\n第二行"
来源：http://dqf.0kj1m.cn

C#:   "第一行\n第二行"
来源：http://ojb.cucudq.cn

[A14] 注释写法
来源：http://wev.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zev.quarkkingdee.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mmi.yanxiufei.cn

JS:   // 单行；/* 多行 */
来源：http://ppt.xingfuxueyuan.xyz

TS:   // 单行；/* 多行 */
来源：http://yyi.snrcjt.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xtv.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://wbf.uphjek.com

Ruby: # 单行；=begin 多行 =end
来源：http://xwp.aibaodan.cn

C#:   // 单行；/* 多行 */
来源：http://rls.yvedp.cn

[A15] 空值判断与默认值
来源：http://wjf.0kj1m.cn

Py:   value = data or "默认值"
来源：http://tbg.wangshuangyany.cn

PHP:  $value = $data ?? "默认值";
来源：http://osg.jlsjyb.cn

JS:   const value = data ?? "默认值";
来源：http://lku.yj202588.top

TS:   const value = data ?? "默认值";
来源：http://ttx.316326.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://osd.havefunace.top

Go:   if data == "" { data = "默认值" }
来源：http://xap.quarkkingdee.top

Ruby: value = data || "默认值"
来源：http://wgz.zdqjudy.top

C#:   var value = data ?? "默认值";
来源：http://wvm.shuidangran.top

[A16] 真假值判断规则
来源：http://zgy.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jbg.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ulf.ydzc1.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ydo.yanxiufei.cn

TS:   if (!x) {}
来源：http://nyl.quarkkingdee.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uqp.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ttb.shuidangran.top

Ruby: unless x            # nil 与 false 为假
来源：http://wve.redwolf501.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mkp.guannengcc.top

[A17] 位运算
来源：http://fxn.snrcjt.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmo.gogol.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ywu.yueranfly.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://okd.ctjpmb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kgr.birdmap.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssd.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yzx.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ybd.xuanzx.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mek.yj20258888.top

[A18] 字符与 ASCII 码互转
来源：http://akj.chenjidiqi.icu

Py:   ord("A"); chr(65)
来源：http://ako.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://ycm.bjfxy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oon.jqgfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rkq.bbcook.cn

Java: (int) 'A'; (char) 65
来源：http://kjo.c1oappe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gpi.cheryme.top

Ruby: "A".ord; 65.chr
来源：http://gxu.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://xrd.sweek.top

[A19] 交换两个变量
来源：http://umm.hnxiangtu.top

Py:   a, b = b, a
来源：http://bhz.sxryk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ydg.0kj1m.cn

JS:   [a, b] = [b, a];
来源：http://cjc.yangfankeji.com

TS:   [a, b] = [b, a];
来源：http://xzd.sufxvd.cn

Java: int t = a; a = b; b = t;
来源：http://ubz.gaohongyu789.top

Go:   a, b = b, a
来源：http://ppx.zhiwuduotai.top

Ruby: a, b = b, a
来源：http://ogs.havefunace.top

C#:   (a, b) = (b, a);
来源：http://wky.hfpthk.cn

[A20] 读取标准输入
来源：http://hyn.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://umc.0kj1m.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uyh.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cwk.jyoumei.cn

TS:   // Node.js：readline 模块
来源：http://oeh.shanyushiyangtech.top

Java: new Scanner(System.in).nextLine()
来源：http://hef.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bxv.cheryme.top

Ruby: gets.chomp
来源：http://seo.pycfn.com

C#:   Console.ReadLine();
来源：http://kha.gzhubu.top

[A21] 保留指定小数位输出
来源：http://qqi.nanxuanxn.top

Py:   f"{3.14159:.2f}"
来源：http://bxv.zhiwuduotai.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wpm.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://pso.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://cyy.shuidangran.top

Java: String.format("%.2f", 3.14159)
来源：http://xtl.hcnkem.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ecw.c1oappe.top

Ruby: format("%.2f", 3.14159)
来源：http://snx.hywenlv.cn

C#:   3.14159.ToString("F2")
来源：http://eur.zhijiandao.cn

[A22] 获取字符串长度
来源：http://ilx.ivvv.top

Py:   len(s)
来源：http://skc.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bsy.smart0.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zmq.52xcode.cn

TS:   s.length
来源：http://dgr.zhaomingkeji.xyz

Java: s.length()
来源：http://cgz.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qtv.sufxvd.cn

Ruby: s.length
来源：http://qvd.shuidangran.top

C#:   s.Length
来源：http://zha.cheryme.top

[A23] 大小写转换
来源：http://tio.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xuv.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wle.hysaishi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yoj.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://npf.ydjk.org.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sbe.gogol.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qhb.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hwm.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eew.fzhhl.top

[A24] 去除首尾空白
来源：http://noh.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uju.hongshengwenyu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://beo.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xep.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ccu.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rwa.sweek.top

Go:   strings.TrimSpace(s)
来源：http://zbc.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kos.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aqv.cheryme.top

[A25] 字符串比较
来源：http://acl.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://qaw.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cqk.jinyuanbaomall.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mam.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vhm.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mgt.fzhhl.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://avd.hongshengwenyu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ume.zhiwuduotai.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lps.cdnleiting.top

[A26] 类型转换总览
来源：http://dxs.tianlin.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vxl.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cdr.yuxming.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fmf.9152youxi.cn

TS:   Number() String() Boolean() x as number
来源：http://fat.birdmap.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lyo.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yje.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kgf.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ffy.ivvv.top

================================================================================
来源：http://ovn.kuanghao11.cn

B. 流程控制
来源：http://xyk.yueranfly.top

================================================================================
来源：http://jpx.jianghu66.top

[B01] 条件判断 if / else
来源：http://dtk.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tvv.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vie.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nti.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hun.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://imh.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dlo.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hwc.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gvm.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://nrx.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gxc.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vvw.uphjek.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://igg.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://flw.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubw.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eed.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jvi.hysaishi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jsi.fktsv.cn

[B03] switch / match / case
来源：http://nhn.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zzu.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://snq.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uys.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://umm.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gsv.fktsv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tnk.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gaj.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rqq.cdnleiting.top

[B04] for 计数循环
来源：http://gou.pycfn.com

Py:   for i in range(10): print(i)
来源：http://ugq.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tgn.fzhhl.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uob.xingfuxueyuan.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://czm.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jst.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wzk.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://nlm.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jnn.yj202588.top

[B05] 遍历数组 / 列表
来源：http://pvl.yongpay.top

Py:   for item in arr: print(item)
来源：http://mri.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bpl.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gcd.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ibh.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gar.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://duv.shuidangran.top

Ruby: arr.each { |item| puts item }
来源：http://hsi.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gxn.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://pzv.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ktp.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oew.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://krt.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qyw.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zea.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vyt.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lox.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eyf.yangfankeji.com

[B07] while 循环
来源：http://izy.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://irg.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://fdn.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://leu.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://zlh.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://ysp.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://owu.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://mpb.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://upl.andypj.xyz

[B08] do-while（至少执行一次）
来源：http://ijq.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://tpt.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://lxw.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://jgd.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://hle.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://oyy.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://aln.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qqp.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://mof.sufxvd.cn

[B09] break 与 continue
来源：http://xcq.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gls.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yvk.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftd.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bbo.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tat.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ija.nwbrower.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ivb.hfpthk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tps.bjfxy.top

[B10] 遍历同时拿索引
来源：http://fzw.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://scs.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://img.cqqwz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://owf.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pnc.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gse.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://slu.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eip.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dma.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://xnn.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://lic.xuetiantiany.cn

PHP:  range(0, 10, 2);
来源：http://ddv.daria6918.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vyd.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cyl.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iyu.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://egm.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://rim.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pmo.cdnleiting.top

[B12] 跳出多层循环
来源：http://jmx.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://alm.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nex.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ykb.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uum.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nwf.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ktn.zhengqikj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fno.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://htz.316326.xyz

[B13] 判断是否为数字
来源：http://pqt.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://qco.xinyue.icu

PHP:  is_numeric($x)
来源：http://gcp.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://msj.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rwb.yueranfly.top

Java: x instanceof Number
来源：http://jfk.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dnv.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://dbq.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://ulb.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://rir.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yce.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://slx.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://tas.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://ivs.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://jaq.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pfn.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vlp.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gzi.zdqjudy.top

[B15] 布尔运算与取反
来源：http://sdv.zhixingplan.top

Py:   a and b or not c
来源：http://awd.hcnkem.com

PHP:  $a && $b || !$c
来源：http://oso.jinghuilouyu.cn

JS:   a && b || !c
来源：http://edm.ydzc1.top

TS:   a && b || !c
来源：http://slt.guannengcc.top

Java: a && b || !c
来源：http://fnc.cqqwz.cn

Go:   a && b || !c
来源：http://qas.mhx1999.top

Ruby: a && b || !c
来源：http://ehv.zhoulong.xyz

C#:   a && b || !c
来源：http://xop.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pnu.jqgufenzy.top

Py:   if not data: return
来源：http://hiw.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://cnm.yj20258.top

JS:   if (!data) return;
来源：http://zrd.dashuyun.cn

TS:   if (!data) return;
来源：http://bbt.epnwcf.com

Java: if (data == null) return;
来源：http://rpa.zhixingplan.top

Go:   if data == nil { return }
来源：http://orh.snrcjt.cn

Ruby: return if data.nil?
来源：http://qqd.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://rbw.nanxinkj.top

================================================================================
来源：http://hrb.9152youxi.cn

C. 函数与作用域
来源：http://nbo.ivvv.top

================================================================================
来源：http://ehb.zhijiandao.cn

[C01] 定义函数
来源：http://irv.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://tst.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bef.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://jhz.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ssr.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://foe.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gay.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://sop.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vug.sysykeji.top

[C02] 默认参数
来源：http://nkc.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://aeh.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cbg.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://iem.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dwu.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mcg.sjlbkw.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bto.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://dcu.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://mjt.cashguo.top

[C03] 可变参数
来源：http://frq.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://xqv.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://abr.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://idf.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dgr.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hxq.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lev.ybcxt.top


<!-- 参考信息 -->