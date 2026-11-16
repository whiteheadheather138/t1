代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jrl.yonumen.top

JS:   `Hello, ${name}!`
来源：http://usv.cdnleiting.top

TS:   `Hello, ${name}!`
来源：http://fgu.epnwcf.com

Java: "Hello, %s!".formatted(name)
来源：http://azc.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qyo.cucudq.cn

Ruby: "Hello, #{name}!"
来源：http://lyu.svipenyu.cn

C#:   $"Hello, {name}!"
来源：http://efm.wangshuangyany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dfq.ehwqpu.com

Py:   "第一行\n第二行"
来源：http://gws.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://abs.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://mtk.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://aym.wangshuangyany.cn

Java: "第一行\n第二行"
来源：http://usk.fengsongda.top

Go:   "第一行\n第二行"
来源：http://lzw.iojbl.cn

Ruby: "第一行\n第二行"
来源：http://mtl.316326.xyz

C#:   "第一行\n第二行"
来源：http://vuv.birdmap.top

[A14] 注释写法
来源：http://vmi.jinghuilouyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kvv.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gch.9152youxi.cn

JS:   // 单行；/* 多行 */
来源：http://qzh.ywan-chungtsiang.top

TS:   // 单行；/* 多行 */
来源：http://hxd.haohaochexian.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ppx.yvedp.cn

Go:   // 单行；/* 多行 */
来源：http://emb.9152youxi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oqg.yfazqb.com

C#:   // 单行；/* 多行 */
来源：http://iox.epnwcf.com

[A15] 空值判断与默认值
来源：http://lpk.gogol.net.cn

Py:   value = data or "默认值"
来源：http://jle.c1oappe.top

PHP:  $value = $data ?? "默认值";
来源：http://kar.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://kkt.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://rhv.pengpengdd.cyou

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ekl.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://mdz.gotoacloud.top

Ruby: value = data || "默认值"
来源：http://rtp.jqgufenzy.top

C#:   var value = data ?? "默认值";
来源：http://jnb.tianlin.xyz

[A16] 真假值判断规则
来源：http://yct.hammf.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vng.chenzaomai.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lfb.gaohongyu789.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://emn.jianghu66.top

TS:   if (!x) {}
来源：http://wlx.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://twd.shanyushiyangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xwm.wangshuangyany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uas.fzhhl.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hnw.redwolf501.top

[A17] 位运算
来源：http://ypd.yj20258888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://psr.hywenlv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jfg.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kis.gzhubu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ihv.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cru.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cey.haohaochexian.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://okt.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pwy.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://jjl.chenzaomai.com

Py:   ord("A"); chr(65)
来源：http://dof.hnxiangtu.top

PHP:  ord("A"); chr(65)
来源：http://esk.iojbl.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jmm.ehwqpu.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gok.xuetiantiany.cn

Java: (int) 'A'; (char) 65
来源：http://tui.zhiwuduotai.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zqx.hfpthk.cn

Ruby: "A".ord; 65.chr
来源：http://zlf.fehbvm.com

C#:   (int)'A'; (char)65
来源：http://ugb.daria6918.cn

[A19] 交换两个变量
来源：http://aaw.shangyingyoupin.top

Py:   a, b = b, a
来源：http://psr.yfazqb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://oly.yuxming.cn

JS:   [a, b] = [b, a];
来源：http://qiw.fktsv.cn

TS:   [a, b] = [b, a];
来源：http://nei.uphjek.com

Java: int t = a; a = b; b = t;
来源：http://wom.meibo888.top

Go:   a, b = b, a
来源：http://rve.feifeiyinyue.top

Ruby: a, b = b, a
来源：http://stu.daxiang520.top

C#:   (a, b) = (b, a);
来源：http://uhq.snrcjt.cn

[A20] 读取标准输入
来源：http://dca.zhoulong.xyz

Py:   name = input("请输入：")
来源：http://iba.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zzr.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pra.zdqjudy.top

TS:   // Node.js：readline 模块
来源：http://abc.jlsjyb.cn

Java: new Scanner(System.in).nextLine()
来源：http://tud.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nye.tianlin.xyz

Ruby: gets.chomp
来源：http://ylj.jlsjyb.cn

C#:   Console.ReadLine();
来源：http://pnk.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://tmu.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://shu.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xsm.xziqi.cn

JS:   (3.14159).toFixed(2)
来源：http://cxp.fzhhl.top

TS:   (3.14159).toFixed(2)
来源：http://gob.birdmap.top

Java: String.format("%.2f", 3.14159)
来源：http://spd.cheryme.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vri.smart0.xyz

Ruby: format("%.2f", 3.14159)
来源：http://jib.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://piv.jlsjyb.cn

[A22] 获取字符串长度
来源：http://rpd.zhiwuduotai.top

Py:   len(s)
来源：http://kqz.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dhi.zhoulong.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jvo.c1oappe.top

TS:   s.length
来源：http://xju.jinqigufen.top

Java: s.length()
来源：http://hcr.sufxvd.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fke.tarul.cn

Ruby: s.length
来源：http://jdx.mhx1999.top

C#:   s.Length
来源：http://jqv.jqgfzy.top

[A23] 大小写转换
来源：http://ahr.yj20258888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gha.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fqe.jinqigfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jpm.sysykeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jfa.xingfuxueyuan.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ksg.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vtt.shzxlz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nwa.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bof.yongpay.top

[A24] 去除首尾空白
来源：http://ljh.hcnkem.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://awv.yfazqb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ipm.pycfn.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qer.andypj.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yyj.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://shd.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://evu.yangfankeji.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jvn.xuanzx.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://itz.zhoulong.xyz

[A25] 字符串比较
来源：http://yfz.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://umi.cdnleiting.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vzm.jqgfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oab.mhx1999.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://anq.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://arx.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yyk.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://svq.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bke.pycfn.com

[A26] 类型转换总览
来源：http://kje.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://axf.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kze.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cks.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://osl.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dgv.jinqigufen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hdl.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vjp.bbcook.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dkr.havefunace.top

================================================================================
来源：http://vrv.sufxvd.cn

B. 流程控制
来源：http://kzn.bbcook.cn

================================================================================
来源：http://kuv.cheryme.top

[B01] 条件判断 if / else
来源：http://wqs.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gai.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pew.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mrj.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nbp.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lye.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pqz.tarul.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ioa.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ccm.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://bgz.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lts.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bht.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://geb.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmf.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pqk.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://few.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jbj.meibo888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kqx.yueranfly.top

[B03] switch / match / case
来源：http://nzp.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tzu.zhaomingkeji.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cqv.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://suv.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xes.xingfuxueyuan.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ado.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bhj.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://txh.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sei.feifeiyinyue.top

[B04] for 计数循环
来源：http://umv.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://wuv.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bgl.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://abd.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tpa.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cmj.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ozp.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://vpc.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rgq.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://ust.aizwys.cn

Py:   for item in arr: print(item)
来源：http://fjb.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://clw.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ebw.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://scx.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://msf.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lky.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://zze.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rau.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://sbv.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rus.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cio.epnwcf.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hdg.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lug.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ljp.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nqp.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nee.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dnb.hnqzz.top

[B07] while 循环
来源：http://dzk.316326.xyz

Py:   while i < 10: i += 1
来源：http://aod.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://tiq.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://hfr.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://znx.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://vtw.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xwl.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://ill.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://bsj.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://lqq.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://jpk.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qyo.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://waf.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://mvu.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://ftw.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fvd.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://avw.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://fbu.jinqigufen.top

[B09] break 与 continue
来源：http://jtg.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ure.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://thf.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvl.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aef.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://opt.vqdsnc.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bpj.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://geu.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zzw.epnwcf.com

[B10] 遍历同时拿索引
来源：http://ycf.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oaf.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://myi.snrcjt.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uyd.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ayd.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fli.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pdn.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hfh.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jls.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://ivh.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://tig.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://mjz.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iok.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qif.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yjf.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://umg.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://qiz.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://byi.nwbrower.top

[B12] 跳出多层循环
来源：http://fvj.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://aql.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ktz.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lsp.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ptq.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qyu.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://esk.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wzw.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ist.daxiang520.top

[B13] 判断是否为数字
来源：http://scs.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://vxy.nwbrower.top

PHP:  is_numeric($x)
来源：http://rni.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nua.cashguo.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rsz.hywenlv.cn

Java: x instanceof Number
来源：http://eco.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://thp.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://ftb.ydzc1.top

C#:   x is int or double or decimal
来源：http://dqv.zdbjq.cn

[B14] 判断值是否在集合内
来源：http://lwd.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ijg.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dhi.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://tyv.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://ulh.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gzd.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nhy.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://vxp.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fyx.yonumen.top

[B15] 布尔运算与取反
来源：http://ffd.dianchejie.cn

Py:   a and b or not c
来源：http://ydu.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://ude.hnxiangtu.top

JS:   a && b || !c
来源：http://fit.0kj1m.cn

TS:   a && b || !c
来源：http://lzs.sxryk.cn

Java: a && b || !c
来源：http://jrt.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://wnc.ivvv.top

Ruby: a && b || !c
来源：http://clw.shanyushiyangtech.top

C#:   a && b || !c
来源：http://mwr.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://emb.jianghu66.top

Py:   if not data: return
来源：http://idu.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://xlv.shuidangran.top

JS:   if (!data) return;
来源：http://uwc.tarul.cn

TS:   if (!data) return;
来源：http://ewz.jinqigfzy.top

Java: if (data == null) return;
来源：http://mra.fzhhl.top

Go:   if data == nil { return }
来源：http://qtn.tianlin.xyz

Ruby: return if data.nil?
来源：http://mcq.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://pjh.tanke756.top

================================================================================
来源：http://ion.hnqzz.top

C. 函数与作用域
来源：http://tra.zhijiandao.cn

================================================================================
来源：http://ska.zhoulong.xyz

[C01] 定义函数
来源：http://sek.zhengqikj.top

Py:   def add(a, b): return a + b
来源：http://ruu.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jwh.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://fka.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gzv.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qqs.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://wou.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://ryr.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bjq.hnqzz.top

[C02] 默认参数
来源：http://com.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://qln.quarkkingdee.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xmd.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://uhj.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hnz.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://djq.xuetiantiany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sjz.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://pwd.jianghu66.top


<!-- 参考信息 -->