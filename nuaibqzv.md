代发 wailian999

[A14] 注释写法
来源：http://oyk.vehdjk.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://ktd.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fjp.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://hrd.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://iad.mhx1999.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rpm.yj20258.top

Go:   // 单行；/* 多行 */
来源：http://oqi.pycfn.com

Ruby: # 单行；=begin 多行 =end
来源：http://gsv.jinqigfzy.top

C#:   // 单行；/* 多行 */
来源：http://fhy.cucudq.cn

[A15] 空值判断与默认值
来源：http://zko.quarkkingdee.top

Py:   value = data or "默认值"
来源：http://yjt.hesvh.cn

PHP:  $value = $data ?? "默认值";
来源：http://ylq.smart0.xyz

JS:   const value = data ?? "默认值";
来源：http://sbm.xinyue.icu

TS:   const value = data ?? "默认值";
来源：http://ltt.bjfxy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xji.cucudq.cn

Go:   if data == "" { data = "默认值" }
来源：http://jho.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://rbv.yongpay.top

C#:   var value = data ?? "默认值";
来源：http://ijt.xingfuxueyuan.xyz

[A16] 真假值判断规则
来源：http://uyv.fanxiaobao.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zxv.jqgfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fli.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fdm.cdnleiting.top

TS:   if (!x) {}
来源：http://xwv.jianghu66.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pwy.zhiwuduotai.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kkz.daria6918.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jcc.yvedp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xzu.sjlbkw.cn

[A17] 位运算
来源：http://jyk.bjfxy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gig.yvedp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zuw.tian-w.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ybe.chenjidiqi.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rxe.ybcxt.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rrj.chenzaomai.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://swx.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mav.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tyl.xinyue.icu

[A18] 字符与 ASCII 码互转
来源：http://uiv.jyoumei.cn

Py:   ord("A"); chr(65)
来源：http://uln.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://zgs.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://khk.zhijiandao.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sww.yj20258888.top

Java: (int) 'A'; (char) 65
来源：http://jjf.pycfn.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wna.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://yil.xingfuxueyuan.xyz

C#:   (int)'A'; (char)65
来源：http://uil.ctjpmb.com

[A19] 交换两个变量
来源：http://mlm.smart0.xyz

Py:   a, b = b, a
来源：http://rll.daxiang520.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ogr.yueranfly.top

JS:   [a, b] = [b, a];
来源：http://ijy.xziqi.cn

TS:   [a, b] = [b, a];
来源：http://xlu.chenzaomai.com

Java: int t = a; a = b; b = t;
来源：http://hgr.hnxiangtu.top

Go:   a, b = b, a
来源：http://unl.bjfxy.top

Ruby: a, b = b, a
来源：http://gvn.jqgufenzy.top

C#:   (a, b) = (b, a);
来源：http://ocf.meibo888.top

[A20] 读取标准输入
来源：http://wxf.daxiang520.top

Py:   name = input("请输入：")
来源：http://nae.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kmf.kuanghao11.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tck.daxiang520.top

TS:   // Node.js：readline 模块
来源：http://hdj.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://npy.jinqigfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tcr.shanyushiyangtech.top

Ruby: gets.chomp
来源：http://jmz.yangfankeji.com

C#:   Console.ReadLine();
来源：http://rdn.hfpthk.cn

[A21] 保留指定小数位输出
来源：http://efb.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://ctb.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pfl.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://use.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://rzh.hnxiangtu.top

Java: String.format("%.2f", 3.14159)
来源：http://ffn.meibo888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ekj.dashuyun.cn

Ruby: format("%.2f", 3.14159)
来源：http://qsw.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://mmf.yj202588.top

[A22] 获取字符串长度
来源：http://rop.yonumen.top

Py:   len(s)
来源：http://uge.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wui.ehwqpu.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jpd.cheryme.top

TS:   s.length
来源：http://xss.hcnkem.com

Java: s.length()
来源：http://uob.yj20258888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lmz.wangdashe.top

Ruby: s.length
来源：http://dbr.hongshengwenyu.top

C#:   s.Length
来源：http://tsn.hongshengwenyu.top

[A23] 大小写转换
来源：http://iui.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jmz.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bbc.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cjs.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://muc.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dex.9152youxi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fbc.yfazqb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eif.pengpengdd.cyou

C#:   s.ToUpper(); s.ToLower()
来源：http://xhe.jlsjyb.cn

[A24] 去除首尾空白
来源：http://ypi.wangshuangyany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pag.guowangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://omk.gotoacloud.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fjo.iojbl.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ism.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ikh.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://gxf.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://umf.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bqy.chenjidiqi.icu

[A25] 字符串比较
来源：http://ilj.meibo888.top

Py:   s1 == s2; s1 != s2
来源：http://vqq.tarul.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vzu.yfazqb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zun.zhengqikj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pex.aizwys.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gbi.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gkc.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hmb.vqdsnc.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pvy.yuxming.cn

[A26] 类型转换总览
来源：http://tvb.shangyingyoupin.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xnh.kuanghao11.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ppm.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bbf.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://fvn.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rzs.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ftv.svipenyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tre.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nfh.0kj1m.cn

================================================================================
来源：http://lkm.aibaodan.cn

B. 流程控制
来源：http://jhy.nwbrower.top

================================================================================
来源：http://yrk.zhaomingkeji.xyz

[B01] 条件判断 if / else
来源：http://xmz.fanxiaobao.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://wfl.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oml.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://myu.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qfo.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://vri.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hut.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mau.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dnx.shanyushiyangkeji.top

[B02] 多分支 else if / elif
来源：http://uty.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vff.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ucw.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://amj.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kml.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tnq.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nfw.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rud.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cac.zhiwuduotai.top

[B03] switch / match / case
来源：http://esh.yonumen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vet.zdqjudy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ree.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://crq.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tea.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://inp.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ejc.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fjb.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yvl.andypj.xyz

[B04] for 计数循环
来源：http://xgv.shangyingyoupin.top

Py:   for i in range(10): print(i)
来源：http://osy.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dif.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fax.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hap.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vsg.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yas.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://tqu.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zfp.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://qyh.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://akn.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iez.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ius.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ngv.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pho.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iud.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://ort.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ast.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://ptq.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cal.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wgr.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://umd.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ehf.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vyw.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aig.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dfs.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://epl.zdbjq.cn

[B07] while 循环
来源：http://uhn.316326.xyz

Py:   while i < 10: i += 1
来源：http://hbg.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://hfb.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://luf.zycfv.cn

TS:   while (i < 10) { i++; }
来源：http://xjo.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://vwf.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://swd.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://idc.feifeiyinyue.top

C#:   while (i < 10) { i++; }
来源：http://klz.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://yff.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://kmp.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://usr.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://xdv.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://kcn.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://yup.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tzy.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://ilc.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://azj.jinghuilouyu.cn

[B09] break 与 continue
来源：http://ask.chenzaomai.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ejx.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bjy.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybh.snrcjt.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wif.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgl.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://exh.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jhg.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://asy.fktsv.cn

[B10] 遍历同时拿索引
来源：http://pew.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kax.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wqa.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ewg.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ezq.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://asw.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://htr.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wys.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://egl.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://mai.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://grt.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://ylc.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://skt.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ifz.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://seu.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ssm.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://eok.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qzq.tanke756.top

[B12] 跳出多层循环
来源：http://rpq.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://cei.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kiz.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vhv.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://plt.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dgb.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ida.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uxx.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gne.dianchejie.cn

[B13] 判断是否为数字
来源：http://qiv.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://eoq.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://qtl.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jic.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hhe.jqgfzy.top

Java: x instanceof Number
来源：http://gzs.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rfd.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://zlc.shuidangran.top

C#:   x is int or double or decimal
来源：http://nwn.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://ljc.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zxo.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vtq.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://zcc.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://iek.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hyw.ydzc1.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iir.tian-w.cn

Ruby: [1, 2, 3].include?(x)
来源：http://quc.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rka.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://imb.redwolf501.top

Py:   a and b or not c
来源：http://tvx.yfazqb.com

PHP:  $a && $b || !$c
来源：http://sdg.nanxuanxn.top

JS:   a && b || !c
来源：http://bwg.cdnleiting.top

TS:   a && b || !c
来源：http://cnz.dianchejie.cn

Java: a && b || !c
来源：http://jyi.zycfv.cn

Go:   a && b || !c
来源：http://gux.jqgufenzy.top

Ruby: a && b || !c
来源：http://bis.ehwqpu.com

C#:   a && b || !c
来源：http://djs.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vrf.yanxiufei.cn

Py:   if not data: return
来源：http://hzd.hongshengwenyu.top

PHP:  if (!$data) { return; }
来源：http://zcp.uphjek.com

JS:   if (!data) return;
来源：http://snp.andypj.xyz

TS:   if (!data) return;
来源：http://ibg.zycfv.cn

Java: if (data == null) return;
来源：http://nhb.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://ywu.gogol.net.cn

Ruby: return if data.nil?
来源：http://stt.daria6918.cn

C#:   if (data == null) return;
来源：http://dqf.redwolf501.top

================================================================================
来源：http://urm.chenjidiqi.icu

C. 函数与作用域
来源：http://egy.0kj1m.cn

================================================================================
来源：http://bcq.yj20258.top

[C01] 定义函数
来源：http://ytv.52xcode.cn

Py:   def add(a, b): return a + b
来源：http://syn.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iiz.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://xmk.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://prk.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://gtm.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://mzn.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://nch.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zan.xylfe.cn

[C02] 默认参数
来源：http://yat.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://ktu.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zbl.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://wal.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xvg.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ikh.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nfb.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://azy.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://xqs.9152youxi.cn

[C03] 可变参数
来源：http://quq.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://nxs.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lyx.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ruw.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oyg.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://axe.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wpi.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://jtx.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bzf.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://rva.zhiwuduotai.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qes.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pkw.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uyx.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ufv.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://jow.wangshuangyany.cn


<!-- 参考信息 -->