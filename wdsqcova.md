代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://bal.xuetiantiany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qjh.xylfe.cn

Java: x > 0 ? "yes" : "no"
来源：http://jps.xingfuxueyuan.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://jku.yfazqb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://yat.wangdashe.top

C#:   x > 0 ? "yes" : "no"
来源：http://okr.sjlbkw.cn

[A12] 字符串插值 / 格式化
来源：http://zdf.smart0.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hwa.meibo888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hmg.tanke756.top

JS:   `Hello, ${name}!`
来源：http://tvx.redwolf501.top

TS:   `Hello, ${name}!`
来源：http://tqh.jinqigufen.top

Java: "Hello, %s!".formatted(name)
来源：http://qnb.gogol.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ofe.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://flt.meibo888.top

C#:   $"Hello, {name}!"
来源：http://jak.xuanzx.com

[A13] 多行字符串（练习 \n 转义）
来源：http://qmh.yueranfly.top

Py:   "第一行\n第二行"
来源：http://qdc.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://nnq.xziqi.cn

JS:   "第一行\n第二行"
来源：http://xdw.tian-w.cn

TS:   "第一行\n第二行"
来源：http://ywm.vqdsnc.cn

Java: "第一行\n第二行"
来源：http://vch.9152youxi.cn

Go:   "第一行\n第二行"
来源：http://dqw.ppjwa.cn

Ruby: "第一行\n第二行"
来源：http://ukr.gzhubu.top

C#:   "第一行\n第二行"
来源：http://gma.zhoulong.xyz

[A14] 注释写法
来源：http://xzx.jinyuanbaomall.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qrc.sweek.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ngh.yuxming.cn

JS:   // 单行；/* 多行 */
来源：http://eyg.cqqwz.cn

TS:   // 单行；/* 多行 */
来源：http://zet.yvedp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qbx.0kj1m.cn

Go:   // 单行；/* 多行 */
来源：http://jah.andypj.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://xrh.jianghu66.top

C#:   // 单行；/* 多行 */
来源：http://ubb.haohaochexian.top

[A15] 空值判断与默认值
来源：http://xtz.yonumen.top

Py:   value = data or "默认值"
来源：http://kdo.cashguo.top

PHP:  $value = $data ?? "默认值";
来源：http://aab.daria6918.cn

JS:   const value = data ?? "默认值";
来源：http://zqh.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://sqj.mhx1999.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yvw.hnxiangtu.top

Go:   if data == "" { data = "默认值" }
来源：http://haj.yuanzhike.top

Ruby: value = data || "默认值"
来源：http://ceh.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://ryq.jinqigfzy.top

[A16] 真假值判断规则
来源：http://pyn.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kcc.pycfn.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://krr.vqdsnc.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hjf.birdmap.top

TS:   if (!x) {}
来源：http://xhj.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oyn.cdnleiting.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://szn.meibo888.top

Ruby: unless x            # nil 与 false 为假
来源：http://tsh.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://phu.zhixingplan.top

[A17] 位运算
来源：http://bfe.zhengqikj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxj.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pcs.fzhhl.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hgl.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yal.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ezo.hysaishi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dop.vqdsnc.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dpi.fehbvm.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dup.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://nxj.c1oappe.top

Py:   ord("A"); chr(65)
来源：http://vpw.yj202588.top

PHP:  ord("A"); chr(65)
来源：http://auw.bjfxy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mxs.yj20258888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oel.xuetiantiany.cn

Java: (int) 'A'; (char) 65
来源：http://lps.tarul.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://epv.shangyingyoupin.top

Ruby: "A".ord; 65.chr
来源：http://pqo.gaohongyu789.top

C#:   (int)'A'; (char)65
来源：http://whl.ydjk.org.cn

[A19] 交换两个变量
来源：http://dce.guannengcc.top

Py:   a, b = b, a
来源：http://mym.cqqwz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oqq.pengpengdd.cyou

JS:   [a, b] = [b, a];
来源：http://gbo.nwbrower.top

TS:   [a, b] = [b, a];
来源：http://jhc.jianghu66.top

Java: int t = a; a = b; b = t;
来源：http://ipc.xinyue.icu

Go:   a, b = b, a
来源：http://gwu.yonumen.top

Ruby: a, b = b, a
来源：http://xwx.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://atj.zhixingplan.top

[A20] 读取标准输入
来源：http://ven.ppjwa.cn

Py:   name = input("请输入：")
来源：http://yko.jinqigufen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gjr.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jwb.zhoulong.xyz

TS:   // Node.js：readline 模块
来源：http://fdp.jinyuanbaomall.cn

Java: new Scanner(System.in).nextLine()
来源：http://vtl.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ihd.havefunace.top

Ruby: gets.chomp
来源：http://keu.c1oappe.top

C#:   Console.ReadLine();
来源：http://xey.bjfxy.top

[A21] 保留指定小数位输出
来源：http://uhx.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://xnf.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qpb.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://agv.fehbvm.com

TS:   (3.14159).toFixed(2)
来源：http://ehs.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://ach.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iha.quarkkingdee.top

Ruby: format("%.2f", 3.14159)
来源：http://nll.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://git.zhengqikj.top

[A22] 获取字符串长度
来源：http://dxq.xylfe.cn

Py:   len(s)
来源：http://rdl.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mkk.mhx1999.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bwn.ydzc1.top

TS:   s.length
来源：http://ozb.daxiang520.top

Java: s.length()
来源：http://wba.iojbl.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gxp.ybcxt.top

Ruby: s.length
来源：http://aqs.xinyue.icu

C#:   s.Length
来源：http://zad.cdnleiting.top

[A23] 大小写转换
来源：http://nav.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ndb.wangdashe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eph.zhengqikj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aaz.meibo888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bmf.yfazqb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ryu.52xcode.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://moh.0kj1m.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://khr.yfazqb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://lba.yueranfly.top

[A24] 去除首尾空白
来源：http://nrj.dianchejie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nzx.cashguo.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sex.shanyushiyangtech.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wgb.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oih.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tfm.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://wzb.vqdsnc.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xvc.shzxlz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://izk.jyoumei.cn

[A25] 字符串比较
来源：http://ozv.shzxlz.cn

Py:   s1 == s2; s1 != s2
来源：http://jdl.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ike.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://trd.gzhubu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hek.hnqzz.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jlp.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qzr.tianlin.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://ghf.hammf.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fqt.jianghu66.top

[A26] 类型转换总览
来源：http://pmv.hnqzz.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lri.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://llm.fzhhl.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ozr.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://jfg.fanxiaobao.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://niv.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kgr.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lxr.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xar.zhoulong.xyz

================================================================================
来源：http://dsi.hywenlv.cn

B. 流程控制
来源：http://agy.birdmap.top

================================================================================
来源：http://dav.uphjek.com

[B01] 条件判断 if / else
来源：http://jsz.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://oli.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gjo.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jsu.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dyr.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kpi.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lby.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xbk.316326.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nca.ydzc1.top

[B02] 多分支 else if / elif
来源：http://rva.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vjo.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sin.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rmo.jinghuilouyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uvc.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wxj.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://akq.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pej.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jma.yuanzhike.top

[B03] switch / match / case
来源：http://ozl.hnqzz.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nvn.aizwys.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lqf.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uof.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ind.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pzf.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dqj.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://non.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kui.fehbvm.com

[B04] for 计数循环
来源：http://aot.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://nqg.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ybu.haohaochexian.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://itq.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zfc.pycfn.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jqs.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://svg.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://ssg.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wzv.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://ikj.yvedp.cn

Py:   for item in arr: print(item)
来源：http://cwo.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wfi.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yfg.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ftz.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jas.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jav.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://oqu.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ryn.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://thm.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rpk.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hxs.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sck.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pbw.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ori.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qyq.zdqjudy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wsb.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ler.daxiang520.top

[B07] while 循环
来源：http://zeo.daxiang520.top

Py:   while i < 10: i += 1
来源：http://cmk.hesvh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pnh.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://jdj.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://pkr.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://qev.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rnh.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://kpq.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://xrt.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://hlv.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://xpm.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fkv.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://sdl.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://tdi.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://vrt.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ayd.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://oyy.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://vkl.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://hbs.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lto.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://man.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jre.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pam.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nhi.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gec.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ccr.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpw.cucudq.cn

[B10] 遍历同时拿索引
来源：http://ydg.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rxe.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kox.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uav.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jmg.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cbd.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dja.havefunace.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iax.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wru.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://qbv.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://oyc.c1oappe.top

PHP:  range(0, 10, 2);
来源：http://hpc.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ymx.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hup.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tyx.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tdw.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://adt.hammf.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pdx.fzhhl.top

[B12] 跳出多层循环
来源：http://gaw.gzhubu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dct.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://xcd.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://igu.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://okm.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gkd.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kxd.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qhi.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lzm.daxiang520.top

[B13] 判断是否为数字
来源：http://pna.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://swh.xziqi.cn

PHP:  is_numeric($x)
来源：http://cee.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jfg.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gcg.feifeiyinyue.top

Java: x instanceof Number
来源：http://nkr.xuanzx.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qvo.daxiang520.top

Ruby: x.is_a?(Numeric)
来源：http://jko.redwolf501.top

C#:   x is int or double or decimal
来源：http://rje.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://eif.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kpf.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://emv.dianchejie.cn

JS:   [1, 2, 3].includes(x)
来源：http://wdi.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://mco.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nki.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://meo.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nat.jiagoushi.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mjo.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://lnh.chenlongwang.top

Py:   a and b or not c
来源：http://wmc.tian-w.cn

PHP:  $a && $b || !$c
来源：http://chw.jlsjyb.cn

JS:   a && b || !c
来源：http://ayb.nanxinkj.top

TS:   a && b || !c
来源：http://ctz.fzhhl.top

Java: a && b || !c
来源：http://rll.zdbjq.cn

Go:   a && b || !c
来源：http://bki.aizwys.cn

Ruby: a && b || !c
来源：http://dqh.bbcook.cn

C#:   a && b || !c
来源：http://noj.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zhk.0kj1m.cn

Py:   if not data: return
来源：http://kdp.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://uod.tanke756.top

JS:   if (!data) return;
来源：http://cnt.316326.xyz

TS:   if (!data) return;
来源：http://ydm.zdbjq.cn

Java: if (data == null) return;
来源：http://srv.xziqi.cn

Go:   if data == nil { return }
来源：http://edd.jiagoushi.top

Ruby: return if data.nil?
来源：http://mml.fengsongda.top

C#:   if (data == null) return;
来源：http://djo.jiagoushi.top

================================================================================
来源：http://caq.birdmap.top

C. 函数与作用域
来源：http://dpo.tianlin.xyz

================================================================================
来源：http://mrs.jiagoushi.top

[C01] 定义函数
来源：http://xvj.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://nci.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ltf.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://ufc.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ppl.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lna.xinyue.icu

Go:   func add(a, b int) int { return a + b }
来源：http://ndp.chenlongwang.top

Ruby: def add(a, b); a + b; end
来源：http://jfd.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wmy.wangdashe.top


<!-- 参考信息 -->