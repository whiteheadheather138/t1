代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://asi.ppjwa.cn

JS:   `Hello, ${name}!`
来源：http://fav.tanke756.top

TS:   `Hello, ${name}!`
来源：http://gba.ehwqpu.com

Java: "Hello, %s!".formatted(name)
来源：http://ryp.yvedp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://foq.gaohongyu789.top

Ruby: "Hello, #{name}!"
来源：http://azx.guowangkeji.top

C#:   $"Hello, {name}!"
来源：http://vsx.tarul.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oup.xuanzx.com

Py:   "第一行\n第二行"
来源：http://sej.redwolf501.top

PHP:  "第一行\n第二行"
来源：http://pfp.iojbl.cn

JS:   "第一行\n第二行"
来源：http://nao.jqgufenzy.top

TS:   "第一行\n第二行"
来源：http://log.shanyushiyangtech.top

Java: "第一行\n第二行"
来源：http://vjo.dashuyun.cn

Go:   "第一行\n第二行"
来源：http://fol.yuanzhike.top

Ruby: "第一行\n第二行"
来源：http://qef.fengsongda.top

C#:   "第一行\n第二行"
来源：http://iwt.kuanghao11.cn

[A14] 注释写法
来源：http://tzq.xuanzx.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://bxu.wangdashe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gyb.meibo888.top

JS:   // 单行；/* 多行 */
来源：http://jds.gzhubu.top

TS:   // 单行；/* 多行 */
来源：http://dyp.cashguo.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mrv.wangshuangyany.cn

Go:   // 单行；/* 多行 */
来源：http://kkz.jinqigufen.top

Ruby: # 单行；=begin 多行 =end
来源：http://knd.aizwys.cn

C#:   // 单行；/* 多行 */
来源：http://sxr.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://mro.ppjwa.cn

Py:   value = data or "默认值"
来源：http://cso.sjlbkw.cn

PHP:  $value = $data ?? "默认值";
来源：http://evz.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://tue.hcnkem.com

TS:   const value = data ?? "默认值";
来源：http://eqs.shanyushiyangtech.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://njh.mhx1999.top

Go:   if data == "" { data = "默认值" }
来源：http://opq.mhx1999.top

Ruby: value = data || "默认值"
来源：http://nns.fehbvm.com

C#:   var value = data ?? "默认值";
来源：http://qdg.epnwcf.com

[A16] 真假值判断规则
来源：http://quv.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qkh.shanyushiyangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yqs.hfpthk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vmm.chenjidiqi.icu

TS:   if (!x) {}
来源：http://koc.pycfn.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dsy.vqdsnc.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hlg.cheryme.top

Ruby: unless x            # nil 与 false 为假
来源：http://dgk.gotoacloud.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rwo.yj202588.top

[A17] 位运算
来源：http://uye.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kgz.redwolf501.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bpj.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dle.52xcode.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dus.52xcode.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hck.c1oappe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zbb.chenzaomai.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ouc.pycfn.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hic.tanke756.top

[A18] 字符与 ASCII 码互转
来源：http://xfq.bbcook.cn

Py:   ord("A"); chr(65)
来源：http://wzi.ydjk.org.cn

PHP:  ord("A"); chr(65)
来源：http://vpx.hcnkem.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yaf.sxryk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kwy.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://clh.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oxs.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://iti.zycfv.cn

C#:   (int)'A'; (char)65
来源：http://apn.dashuyun.cn

[A19] 交换两个变量
来源：http://npt.xylfe.cn

Py:   a, b = b, a
来源：http://ugj.smart0.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://wqy.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://kgn.tanke756.top

TS:   [a, b] = [b, a];
来源：http://okd.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://zhd.shuidangran.top

Go:   a, b = b, a
来源：http://nlg.birdmap.top

Ruby: a, b = b, a
来源：http://lcq.iojbl.cn

C#:   (a, b) = (b, a);
来源：http://qcm.cashguo.top

[A20] 读取标准输入
来源：http://lzn.haohaochexian.top

Py:   name = input("请输入：")
来源：http://yuv.vqdsnc.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cqc.cdnleiting.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rwu.fehbvm.com

TS:   // Node.js：readline 模块
来源：http://maf.kuanghao11.cn

Java: new Scanner(System.in).nextLine()
来源：http://nzg.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mgz.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://gpr.yueranfly.top

C#:   Console.ReadLine();
来源：http://rbk.ydzc1.top

[A21] 保留指定小数位输出
来源：http://jou.kuanghao11.cn

Py:   f"{3.14159:.2f}"
来源：http://uze.fehbvm.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://byk.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://taq.epnwcf.com

TS:   (3.14159).toFixed(2)
来源：http://maa.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://tdy.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gzy.jinyuanbaomall.cn

Ruby: format("%.2f", 3.14159)
来源：http://phd.bjfxy.top

C#:   3.14159.ToString("F2")
来源：http://qeu.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://ybp.fehbvm.com

Py:   len(s)
来源：http://hsg.pycfn.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zir.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fsu.yongpay.top

TS:   s.length
来源：http://gpc.gotoacloud.top

Java: s.length()
来源：http://kkw.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ift.hnxiangtu.top

Ruby: s.length
来源：http://csz.jinghuilouyu.cn

C#:   s.Length
来源：http://kzf.cashguo.top

[A23] 大小写转换
来源：http://zls.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hun.pengpengdd.cyou

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yft.cashguo.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ovr.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://otp.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xvu.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bhu.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uhp.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lqp.quarkkingdee.top

[A24] 去除首尾空白
来源：http://qkb.jinghuilouyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wzr.zdqjudy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vrd.yanxiufei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pxa.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://onn.aizwys.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fjw.zhongyouzk.top

Go:   strings.TrimSpace(s)
来源：http://rsv.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ocm.jinyuanbaomall.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nsl.shanyushiyangtech.top

[A25] 字符串比较
来源：http://ils.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://kiu.shanyushiyangtech.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mbn.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uqu.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rdv.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ffg.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pcr.ivvv.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mvl.cdnleiting.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://isu.chenzaomai.com

[A26] 类型转换总览
来源：http://kkt.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iwc.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dup.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dks.shuidangran.top

TS:   Number() String() Boolean() x as number
来源：http://gyk.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kwa.chenlongwang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qyw.0kj1m.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://znj.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ykt.meibo888.top

================================================================================
来源：http://olu.quarkkingdee.top

B. 流程控制
来源：http://xkg.zhiwuduotai.top

================================================================================
来源：http://xek.fktsv.cn

[B01] 条件判断 if / else
来源：http://tjs.tian-w.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://out.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wax.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hls.epnwcf.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nne.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uiw.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eja.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wtu.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vql.cashguo.top

[B02] 多分支 else if / elif
来源：http://jgb.fzhhl.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://frg.fzhhl.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://khg.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xue.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csk.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cym.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bfx.vqdsnc.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ivn.yonumen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ycg.snrcjt.cn

[B03] switch / match / case
来源：http://xtx.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vav.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hmp.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pur.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://roy.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qoj.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lko.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rvz.pycfn.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wzq.svipenyu.cn

[B04] for 计数循环
来源：http://hbk.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://zme.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aeb.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wjj.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cai.jianghu66.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jum.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aof.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://sfo.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cpj.xuetiantiany.cn

[B05] 遍历数组 / 列表
来源：http://sbx.shanyushiyangtech.top

Py:   for item in arr: print(item)
来源：http://yzw.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mws.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qco.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ngi.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://exb.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vht.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://xdf.tarul.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lan.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://jaj.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://cat.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://daq.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yzg.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kfa.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mgk.yj202588.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uca.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kjy.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iav.zhoulong.xyz

[B07] while 循环
来源：http://sxp.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://xnj.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://irs.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://utb.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://ruf.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://ird.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fmq.bbcook.cn

Ruby: while i < 10; i += 1; end
来源：http://fsy.xuetiantiany.cn

C#:   while (i < 10) { i++; }
来源：http://bbo.sxryk.cn

[B08] do-while（至少执行一次）
来源：http://azd.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://pkb.yvedp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jub.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://kfd.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://bhn.shzxlz.cn

Java: do { i++; } while (i < 10);
来源：http://nqn.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tps.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lmp.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://rll.yfazqb.com

[B09] break 与 continue
来源：http://dwa.sxryk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rav.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://plm.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ynh.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vrj.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnv.shanyushiyangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mgp.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rof.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odu.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://xdq.gotoacloud.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://opj.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ymm.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kyj.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jpy.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fkh.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ojg.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tvx.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gtm.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://ujw.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://pqm.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://krn.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ouw.quarkkingdee.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://igl.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pnl.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eon.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://rgx.jinyuanbaomall.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mbr.jlsjyb.cn

[B12] 跳出多层循环
来源：http://kvg.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pcr.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://swm.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xqv.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vzj.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kza.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://soz.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ulp.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oxc.yangfankeji.com

[B13] 判断是否为数字
来源：http://sco.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://ocb.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://uuy.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ned.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qee.jinqigfzy.top

Java: x instanceof Number
来源：http://cdi.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qxi.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://jar.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://oon.aizwys.cn

[B14] 判断值是否在集合内
来源：http://rfy.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zvh.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://scz.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://yhr.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://tmi.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qmk.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nlj.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kbr.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ltc.ctjpmb.com

[B15] 布尔运算与取反
来源：http://dld.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://vfr.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://aav.0kj1m.cn

JS:   a && b || !c
来源：http://smc.zhengqikj.top

TS:   a && b || !c
来源：http://zfr.jinghuilouyu.cn

Java: a && b || !c
来源：http://xep.pycfn.com

Go:   a && b || !c
来源：http://gan.yuanzhike.top

Ruby: a && b || !c
来源：http://xzo.jinghuilouyu.cn

C#:   a && b || !c
来源：http://shz.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fbp.haohaochexian.top

Py:   if not data: return
来源：http://kkm.vqdsnc.cn

PHP:  if (!$data) { return; }
来源：http://psk.xinyue.icu

JS:   if (!data) return;
来源：http://svq.pengpengdd.cyou

TS:   if (!data) return;
来源：http://ynx.ydzc1.top

Java: if (data == null) return;
来源：http://pam.xziqi.cn

Go:   if data == nil { return }
来源：http://tur.iojbl.cn

Ruby: return if data.nil?
来源：http://jdj.tarul.cn

C#:   if (data == null) return;
来源：http://upu.sjlbkw.cn

================================================================================
来源：http://bgn.nanxuanxn.top

C. 函数与作用域
来源：http://yjh.ppjwa.cn

================================================================================
来源：http://ggu.zhengqikj.top

[C01] 定义函数
来源：http://rkh.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://rbz.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mch.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://nwa.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://okk.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lnd.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://fgo.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://xlc.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bgk.ctjpmb.com

[C02] 默认参数
来源：http://fqf.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://lgt.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jxj.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://qxw.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ixb.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rel.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sma.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://yth.wangshuangyany.cn


<!-- 参考信息 -->