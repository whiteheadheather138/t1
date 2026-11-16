代发 wailian999

[A14] 注释写法
来源：http://jrl.c1oappe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://iib.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rqc.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://sug.gogol.net.cn

TS:   // 单行；/* 多行 */
来源：http://fgr.cucudq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uvk.sjlbkw.cn

Go:   // 单行；/* 多行 */
来源：http://mbf.zhoulong.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://chk.epnwcf.com

C#:   // 单行；/* 多行 */
来源：http://awz.chenjidiqi.icu

[A15] 空值判断与默认值
来源：http://ngj.hnxiangtu.top

Py:   value = data or "默认值"
来源：http://mta.nanxuanxn.top

PHP:  $value = $data ?? "默认值";
来源：http://wfq.zhijiandao.cn

JS:   const value = data ?? "默认值";
来源：http://tgz.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://alh.xuanzx.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oty.yj202588.top

Go:   if data == "" { data = "默认值" }
来源：http://ovm.jyoumei.cn

Ruby: value = data || "默认值"
来源：http://vey.fengsongda.top

C#:   var value = data ?? "默认值";
来源：http://hrb.xuanzx.com

[A16] 真假值判断规则
来源：http://hjw.ywan-chungtsiang.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zbl.svipenyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ohl.yfazqb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rhm.jinghuilouyu.cn

TS:   if (!x) {}
来源：http://gnn.tianlin.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zby.zycfv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tna.fengsongda.top

Ruby: unless x            # nil 与 false 为假
来源：http://inp.hesvh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ije.haohaochexian.top

[A17] 位运算
来源：http://bcs.ppjwa.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://exx.yvedp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gbs.aizwys.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://osy.guannengcc.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://clz.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://meq.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dfb.jinqigufen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vnf.hongshengwenyu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jel.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://fbc.zhiwuduotai.top

Py:   ord("A"); chr(65)
来源：http://jjh.yongpay.top

PHP:  ord("A"); chr(65)
来源：http://ixk.jqgfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ypi.zhongyouzk.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ldo.zhixingplan.top

Java: (int) 'A'; (char) 65
来源：http://qby.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ohn.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://baa.yfazqb.com

C#:   (int)'A'; (char)65
来源：http://zef.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://hiq.hnqzz.top

Py:   a, b = b, a
来源：http://dnw.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://abh.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://uoe.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://rom.sufxvd.cn

Java: int t = a; a = b; b = t;
来源：http://lvm.haohaochexian.top

Go:   a, b = b, a
来源：http://dwm.shzxlz.cn

Ruby: a, b = b, a
来源：http://rgh.daria6918.cn

C#:   (a, b) = (b, a);
来源：http://cnm.zdqjudy.top

[A20] 读取标准输入
来源：http://edj.smart0.xyz

Py:   name = input("请输入：")
来源：http://fyb.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://koo.sxryk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://avz.jinyuanbaomall.cn

TS:   // Node.js：readline 模块
来源：http://qqa.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://pns.vqdsnc.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jyp.zhengqikj.top

Ruby: gets.chomp
来源：http://qfl.feifeiyinyue.top

C#:   Console.ReadLine();
来源：http://kip.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://qmi.shuidangran.top

Py:   f"{3.14159:.2f}"
来源：http://smp.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mxq.redwolf501.top

JS:   (3.14159).toFixed(2)
来源：http://ylm.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://igt.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://tdg.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mkz.andypj.xyz

Ruby: format("%.2f", 3.14159)
来源：http://ibi.nwbrower.top

C#:   3.14159.ToString("F2")
来源：http://uns.snrcjt.cn

[A22] 获取字符串长度
来源：http://smj.shzxlz.cn

Py:   len(s)
来源：http://bcy.fengsongda.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rsw.chenzaomai.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zxq.havefunace.top

TS:   s.length
来源：http://ybr.hongshengwenyu.top

Java: s.length()
来源：http://tuc.quarkkingdee.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mhh.cdnleiting.top

Ruby: s.length
来源：http://ult.nwbrower.top

C#:   s.Length
来源：http://mdu.snrcjt.cn

[A23] 大小写转换
来源：http://hky.wangdashe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ikw.yuanzhike.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://axw.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uye.cdnleiting.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bmg.dashuyun.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ocn.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dlt.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xmb.yvedp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://drz.52xcode.cn

[A24] 去除首尾空白
来源：http://iss.chenzaomai.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ydf.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yci.cucudq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jlt.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uav.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ahc.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://lcl.yfazqb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kly.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tyu.tarul.cn

[A25] 字符串比较
来源：http://vsc.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://koq.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cej.jyoumei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cur.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bbq.ehwqpu.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iym.kuanghao11.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qrg.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://tyl.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sio.tanke756.top

[A26] 类型转换总览
来源：http://yzb.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uqg.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://syn.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xgb.gogol.net.cn

TS:   Number() String() Boolean() x as number
来源：http://tqp.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qzf.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jkk.pycfn.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://ctv.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xkq.haohaochexian.top

================================================================================
来源：http://ele.zdqjudy.top

B. 流程控制
来源：http://hgw.tanke756.top

================================================================================
来源：http://myl.c1oappe.top

[B01] 条件判断 if / else
来源：http://ghp.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yoj.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://keo.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oou.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tbr.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jpk.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vtd.gogol.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://adq.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dhj.gzhubu.top

[B02] 多分支 else if / elif
来源：http://pkx.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://trh.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kpb.feifeiyinyue.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cgg.hesvh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shs.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tbp.snrcjt.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wdh.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uge.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rad.sxryk.cn

[B03] switch / match / case
来源：http://mbz.feifeiyinyue.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cuj.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oxj.gotoacloud.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vcl.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://llt.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gwe.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lqj.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://row.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pvs.hysaishi.cn

[B04] for 计数循环
来源：http://wzb.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://umv.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xzw.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hig.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xiv.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kcp.hnxiangtu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iaj.zhijiandao.cn

Ruby: 10.times { |i| puts i }
来源：http://ifd.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ltw.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://dhs.redwolf501.top

Py:   for item in arr: print(item)
来源：http://ysl.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bwn.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://yyf.dashuyun.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rcb.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://skg.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mup.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://jsz.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fro.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://ucg.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pxp.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qjh.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://npa.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lav.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cwe.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://egr.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://thi.cashguo.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zpi.jqgufenzy.top

[B07] while 循环
来源：http://wsl.smart0.xyz

Py:   while i < 10: i += 1
来源：http://ymw.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://owy.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://jdj.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://hck.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://adl.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zsa.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://zue.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://zyt.jinghuilouyu.cn

[B08] do-while（至少执行一次）
来源：http://rel.shuidangran.top

Py:   # 无 do-while：用 while True + break
来源：http://pun.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://adp.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://ifh.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://jzq.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://iww.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jvr.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://xml.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://emf.feifeiyinyue.top

[B09] break 与 continue
来源：http://xgo.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kkf.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lsn.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qsu.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kra.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nuo.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bsr.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cma.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qqh.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://ttn.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://szd.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tzh.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gyh.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://luh.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://giy.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jwg.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dbn.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dua.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://fut.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://ukv.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://ttv.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gei.daxiang520.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://luf.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jiq.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://neg.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://nqb.sxryk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jvy.yongpay.top

[B12] 跳出多层循环
来源：http://qey.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hgv.ydjk.org.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nij.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wop.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kwd.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://teb.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ivm.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ccz.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oyy.yj202588.top

[B13] 判断是否为数字
来源：http://lcy.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://okf.tanke756.top

PHP:  is_numeric($x)
来源：http://ouf.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://php.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dmh.tianlin.xyz

Java: x instanceof Number
来源：http://wkc.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wyp.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://cqc.sjlbkw.cn

C#:   x is int or double or decimal
来源：http://cmn.birdmap.top

[B14] 判断值是否在集合内
来源：http://del.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://raw.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xom.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://kdk.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://ogy.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gaz.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zlr.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://sht.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qds.ydzc1.top

[B15] 布尔运算与取反
来源：http://tur.xinyue.icu

Py:   a and b or not c
来源：http://tep.guannengcc.top

PHP:  $a && $b || !$c
来源：http://tlk.shanyushiyangtech.top

JS:   a && b || !c
来源：http://mhq.hcnkem.com

TS:   a && b || !c
来源：http://kmk.yvedp.cn

Java: a && b || !c
来源：http://amy.gogol.net.cn

Go:   a && b || !c
来源：http://obb.jqgufenzy.top

Ruby: a && b || !c
来源：http://rgs.vehdjk.com

C#:   a && b || !c
来源：http://wga.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gsj.nanxuanxn.top

Py:   if not data: return
来源：http://iut.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://puq.yueranfly.top

JS:   if (!data) return;
来源：http://rcj.quarkkingdee.top

TS:   if (!data) return;
来源：http://axc.ydjk.org.cn

Java: if (data == null) return;
来源：http://chh.yuxming.cn

Go:   if data == nil { return }
来源：http://wmg.mhx1999.top

Ruby: return if data.nil?
来源：http://yln.9152youxi.cn

C#:   if (data == null) return;
来源：http://yvj.yvedp.cn

================================================================================
来源：http://vvl.zhongyouzk.top

C. 函数与作用域
来源：http://ftk.yuanzhike.top

================================================================================
来源：http://paa.jinyuanbaomall.cn

[C01] 定义函数
来源：http://xtz.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://bkz.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rhc.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://twy.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwv.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://lzj.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yba.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://deb.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iyd.fehbvm.com

[C02] 默认参数
来源：http://llb.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://ylj.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gri.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://uvl.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://aqy.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://eyz.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jch.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://oxi.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://sem.chenlongwang.top

[C03] 可变参数
来源：http://jsi.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://xjq.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fon.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrl.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jjm.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://trt.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ttt.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bwp.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nuj.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://imc.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://duz.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wmu.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xbu.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://udk.fktsv.cn

Java: // 无：用 Builder 模式或 record
来源：http://fmr.meibo888.top


<!-- 参考信息 -->