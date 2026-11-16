代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://dqu.hnxiangtu.top

C#:   x > 0 ? "yes" : "no"
来源：http://ygq.yuanzhike.top

[A12] 字符串插值 / 格式化
来源：http://rdi.ywan-chungtsiang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xmg.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zsv.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://hjf.dashuyun.cn

TS:   `Hello, ${name}!`
来源：http://qze.hywenlv.cn

Java: "Hello, %s!".formatted(name)
来源：http://zig.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cmg.sxryk.cn

Ruby: "Hello, #{name}!"
来源：http://axg.bbcook.cn

C#:   $"Hello, {name}!"
来源：http://rws.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cpg.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://zun.guowangkeji.top

PHP:  "第一行\n第二行"
来源：http://epl.bjfxy.top

JS:   "第一行\n第二行"
来源：http://etb.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://ntk.sysykeji.top

Java: "第一行\n第二行"
来源：http://grf.jqgfzy.top

Go:   "第一行\n第二行"
来源：http://beg.jinghuilouyu.cn

Ruby: "第一行\n第二行"
来源：http://nkb.vehdjk.com

C#:   "第一行\n第二行"
来源：http://vgt.zhixingplan.top

[A14] 注释写法
来源：http://qmr.yongpay.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fwp.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hqe.zhaomingkeji.xyz

JS:   // 单行；/* 多行 */
来源：http://zjg.jiagoushi.top

TS:   // 单行；/* 多行 */
来源：http://yth.xziqi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nlw.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://ags.xylfe.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zdh.shanyushiyangtech.top

C#:   // 单行；/* 多行 */
来源：http://dwf.jyoumei.cn

[A15] 空值判断与默认值
来源：http://sft.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://qcg.nanxinkj.top

PHP:  $value = $data ?? "默认值";
来源：http://jsc.jinghuilouyu.cn

JS:   const value = data ?? "默认值";
来源：http://oyz.hysaishi.cn

TS:   const value = data ?? "默认值";
来源：http://dlc.andypj.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dkt.meibo888.top

Go:   if data == "" { data = "默认值" }
来源：http://pvi.zhijiandao.cn

Ruby: value = data || "默认值"
来源：http://hvp.kuanghao11.cn

C#:   var value = data ?? "默认值";
来源：http://eec.yangfankeji.com

[A16] 真假值判断规则
来源：http://hhj.fengsongda.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hdb.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mus.shzxlz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jms.feifeiyinyue.top

TS:   if (!x) {}
来源：http://tdn.hnxiangtu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fjv.gogol.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cwr.nanxuanxn.top

Ruby: unless x            # nil 与 false 为假
来源：http://gkd.sufxvd.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oao.iojbl.cn

[A17] 位运算
来源：http://ipr.hnqzz.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vjq.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ior.daxiang520.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://adc.shanyushiyangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jaf.tarul.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vsc.yj202588.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zaj.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzp.ehwqpu.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wuj.xuetiantiany.cn

[A18] 字符与 ASCII 码互转
来源：http://ifd.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://cgv.aibaodan.cn

PHP:  ord("A"); chr(65)
来源：http://ibs.chenjidiqi.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gkd.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://znk.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://kzt.xuetiantiany.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hbq.yuanzhike.top

Ruby: "A".ord; 65.chr
来源：http://hur.vehdjk.com

C#:   (int)'A'; (char)65
来源：http://biz.nanxuanxn.top

[A19] 交换两个变量
来源：http://ras.shanyushiyangtech.top

Py:   a, b = b, a
来源：http://xjb.yongpay.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mdm.fzhhl.top

JS:   [a, b] = [b, a];
来源：http://ebn.sweek.top

TS:   [a, b] = [b, a];
来源：http://ekd.shuidangran.top

Java: int t = a; a = b; b = t;
来源：http://dys.zhongyouzk.top

Go:   a, b = b, a
来源：http://bzf.gotoacloud.top

Ruby: a, b = b, a
来源：http://biy.hesvh.cn

C#:   (a, b) = (b, a);
来源：http://gfr.yj202588.top

[A20] 读取标准输入
来源：http://nhz.jiagoushi.top

Py:   name = input("请输入：")
来源：http://ngu.svipenyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kti.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cua.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://goi.zdqjudy.top

Java: new Scanner(System.in).nextLine()
来源：http://bif.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vdb.pycfn.com

Ruby: gets.chomp
来源：http://pfn.hesvh.cn

C#:   Console.ReadLine();
来源：http://kfe.xinyue.icu

[A21] 保留指定小数位输出
来源：http://ist.birdmap.top

Py:   f"{3.14159:.2f}"
来源：http://eyl.zdqjudy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nks.sjlbkw.cn

JS:   (3.14159).toFixed(2)
来源：http://itz.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://xfi.jqgfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://osf.sweek.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qjg.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://amo.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://snx.zycfv.cn

[A22] 获取字符串长度
来源：http://yqs.yongpay.top

Py:   len(s)
来源：http://ajj.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pav.zhijiandao.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jsv.52xcode.cn

TS:   s.length
来源：http://erh.hcnkem.com

Java: s.length()
来源：http://mhv.zdqjudy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://elb.guannengcc.top

Ruby: s.length
来源：http://bws.hysaishi.cn

C#:   s.Length
来源：http://aeo.jyoumei.cn

[A23] 大小写转换
来源：http://awr.tianlin.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://ggt.kuanghao11.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://srf.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dip.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vxx.xziqi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vtf.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vxf.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vow.9152youxi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eit.iojbl.cn

[A24] 去除首尾空白
来源：http://yeb.nanxuanxn.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bwx.xuanzx.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uyi.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://imn.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zfg.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uyn.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://tyi.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uqz.0kj1m.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ber.nanxuanxn.top

[A25] 字符串比较
来源：http://vel.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://gvw.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rog.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sdm.0kj1m.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qua.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pkv.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tci.ybcxt.top

Ruby: s1 == s2; s1 <=> s2
来源：http://snn.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oid.zhongyouzk.top

[A26] 类型转换总览
来源：http://mzd.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xuv.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ock.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ddy.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://jds.hnxiangtu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lpp.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xfs.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://oeu.316326.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ucy.tanke756.top

================================================================================
来源：http://vxx.vqdsnc.cn

B. 流程控制
来源：http://pgw.fengsongda.top

================================================================================
来源：http://vyw.wangdashe.top

[B01] 条件判断 if / else
来源：http://vih.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jno.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dag.chenlongwang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://utl.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wpw.meibo888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nck.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fao.jinyuanbaomall.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qlr.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nlx.ivvv.top

[B02] 多分支 else if / elif
来源：http://cin.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oea.tianlin.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tjb.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yqy.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ouy.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dje.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dnt.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zwi.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdk.jqgufenzy.top

[B03] switch / match / case
来源：http://vsp.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nqf.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://swb.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cqa.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://adr.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lai.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dyt.xuetiantiany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jod.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fus.yfazqb.com

[B04] for 计数循环
来源：http://swa.sweek.top

Py:   for i in range(10): print(i)
来源：http://dbc.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zqn.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bsv.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://odi.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nfr.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sio.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://zvf.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tyz.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://zdn.shuidangran.top

Py:   for item in arr: print(item)
来源：http://vki.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vwf.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://zei.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hxg.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://whv.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nld.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://dwh.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ald.yonumen.top

[B06] 遍历字典 / 对象
来源：http://khe.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://odq.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bew.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wca.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vgr.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qxy.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vmn.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ywf.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jrb.chenzaomai.com

[B07] while 循环
来源：http://dnt.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://uce.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jvt.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://kbv.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://jnb.cashguo.top

Java: while (i < 10) { i++; }
来源：http://cpe.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pfc.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://gtu.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://yrm.dashuyun.cn

[B08] do-while（至少执行一次）
来源：http://rss.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://bhd.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://edi.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://lli.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://lpr.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://vod.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://kxv.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://cpv.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://hag.uphjek.com

[B09] break 与 continue
来源：http://oju.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vlh.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pnb.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sgl.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzf.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rgm.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eeq.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://shj.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqe.andypj.xyz

[B10] 遍历同时拿索引
来源：http://onf.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jpa.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gvi.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mfj.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fqj.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gre.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mzr.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vto.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ron.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://ewm.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://mfi.vehdjk.com

PHP:  range(0, 10, 2);
来源：http://gbe.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vey.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nan.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ybn.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ppw.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://dmm.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ycw.yfazqb.com

[B12] 跳出多层循环
来源：http://uzg.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ikn.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ndz.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zxn.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oyj.pycfn.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qyd.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ofj.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gev.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vvc.ydjk.org.cn

[B13] 判断是否为数字
来源：http://orc.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://jzt.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://aee.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kew.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://olu.yvedp.cn

Java: x instanceof Number
来源：http://vvr.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cnw.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://djv.yueranfly.top

C#:   x is int or double or decimal
来源：http://gik.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://wbl.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yva.jiagoushi.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qxq.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://xlv.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://uom.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://drg.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://omu.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://ksg.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://btv.hesvh.cn

[B15] 布尔运算与取反
来源：http://njr.yangfankeji.com

Py:   a and b or not c
来源：http://vuz.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://ncr.aizwys.cn

JS:   a && b || !c
来源：http://jqz.sweek.top

TS:   a && b || !c
来源：http://aze.ehwqpu.com

Java: a && b || !c
来源：http://mdv.birdmap.top

Go:   a && b || !c
来源：http://ykf.shangyingyoupin.top

Ruby: a && b || !c
来源：http://gtp.yueranfly.top

C#:   a && b || !c
来源：http://rqd.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://sjz.shzxlz.cn

Py:   if not data: return
来源：http://uez.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://qdv.wangshuangyany.cn

JS:   if (!data) return;
来源：http://oep.gogol.net.cn

TS:   if (!data) return;
来源：http://vqm.vehdjk.com

Java: if (data == null) return;
来源：http://fkw.cheryme.top

Go:   if data == nil { return }
来源：http://keo.nwbrower.top

Ruby: return if data.nil?
来源：http://tob.jinqigufen.top

C#:   if (data == null) return;
来源：http://tuo.ivvv.top

================================================================================
来源：http://tfb.ywan-chungtsiang.top

C. 函数与作用域
来源：http://lcr.svipenyu.cn

================================================================================
来源：http://icl.jinqigfzy.top

[C01] 定义函数
来源：http://xhv.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://pff.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wzl.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://quq.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pzj.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://cui.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://prs.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://hse.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nrm.fanxiaobao.xyz

[C02] 默认参数
来源：http://tyj.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://uso.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ral.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://bxa.jqgfzy.top


<!-- 参考信息 -->