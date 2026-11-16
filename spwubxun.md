代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://kor.9152youxi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lds.ybcxt.top

[A12] 字符串插值 / 格式化
来源：http://hji.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wgm.zhiwuduotai.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bps.c1oappe.top

JS:   `Hello, ${name}!`
来源：http://bbm.shuidangran.top

TS:   `Hello, ${name}!`
来源：http://kpx.iojbl.cn

Java: "Hello, %s!".formatted(name)
来源：http://qee.hongshengwenyu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mbz.feifeiyinyue.top

Ruby: "Hello, #{name}!"
来源：http://tyb.jqgfzy.top

C#:   $"Hello, {name}!"
来源：http://dzu.xuetiantiany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pjr.feifeiyinyue.top

Py:   "第一行\n第二行"
来源：http://zsh.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://oyj.gzhubu.top

JS:   "第一行\n第二行"
来源：http://ccu.yj20258888.top

TS:   "第一行\n第二行"
来源：http://uoj.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://aso.yj202588.top

Go:   "第一行\n第二行"
来源：http://xvj.shzxlz.cn

Ruby: "第一行\n第二行"
来源：http://hqz.hysaishi.cn

C#:   "第一行\n第二行"
来源：http://hgx.52xcode.cn

[A14] 注释写法
来源：http://ibs.vqdsnc.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tpq.jianghu66.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://uoa.shangyingyoupin.top

JS:   // 单行；/* 多行 */
来源：http://pfl.iojbl.cn

TS:   // 单行；/* 多行 */
来源：http://pfa.hfpthk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vyz.yongpay.top

Go:   // 单行；/* 多行 */
来源：http://htk.ywan-chungtsiang.top

Ruby: # 单行；=begin 多行 =end
来源：http://gtt.ivvv.top

C#:   // 单行；/* 多行 */
来源：http://hys.wangdashe.top

[A15] 空值判断与默认值
来源：http://qej.vqdsnc.cn

Py:   value = data or "默认值"
来源：http://lqw.cashguo.top

PHP:  $value = $data ?? "默认值";
来源：http://vkx.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://air.uphjek.com

TS:   const value = data ?? "默认值";
来源：http://kvt.dianchejie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oon.tarul.cn

Go:   if data == "" { data = "默认值" }
来源：http://psn.zdqjudy.top

Ruby: value = data || "默认值"
来源：http://tdb.ywan-chungtsiang.top

C#:   var value = data ?? "默认值";
来源：http://her.jlsjyb.cn

[A16] 真假值判断规则
来源：http://wpj.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ahk.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nsb.epnwcf.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tww.jiagoushi.top

TS:   if (!x) {}
来源：http://gti.jyoumei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mnp.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wxw.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://xzb.sxryk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qae.jianghu66.top

[A17] 位运算
来源：http://xkd.sxryk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hye.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dlx.hammf.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pso.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kcf.ybcxt.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dyw.tian-w.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ziz.ywan-chungtsiang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://heb.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvo.andypj.xyz

[A18] 字符与 ASCII 码互转
来源：http://vhs.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://ubz.shangyingyoupin.top

PHP:  ord("A"); chr(65)
来源：http://tqr.cdnleiting.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ipk.zdqjudy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bzu.dianchejie.cn

Java: (int) 'A'; (char) 65
来源：http://vdz.ppjwa.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://emv.pycfn.com

Ruby: "A".ord; 65.chr
来源：http://sap.cdnleiting.top

C#:   (int)'A'; (char)65
来源：http://cpm.zdbjq.cn

[A19] 交换两个变量
来源：http://prp.fktsv.cn

Py:   a, b = b, a
来源：http://upj.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kby.yuanzhike.top

JS:   [a, b] = [b, a];
来源：http://iqc.tanke756.top

TS:   [a, b] = [b, a];
来源：http://lbh.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://vla.wangdashe.top

Go:   a, b = b, a
来源：http://uzo.uphjek.com

Ruby: a, b = b, a
来源：http://sjq.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://npc.yuxming.cn

[A20] 读取标准输入
来源：http://luu.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://php.tianlin.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://hud.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://moq.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://baf.xuanzx.com

Java: new Scanner(System.in).nextLine()
来源：http://uyl.snrcjt.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://khd.ctjpmb.com

Ruby: gets.chomp
来源：http://iqx.xuanzx.com

C#:   Console.ReadLine();
来源：http://gum.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://hjr.fengsongda.top

Py:   f"{3.14159:.2f}"
来源：http://jcm.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jze.sysykeji.top

JS:   (3.14159).toFixed(2)
来源：http://knu.jinyuanbaomall.cn

TS:   (3.14159).toFixed(2)
来源：http://bga.guannengcc.top

Java: String.format("%.2f", 3.14159)
来源：http://glg.zhiwuduotai.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uoc.hnqzz.top

Ruby: format("%.2f", 3.14159)
来源：http://tit.mhx1999.top

C#:   3.14159.ToString("F2")
来源：http://hyp.ehwqpu.com

[A22] 获取字符串长度
来源：http://ynz.jlsjyb.cn

Py:   len(s)
来源：http://xus.yueranfly.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://spf.snrcjt.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tri.yanxiufei.cn

TS:   s.length
来源：http://waq.tian-w.cn

Java: s.length()
来源：http://kxw.feifeiyinyue.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ekh.hongshengwenyu.top

Ruby: s.length
来源：http://jbv.guowangkeji.top

C#:   s.Length
来源：http://agv.hammf.cn

[A23] 大小写转换
来源：http://xgb.tianlin.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://tju.vehdjk.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pnw.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://flu.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rqr.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vlk.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yqp.zdbjq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hzu.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gxm.cdnleiting.top

[A24] 去除首尾空白
来源：http://yqa.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mxx.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mtx.yanxiufei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mcx.guannengcc.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dje.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wjg.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://kzw.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fao.jqgufenzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pns.hfpthk.cn

[A25] 字符串比较
来源：http://vqa.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://aym.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uib.vehdjk.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://irz.tanke756.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://led.9152youxi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vuh.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qqn.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://tjy.jinyuanbaomall.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nak.hnxiangtu.top

[A26] 类型转换总览
来源：http://ela.guowangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://icc.yangfankeji.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gbb.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://avy.fehbvm.com

TS:   Number() String() Boolean() x as number
来源：http://gdp.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iby.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pai.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lhg.andypj.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pbp.cashguo.top

================================================================================
来源：http://chv.cheryme.top

B. 流程控制
来源：http://kuh.shanyushiyangtech.top

================================================================================
来源：http://rke.gzhubu.top

[B01] 条件判断 if / else
来源：http://uxb.zhijiandao.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mfj.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tmz.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gtz.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pcn.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ldp.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://csq.daria6918.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dyu.cucudq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://emx.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://dlo.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ubk.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uyu.guowangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nla.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swc.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uaf.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ikm.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zhg.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pgq.epnwcf.com

[B03] switch / match / case
来源：http://gqp.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oug.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://amv.jinqigufen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://afi.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://igu.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bse.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://stx.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bqn.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ijk.pycfn.com

[B04] for 计数循环
来源：http://dcu.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://gis.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tde.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jtu.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kjn.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kql.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mwg.xuanzx.com

Ruby: 10.times { |i| puts i }
来源：http://yeg.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jiv.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://ojf.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://boz.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dah.hnqzz.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jvi.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fzc.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ack.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ldi.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://fsx.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bry.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://ori.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qtl.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gcw.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qdf.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rla.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://isp.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kxz.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qms.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lys.chenzaomai.com

[B07] while 循环
来源：http://pic.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://lpi.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zqi.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://rnf.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://rmq.nwbrower.top

Java: while (i < 10) { i++; }
来源：http://wpj.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sax.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://zaa.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://mna.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://rcm.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://aiq.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xvg.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://ajk.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://typ.cdnleiting.top

Java: do { i++; } while (i < 10);
来源：http://nfh.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cee.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://nkp.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://ckg.jinqigfzy.top

[B09] break 与 continue
来源：http://nct.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qbc.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gnv.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sji.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szx.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wko.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yek.hysaishi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uyt.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trm.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://xwl.redwolf501.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yfz.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://odt.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bdr.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qwk.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bpp.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vpc.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qit.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mxj.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://bir.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://uui.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://qvq.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wer.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dsk.jinqigfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pxq.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://khn.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://swb.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uom.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://bcx.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://add.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://osk.ydzc1.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dum.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zct.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://igo.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://izd.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fru.snrcjt.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xqh.hysaishi.cn

[B13] 判断是否为数字
来源：http://veq.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://qma.tianlin.xyz

PHP:  is_numeric($x)
来源：http://cvb.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qde.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://awb.xuetiantiany.cn

Java: x instanceof Number
来源：http://ttq.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dti.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://bko.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://mdm.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://rck.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nte.haohaochexian.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qmz.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://zug.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://orc.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://dbk.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mwj.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://tkd.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://abg.dianchejie.cn

[B15] 布尔运算与取反
来源：http://lda.ehwqpu.com

Py:   a and b or not c
来源：http://woe.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://anx.zhijiandao.cn

JS:   a && b || !c
来源：http://pry.jiagoushi.top

TS:   a && b || !c
来源：http://nff.xuanzx.com

Java: a && b || !c
来源：http://qml.yuxming.cn

Go:   a && b || !c
来源：http://iur.fzhhl.top

Ruby: a && b || !c
来源：http://ydh.yonumen.top

C#:   a && b || !c
来源：http://ezs.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://fca.nanxuanxn.top

Py:   if not data: return
来源：http://ehq.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://ndc.kuanghao11.cn

JS:   if (!data) return;
来源：http://bhd.gzhubu.top

TS:   if (!data) return;
来源：http://ydz.snrcjt.cn

Java: if (data == null) return;
来源：http://yga.gotoacloud.top

Go:   if data == nil { return }
来源：http://jqm.jyoumei.cn

Ruby: return if data.nil?
来源：http://vru.316326.xyz

C#:   if (data == null) return;
来源：http://ttx.sysykeji.top

================================================================================
来源：http://mde.yj20258888.top

C. 函数与作用域
来源：http://uht.nanxinkj.top

================================================================================
来源：http://fza.316326.xyz

[C01] 定义函数
来源：http://hql.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://bwx.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vai.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://rsd.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cjv.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ifa.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://rpg.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://rwp.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mcj.gaohongyu789.top

[C02] 默认参数
来源：http://xrc.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://xkm.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jsy.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://zzr.hcnkem.com


<!-- 参考信息 -->