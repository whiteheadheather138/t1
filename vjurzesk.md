代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hkn.jlsjyb.cn

Ruby: "Hello, #{name}!"
来源：http://ihp.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://udn.yuanzhike.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hzz.zdqjudy.top

Py:   "第一行\n第二行"
来源：http://mwc.havefunace.top

PHP:  "第一行\n第二行"
来源：http://jvr.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://xwp.birdmap.top

TS:   "第一行\n第二行"
来源：http://txr.epnwcf.com

Java: "第一行\n第二行"
来源：http://opl.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://pts.shzxlz.cn

Ruby: "第一行\n第二行"
来源：http://vet.shangyingyoupin.top

C#:   "第一行\n第二行"
来源：http://zou.smart0.xyz

[A14] 注释写法
来源：http://guy.xinyue.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://xwk.tian-w.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uud.zhengqikj.top

JS:   // 单行；/* 多行 */
来源：http://rco.xingfuxueyuan.xyz

TS:   // 单行；/* 多行 */
来源：http://dhe.smart0.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mhk.jlsjyb.cn

Go:   // 单行；/* 多行 */
来源：http://fym.cheryme.top

Ruby: # 单行；=begin 多行 =end
来源：http://ogb.andypj.xyz

C#:   // 单行；/* 多行 */
来源：http://wro.wangshuangyany.cn

[A15] 空值判断与默认值
来源：http://ind.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://yvr.cqqwz.cn

PHP:  $value = $data ?? "默认值";
来源：http://kon.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://bur.yj20258.top

TS:   const value = data ?? "默认值";
来源：http://obg.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://opq.yonumen.top

Go:   if data == "" { data = "默认值" }
来源：http://tqe.nwbrower.top

Ruby: value = data || "默认值"
来源：http://dph.yvedp.cn

C#:   var value = data ?? "默认值";
来源：http://fqs.yuanzhike.top

[A16] 真假值判断规则
来源：http://nco.zhixingplan.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ywr.vqdsnc.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nyw.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lvo.yuxming.cn

TS:   if (!x) {}
来源：http://tvc.c1oappe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xeq.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ydh.jqgfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://mzx.redwolf501.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qld.cqqwz.cn

[A17] 位运算
来源：http://rdq.vqdsnc.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykl.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zol.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hfp.hnqzz.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ubi.daxiang520.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjb.vqdsnc.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pxk.dianchejie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://geb.zhaomingkeji.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qhu.yonumen.top

[A18] 字符与 ASCII 码互转
来源：http://fqf.gzhubu.top

Py:   ord("A"); chr(65)
来源：http://rko.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://xjq.jianghu66.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oor.jlsjyb.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qoc.zdqjudy.top

Java: (int) 'A'; (char) 65
来源：http://soh.tian-w.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pzq.xylfe.cn

Ruby: "A".ord; 65.chr
来源：http://ojs.xylfe.cn

C#:   (int)'A'; (char)65
来源：http://krp.yonumen.top

[A19] 交换两个变量
来源：http://bge.cqqwz.cn

Py:   a, b = b, a
来源：http://ani.yj20258888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mki.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://lca.sweek.top

TS:   [a, b] = [b, a];
来源：http://dho.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://lqi.chenzaomai.com

Go:   a, b = b, a
来源：http://mnl.aizwys.cn

Ruby: a, b = b, a
来源：http://hda.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://nsp.yanxiufei.cn

[A20] 读取标准输入
来源：http://zgt.guowangkeji.top

Py:   name = input("请输入：")
来源：http://bxp.yanxiufei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jki.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ibf.redwolf501.top

TS:   // Node.js：readline 模块
来源：http://qgh.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://lnu.guannengcc.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ayn.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://vve.gaohongyu789.top

C#:   Console.ReadLine();
来源：http://hyq.ivvv.top

[A21] 保留指定小数位输出
来源：http://vzl.sweek.top

Py:   f"{3.14159:.2f}"
来源：http://qet.gaohongyu789.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bik.xylfe.cn

JS:   (3.14159).toFixed(2)
来源：http://vom.xylfe.cn

TS:   (3.14159).toFixed(2)
来源：http://hek.hfpthk.cn

Java: String.format("%.2f", 3.14159)
来源：http://ojn.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dhn.jqgfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://lwh.jqgfzy.top

C#:   3.14159.ToString("F2")
来源：http://kuz.9152youxi.cn

[A22] 获取字符串长度
来源：http://gbo.yuxming.cn

Py:   len(s)
来源：http://zxa.tian-w.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qgm.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ohl.smart0.xyz

TS:   s.length
来源：http://vbm.ywan-chungtsiang.top

Java: s.length()
来源：http://cqd.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://clp.chenlongwang.top

Ruby: s.length
来源：http://ivr.cucudq.cn

C#:   s.Length
来源：http://juv.shanyushiyangkeji.top

[A23] 大小写转换
来源：http://obx.jiagoushi.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mic.cheryme.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nau.aizwys.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iqy.iojbl.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ney.nanxuanxn.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jgd.sweek.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yvx.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gqg.yj20258888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hde.fktsv.cn

[A24] 去除首尾空白
来源：http://xnj.quarkkingdee.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aea.chenjidiqi.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dds.hesvh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wru.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sgk.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lvp.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://cew.gzhubu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://goa.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ssl.ywan-chungtsiang.top

[A25] 字符串比较
来源：http://inz.yfazqb.com

Py:   s1 == s2; s1 != s2
来源：http://glh.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jcd.bjfxy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ofw.hongshengwenyu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kjo.ppjwa.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rxi.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://how.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://zgw.shuidangran.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bxe.daria6918.cn

[A26] 类型转换总览
来源：http://mmj.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yvd.ydjk.org.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tvn.nanxuanxn.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qbb.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://pne.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xbj.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cmm.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xmm.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xsg.fktsv.cn

================================================================================
来源：http://xlh.dianchejie.cn

B. 流程控制
来源：http://ffz.ywan-chungtsiang.top

================================================================================
来源：http://osr.zhongyouzk.top

[B01] 条件判断 if / else
来源：http://gmw.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tfx.xinyue.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ves.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ygv.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jbn.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qsh.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zvm.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wuz.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eem.zhoulong.xyz

[B02] 多分支 else if / elif
来源：http://pjc.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hki.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kvj.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uhu.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cte.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbx.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xzi.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lqc.yuxming.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krk.yj20258888.top

[B03] switch / match / case
来源：http://knb.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qum.jlsjyb.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eke.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://weq.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://max.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eug.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ueo.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yij.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vub.xziqi.cn

[B04] for 计数循环
来源：http://akc.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://qnq.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wnr.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xcg.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mpq.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xmb.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ihd.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://bni.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iuf.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://wtu.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://ock.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wgu.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yfv.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pfv.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kfb.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dwh.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://qwr.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mof.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://vec.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://acn.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://klu.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iyu.yvedp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qty.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xra.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://url.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sjk.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ynq.zhijiandao.cn

[B07] while 循环
来源：http://mxx.sysykeji.top

Py:   while i < 10: i += 1
来源：http://ltk.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://nvt.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://tjy.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://zcp.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://fjg.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vkk.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://npe.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://uxy.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://wwg.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://rxc.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://neo.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://lms.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://tru.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://rms.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yxq.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://rsp.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://oas.zdbjq.cn

[B09] break 与 continue
来源：http://vwb.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oqt.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://txo.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lqm.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ptd.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aow.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xpu.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gjw.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lje.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://fbm.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qbp.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://luo.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gsu.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tah.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://saw.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ava.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://byy.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cih.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://xti.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://sqm.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://izk.kuanghao11.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nzx.hnxiangtu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tsm.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://anq.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hua.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://ayy.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jit.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://med.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vmo.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mdd.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://muf.yvedp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ywj.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cxf.hammf.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pop.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zqy.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xwu.wangdashe.top

[B13] 判断是否为数字
来源：http://oas.gaohongyu789.top

Py:   isinstance(x, (int, float))
来源：http://tcn.c1oappe.top

PHP:  is_numeric($x)
来源：http://sxy.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cej.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://esh.feifeiyinyue.top

Java: x instanceof Number
来源：http://eyf.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qvo.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://rsf.hfpthk.cn

C#:   x is int or double or decimal
来源：http://frj.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://uhv.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://koq.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rzh.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://atk.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://rsi.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ceb.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://muy.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gfu.hnxiangtu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jzw.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://blw.ydzc1.top

Py:   a and b or not c
来源：http://yjh.guannengcc.top

PHP:  $a && $b || !$c
来源：http://ywg.yanxiufei.cn

JS:   a && b || !c
来源：http://tqd.hfpthk.cn

TS:   a && b || !c
来源：http://aec.fengsongda.top

Java: a && b || !c
来源：http://fnu.sxryk.cn

Go:   a && b || !c
来源：http://rrj.jinqigfzy.top

Ruby: a && b || !c
来源：http://lmb.jlsjyb.cn

C#:   a && b || !c
来源：http://jln.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://vxm.gogol.net.cn

Py:   if not data: return
来源：http://phk.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://mqm.cashguo.top

JS:   if (!data) return;
来源：http://low.fktsv.cn

TS:   if (!data) return;
来源：http://vtt.uphjek.com

Java: if (data == null) return;
来源：http://mml.0kj1m.cn

Go:   if data == nil { return }
来源：http://mhp.zycfv.cn

Ruby: return if data.nil?
来源：http://gxo.epnwcf.com

C#:   if (data == null) return;
来源：http://bfk.wangshuangyany.cn

================================================================================
来源：http://ehn.sufxvd.cn

C. 函数与作用域
来源：http://wbc.andypj.xyz

================================================================================
来源：http://tcr.tian-w.cn

[C01] 定义函数
来源：http://zfk.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://hnt.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yiv.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://wpc.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cam.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pvh.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dqw.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://vnx.sufxvd.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://llh.xuanzx.com

[C02] 默认参数
来源：http://rrr.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://vgx.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://knv.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://new.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ryq.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hev.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://trv.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://ehc.snrcjt.cn

C#:   string Greet(string name = "World") => name;
来源：http://pue.zhongyouzk.top

[C03] 可变参数
来源：http://hjc.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://sgb.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dqw.jinghuilouyu.cn


<!-- 参考信息 -->