代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://gta.yj20258.top

C#:   x > 0 ? "yes" : "no"
来源：http://bae.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://dgf.quarkkingdee.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uex.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xtz.yj202588.top

JS:   `Hello, ${name}!`
来源：http://ntr.hysaishi.cn

TS:   `Hello, ${name}!`
来源：http://kso.yj202588.top

Java: "Hello, %s!".formatted(name)
来源：http://glo.jinyuanbaomall.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://osj.feifeiyinyue.top

Ruby: "Hello, #{name}!"
来源：http://iwi.hammf.cn

C#:   $"Hello, {name}!"
来源：http://waf.feifeiyinyue.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mnz.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://ucv.c1oappe.top

PHP:  "第一行\n第二行"
来源：http://rhp.hammf.cn

JS:   "第一行\n第二行"
来源：http://tyv.jlsjyb.cn

TS:   "第一行\n第二行"
来源：http://ldw.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://cyn.chenzaomai.com

Go:   "第一行\n第二行"
来源：http://sit.yongpay.top

Ruby: "第一行\n第二行"
来源：http://pxm.vqdsnc.cn

C#:   "第一行\n第二行"
来源：http://hkj.zhixingplan.top

[A14] 注释写法
来源：http://jtw.fengsongda.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://yii.jqgfzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xbk.jinyuanbaomall.cn

JS:   // 单行；/* 多行 */
来源：http://phn.cucudq.cn

TS:   // 单行；/* 多行 */
来源：http://sbt.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fxg.0kj1m.cn

Go:   // 单行；/* 多行 */
来源：http://eop.iojbl.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xsb.fengsongda.top

C#:   // 单行；/* 多行 */
来源：http://bvk.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://prb.wangdashe.top

Py:   value = data or "默认值"
来源：http://aya.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://tox.ctjpmb.com

JS:   const value = data ?? "默认值";
来源：http://gly.birdmap.top

TS:   const value = data ?? "默认值";
来源：http://gne.hysaishi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tzk.hfpthk.cn

Go:   if data == "" { data = "默认值" }
来源：http://cml.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://iks.vehdjk.com

C#:   var value = data ?? "默认值";
来源：http://ygt.jianghu66.top

[A16] 真假值判断规则
来源：http://bgf.316326.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fki.haohaochexian.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tvb.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wyf.ctjpmb.com

TS:   if (!x) {}
来源：http://ywx.redwolf501.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ljb.tian-w.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cvf.yongpay.top

Ruby: unless x            # nil 与 false 为假
来源：http://zve.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dgc.svipenyu.cn

[A17] 位运算
来源：http://exs.redwolf501.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://deg.jinghuilouyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uzn.cucudq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://psh.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rcj.iojbl.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nnd.epnwcf.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yde.jqgufenzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ahp.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://obe.yfazqb.com

[A18] 字符与 ASCII 码互转
来源：http://ull.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://kdk.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://jva.jinyuanbaomall.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jgs.zhengqikj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aln.tanke756.top

Java: (int) 'A'; (char) 65
来源：http://hen.jiagoushi.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qvo.aibaodan.cn

Ruby: "A".ord; 65.chr
来源：http://doa.cheryme.top

C#:   (int)'A'; (char)65
来源：http://sns.gzhubu.top

[A19] 交换两个变量
来源：http://ofw.sufxvd.cn

Py:   a, b = b, a
来源：http://jqi.chenjidiqi.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://ozp.shanyushiyangtech.top

JS:   [a, b] = [b, a];
来源：http://alt.yonumen.top

TS:   [a, b] = [b, a];
来源：http://tzw.vqdsnc.cn

Java: int t = a; a = b; b = t;
来源：http://aex.ctjpmb.com

Go:   a, b = b, a
来源：http://wzw.ydzc1.top

Ruby: a, b = b, a
来源：http://kmb.xingfuxueyuan.xyz

C#:   (a, b) = (b, a);
来源：http://avt.meibo888.top

[A20] 读取标准输入
来源：http://qid.sweek.top

Py:   name = input("请输入：")
来源：http://sld.zhongyouzk.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kmt.cdnleiting.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bqy.wangdashe.top

TS:   // Node.js：readline 模块
来源：http://tqh.daria6918.cn

Java: new Scanner(System.in).nextLine()
来源：http://tnn.xuanzx.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rog.uphjek.com

Ruby: gets.chomp
来源：http://wlo.zdbjq.cn

C#:   Console.ReadLine();
来源：http://zov.fzhhl.top

[A21] 保留指定小数位输出
来源：http://hbd.aibaodan.cn

Py:   f"{3.14159:.2f}"
来源：http://dxd.chenjidiqi.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://atx.hnxiangtu.top

JS:   (3.14159).toFixed(2)
来源：http://pvt.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://eqq.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://mpz.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bqv.cqqwz.cn

Ruby: format("%.2f", 3.14159)
来源：http://bcs.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://ktd.yfazqb.com

[A22] 获取字符串长度
来源：http://nmo.sysykeji.top

Py:   len(s)
来源：http://tlc.ydzc1.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hxl.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hgd.fehbvm.com

TS:   s.length
来源：http://wpj.yvedp.cn

Java: s.length()
来源：http://qfn.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uhk.jinqigufen.top

Ruby: s.length
来源：http://trb.nanxinkj.top

C#:   s.Length
来源：http://shr.havefunace.top

[A23] 大小写转换
来源：http://mqz.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://zvj.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ssz.vehdjk.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bup.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ans.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wcp.pycfn.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://isw.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gad.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vix.tanke756.top

[A24] 去除首尾空白
来源：http://yeb.xinyue.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fro.zdqjudy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://buy.pycfn.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ksc.hysaishi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://akm.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fws.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://dlj.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mgd.hnqzz.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ugt.meibo888.top

[A25] 字符串比较
来源：http://tzb.aizwys.cn

Py:   s1 == s2; s1 != s2
来源：http://iyd.fehbvm.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tao.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tsz.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mfz.ybcxt.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vck.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wsn.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://vpb.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lvu.zhiwuduotai.top

[A26] 类型转换总览
来源：http://myq.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://abr.dashuyun.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ncp.nanxuanxn.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xtc.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://syj.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wtp.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mmw.uphjek.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://bos.cashguo.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ixt.kuanghao11.cn

================================================================================
来源：http://uti.mhx1999.top

B. 流程控制
来源：http://knz.fehbvm.com

================================================================================
来源：http://vtn.guowangkeji.top

[B01] 条件判断 if / else
来源：http://gpj.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://bpu.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uje.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mqw.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ntr.yj20258.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ciq.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://umo.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mpo.zhiwuduotai.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gwl.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://vpi.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://biq.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wza.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tzy.cdnleiting.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kcg.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zdj.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://koi.sweek.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yry.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gqo.nanxuanxn.top

[B03] switch / match / case
来源：http://fmp.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cce.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qqt.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iyq.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hkc.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lji.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bja.hcnkem.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fje.yangfankeji.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ppj.hfpthk.cn

[B04] for 计数循环
来源：http://hzq.tanke756.top

Py:   for i in range(10): print(i)
来源：http://hml.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qcv.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://obe.hysaishi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://irp.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://amc.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tjm.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://amz.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rwf.hammf.cn

[B05] 遍历数组 / 列表
来源：http://kom.cheryme.top

Py:   for item in arr: print(item)
来源：http://ixx.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dgh.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://tcg.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rnh.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mic.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zye.hammf.cn

Ruby: arr.each { |item| puts item }
来源：http://sgq.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zwb.hammf.cn

[B06] 遍历字典 / 对象
来源：http://exf.jinghuilouyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ysd.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yxo.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://utd.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nnx.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://osl.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ezs.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gzb.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vfi.fzhhl.top

[B07] while 循环
来源：http://dsc.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://qiq.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gwg.yonumen.top

JS:   while (i < 10) { i++; }
来源：http://dkj.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://irs.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://gnl.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eez.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://fpc.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://oym.gogol.net.cn

[B08] do-while（至少执行一次）
来源：http://rkg.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://fgh.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xkf.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://faf.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://gbo.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://bex.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://hye.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xjw.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://dkf.jiagoushi.top

[B09] break 与 continue
来源：http://eaq.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ust.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nva.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aon.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wsu.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qbi.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qgl.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fok.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tdl.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://wqy.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://osf.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oyg.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iht.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lkw.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uoy.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lzr.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hce.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://umw.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://xdj.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://yxo.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://prm.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zbs.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dnu.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yfb.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pyy.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://njm.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qdx.jyoumei.cn

[B12] 跳出多层循环
来源：http://nar.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://set.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zkd.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oct.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tlf.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ryd.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cse.sufxvd.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mzj.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pkw.hysaishi.cn

[B13] 判断是否为数字
来源：http://kdy.meibo888.top

Py:   isinstance(x, (int, float))
来源：http://amb.andypj.xyz

PHP:  is_numeric($x)
来源：http://ipj.redwolf501.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://itr.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qkj.shanyushiyangtech.top

Java: x instanceof Number
来源：http://ajd.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nmj.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://zsu.andypj.xyz

C#:   x is int or double or decimal
来源：http://dez.tanke756.top

[B14] 判断值是否在集合内
来源：http://yhm.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ohl.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lak.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://xjt.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://hjl.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yap.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pns.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://avs.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://smr.guowangkeji.top

[B15] 布尔运算与取反
来源：http://blr.vqdsnc.cn

Py:   a and b or not c
来源：http://zlc.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://oyx.52xcode.cn

JS:   a && b || !c
来源：http://acj.hnqzz.top

TS:   a && b || !c
来源：http://vdg.yueranfly.top

Java: a && b || !c
来源：http://djz.zhijiandao.cn

Go:   a && b || !c
来源：http://lwn.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://sud.vqdsnc.cn

C#:   a && b || !c
来源：http://xvs.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://jlq.chenjidiqi.icu

Py:   if not data: return
来源：http://mcn.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://fvb.shuidangran.top

JS:   if (!data) return;
来源：http://zwg.sjlbkw.cn

TS:   if (!data) return;
来源：http://shh.daria6918.cn

Java: if (data == null) return;
来源：http://bml.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://rrx.cqqwz.cn

Ruby: return if data.nil?
来源：http://syu.shzxlz.cn

C#:   if (data == null) return;
来源：http://pjp.xuetiantiany.cn

================================================================================
来源：http://lkb.chenjidiqi.icu

C. 函数与作用域
来源：http://rlw.zhiwuduotai.top

================================================================================
来源：http://soe.daria6918.cn

[C01] 定义函数
来源：http://zoy.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://sbd.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qca.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://gua.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rne.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jjj.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://hbc.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://fvk.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qpy.gogol.net.cn

[C02] 默认参数
来源：http://tbj.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://gzo.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qdp.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://dgb.xinyue.icu


<!-- 参考信息 -->