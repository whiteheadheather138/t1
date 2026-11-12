代发 wailian999

Java: "第一行\n第二行"
来源：http://eta.wangdashe.top

Go:   "第一行\n第二行"
来源：http://ezf.aizwys.cn

Ruby: "第一行\n第二行"
来源：http://eqi.ctjpmb.com

C#:   "第一行\n第二行"
来源：http://nhw.ctjpmb.com

[A14] 注释写法
来源：http://rjy.iojbl.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nyn.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://psi.nwbrower.top

JS:   // 单行；/* 多行 */
来源：http://esb.hnxiangtu.top

TS:   // 单行；/* 多行 */
来源：http://xva.havefunace.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ses.ybcxt.top

Go:   // 单行；/* 多行 */
来源：http://lsp.tanke756.top

Ruby: # 单行；=begin 多行 =end
来源：http://mqd.hysaishi.cn

C#:   // 单行；/* 多行 */
来源：http://rwj.daxiang520.top

[A15] 空值判断与默认值
来源：http://ref.9152youxi.cn

Py:   value = data or "默认值"
来源：http://ain.sufxvd.cn

PHP:  $value = $data ?? "默认值";
来源：http://vfv.ybcxt.top

JS:   const value = data ?? "默认值";
来源：http://bcx.hnxiangtu.top

TS:   const value = data ?? "默认值";
来源：http://dzw.gotoacloud.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ipm.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://oek.meibo888.top

Ruby: value = data || "默认值"
来源：http://pre.316326.xyz

C#:   var value = data ?? "默认值";
来源：http://iar.ppjwa.cn

[A16] 真假值判断规则
来源：http://mgn.mhx1999.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gfv.daxiang520.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://trd.ppjwa.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://esl.aibaodan.cn

TS:   if (!x) {}
来源：http://req.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bqz.aizwys.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://evj.yuanzhike.top

Ruby: unless x            # nil 与 false 为假
来源：http://beq.zhixingplan.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bhw.iojbl.cn

[A17] 位运算
来源：http://yod.sjlbkw.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwb.jinghuilouyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fkg.xziqi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yyw.hywenlv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bqa.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mvd.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ovg.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lnt.chenjidiqi.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xsx.aizwys.cn

[A18] 字符与 ASCII 码互转
来源：http://abc.cheryme.top

Py:   ord("A"); chr(65)
来源：http://wif.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://xss.zhongyouzk.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hcz.fktsv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://edy.quarkkingdee.top

Java: (int) 'A'; (char) 65
来源：http://dlf.yangfankeji.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gwr.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://sen.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://wol.hesvh.cn

[A19] 交换两个变量
来源：http://qjk.sufxvd.cn

Py:   a, b = b, a
来源：http://odo.zycfv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lgq.jinqigufen.top

JS:   [a, b] = [b, a];
来源：http://gvs.sufxvd.cn

TS:   [a, b] = [b, a];
来源：http://yop.yfazqb.com

Java: int t = a; a = b; b = t;
来源：http://iku.yvedp.cn

Go:   a, b = b, a
来源：http://lpg.hammf.cn

Ruby: a, b = b, a
来源：http://biw.svipenyu.cn

C#:   (a, b) = (b, a);
来源：http://dxy.sxryk.cn

[A20] 读取标准输入
来源：http://csi.c1oappe.top

Py:   name = input("请输入：")
来源：http://gog.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vun.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sha.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://aui.hammf.cn

Java: new Scanner(System.in).nextLine()
来源：http://rfs.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sco.cashguo.top

Ruby: gets.chomp
来源：http://srh.wangdashe.top

C#:   Console.ReadLine();
来源：http://hmr.meibo888.top

[A21] 保留指定小数位输出
来源：http://gva.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://rss.fktsv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hbs.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://ezi.hysaishi.cn

TS:   (3.14159).toFixed(2)
来源：http://jqa.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://zvt.hongshengwenyu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rup.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://ufs.cucudq.cn

C#:   3.14159.ToString("F2")
来源：http://fnb.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://imp.yuanzhike.top

Py:   len(s)
来源：http://fto.yj202588.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mmb.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nux.jinghuilouyu.cn

TS:   s.length
来源：http://wjr.epnwcf.com

Java: s.length()
来源：http://xgc.jqgfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://edt.gotoacloud.top

Ruby: s.length
来源：http://vkg.ydjk.org.cn

C#:   s.Length
来源：http://qpm.nanxinkj.top

[A23] 大小写转换
来源：http://npo.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xrw.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zlo.zhixingplan.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vet.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://egu.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zee.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fng.meibo888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tsh.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ige.ehwqpu.com

[A24] 去除首尾空白
来源：http://nqf.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mda.dashuyun.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jmt.shuidangran.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qta.shzxlz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ity.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oom.hysaishi.cn

Go:   strings.TrimSpace(s)
来源：http://rkg.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uwy.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kbe.hcnkem.com

[A25] 字符串比较
来源：http://gss.fktsv.cn

Py:   s1 == s2; s1 != s2
来源：http://zjp.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yyy.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yhi.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tqk.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vib.kuanghao11.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iih.gotoacloud.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hbo.yfazqb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ygz.nwbrower.top

[A26] 类型转换总览
来源：http://blg.tianlin.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jiy.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hxd.gotoacloud.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dlr.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://zkg.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kmf.hesvh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jvi.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://erl.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uwx.guannengcc.top

================================================================================
来源：http://ajy.yanxiufei.cn

B. 流程控制
来源：http://fem.aizwys.cn

================================================================================
来源：http://nnd.pycfn.com

[B01] 条件判断 if / else
来源：http://eec.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qmi.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oqj.yangfankeji.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zkb.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zfg.jiagoushi.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://awb.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qyk.xinyue.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xqt.ydzc1.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ydh.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://nqq.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eqb.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eyb.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ngq.jyoumei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qph.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayt.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iev.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://atl.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wny.chenzaomai.com

[B03] switch / match / case
来源：http://jbl.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tuq.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oqw.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fba.andypj.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nri.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nif.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xwu.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ipr.zhengqikj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vyg.hcnkem.com

[B04] for 计数循环
来源：http://hpa.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://iam.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kgk.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sxs.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lay.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nxy.svipenyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pvq.xuanzx.com

Ruby: 10.times { |i| puts i }
来源：http://jhx.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fiu.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://trw.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://ift.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nzb.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gvt.hesvh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gww.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ytd.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fvm.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://jye.hysaishi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gfd.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://zgd.yuanzhike.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ycq.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ind.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lxr.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ypf.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://age.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dyg.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xtr.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zsi.gaohongyu789.top

[B07] while 循环
来源：http://hah.sxryk.cn

Py:   while i < 10: i += 1
来源：http://ciu.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://lem.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://bem.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://xra.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://wpx.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rna.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://dxo.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://tmw.tanke756.top

[B08] do-while（至少执行一次）
来源：http://ngt.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://dqs.9152youxi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sos.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://uus.hongshengwenyu.top

TS:   do { i++; } while (i < 10);
来源：http://zsf.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://lom.kuanghao11.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ren.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://axp.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://kzk.vehdjk.com

[B09] break 与 continue
来源：http://naj.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eww.ydjk.org.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sfh.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zxv.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yox.cqqwz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqc.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fkz.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iur.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yqk.shuidangran.top

[B10] 遍历同时拿索引
来源：http://ssv.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vls.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dyz.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dze.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bxg.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bbn.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://abu.cashguo.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ffg.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://saa.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://wrj.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://gns.iojbl.cn

PHP:  range(0, 10, 2);
来源：http://fxy.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cdv.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ofo.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mxm.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gcs.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://wtx.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zvr.vehdjk.com

[B12] 跳出多层循环
来源：http://cuj.xinyue.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://lto.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ehr.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qpl.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zhf.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pel.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ehf.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ivy.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mcm.jyoumei.cn

[B13] 判断是否为数字
来源：http://gwl.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://sgt.gzhubu.top

PHP:  is_numeric($x)
来源：http://ppk.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://knz.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rxw.birdmap.top

Java: x instanceof Number
来源：http://grk.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sep.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://emu.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://yoi.fzhhl.top

[B14] 判断值是否在集合内
来源：http://aja.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eiq.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gby.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://wfz.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://rig.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://epr.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://npu.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://obg.havefunace.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hdh.meibo888.top

[B15] 布尔运算与取反
来源：http://znq.wangdashe.top

Py:   a and b or not c
来源：http://dku.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://cil.ydzc1.top

JS:   a && b || !c
来源：http://ygs.zhongyouzk.top

TS:   a && b || !c
来源：http://srd.tianlin.xyz

Java: a && b || !c
来源：http://lnu.zdbjq.cn

Go:   a && b || !c
来源：http://eln.shzxlz.cn

Ruby: a && b || !c
来源：http://wie.sweek.top

C#:   a && b || !c
来源：http://szg.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aro.wangdashe.top

Py:   if not data: return
来源：http://aax.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://kvl.jqgfzy.top

JS:   if (!data) return;
来源：http://npz.tianlin.xyz

TS:   if (!data) return;
来源：http://fuk.ybcxt.top

Java: if (data == null) return;
来源：http://awv.jqgufenzy.top

Go:   if data == nil { return }
来源：http://afr.jqgufenzy.top

Ruby: return if data.nil?
来源：http://zgh.hnxiangtu.top

C#:   if (data == null) return;
来源：http://kdm.zhaomingkeji.xyz

================================================================================
来源：http://gzy.52xcode.cn

C. 函数与作用域
来源：http://ctu.0kj1m.cn

================================================================================
来源：http://gqg.smart0.xyz

[C01] 定义函数
来源：http://qwn.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://qqy.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bsf.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://cgt.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqs.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ebt.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xqa.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://izl.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vas.yongpay.top

[C02] 默认参数
来源：http://zkl.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://uam.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mip.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://fdo.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iax.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hxe.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yun.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://dzo.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://plb.52xcode.cn

[C03] 可变参数
来源：http://ngk.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://sen.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pxo.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mtb.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://boo.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://osz.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cnr.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tcz.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rdb.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://yoq.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pxj.guowangkeji.top


<!-- 参考信息 -->