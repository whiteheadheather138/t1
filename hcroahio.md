代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://cao.epnwcf.com

TS:   x > 0 ? "yes" : "no"
来源：http://hef.daxiang520.top

Java: x > 0 ? "yes" : "no"
来源：http://odh.andypj.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://lli.aibaodan.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bxn.yongpay.top

C#:   x > 0 ? "yes" : "no"
来源：http://bpy.shzxlz.cn

[A12] 字符串插值 / 格式化
来源：http://zsd.hywenlv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nsz.wangdashe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pci.jqgufenzy.top

JS:   `Hello, ${name}!`
来源：http://bkk.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://ils.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://msj.tarul.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xto.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://cbb.ehwqpu.com

C#:   $"Hello, {name}!"
来源：http://xkr.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://rqg.fktsv.cn

Py:   "第一行\n第二行"
来源：http://isy.hnxiangtu.top

PHP:  "第一行\n第二行"
来源：http://bgm.havefunace.top

JS:   "第一行\n第二行"
来源：http://ytr.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://gyi.aibaodan.cn

Java: "第一行\n第二行"
来源：http://ksu.jinqigufen.top

Go:   "第一行\n第二行"
来源：http://xav.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://qnv.daxiang520.top

C#:   "第一行\n第二行"
来源：http://jmg.316326.xyz

[A14] 注释写法
来源：http://cod.wangdashe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://frz.cucudq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://azd.snrcjt.cn

JS:   // 单行；/* 多行 */
来源：http://rqp.jyoumei.cn

TS:   // 单行；/* 多行 */
来源：http://ydv.9152youxi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kav.vqdsnc.cn

Go:   // 单行；/* 多行 */
来源：http://ngk.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hbf.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://zac.yanxiufei.cn

[A15] 空值判断与默认值
来源：http://ien.52xcode.cn

Py:   value = data or "默认值"
来源：http://gyf.yfazqb.com

PHP:  $value = $data ?? "默认值";
来源：http://aly.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://hwk.aizwys.cn

TS:   const value = data ?? "默认值";
来源：http://tlq.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ilj.hnxiangtu.top

Go:   if data == "" { data = "默认值" }
来源：http://ecm.ywan-chungtsiang.top

Ruby: value = data || "默认值"
来源：http://zxu.zhongyouzk.top

C#:   var value = data ?? "默认值";
来源：http://ykq.guowangkeji.top

[A16] 真假值判断规则
来源：http://btt.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://irk.ctjpmb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bij.yj202588.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nmm.sufxvd.cn

TS:   if (!x) {}
来源：http://lxk.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jgd.wangshuangyany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qrv.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://abh.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cwp.sjlbkw.cn

[A17] 位运算
来源：http://uag.sufxvd.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nvl.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eda.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lil.iojbl.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pwr.chenlongwang.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bpl.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ntt.ydjk.org.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mff.guowangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://epi.jqgfzy.top

[A18] 字符与 ASCII 码互转
来源：http://xms.52xcode.cn

Py:   ord("A"); chr(65)
来源：http://dut.tarul.cn

PHP:  ord("A"); chr(65)
来源：http://bbh.bjfxy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nqp.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dff.zhiwuduotai.top

Java: (int) 'A'; (char) 65
来源：http://nhl.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ynr.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://lrq.52xcode.cn

C#:   (int)'A'; (char)65
来源：http://bfs.snrcjt.cn

[A19] 交换两个变量
来源：http://hwv.kuanghao11.cn

Py:   a, b = b, a
来源：http://waz.yj20258.top

PHP:  [$a, $b] = [$b, $a];
来源：http://guj.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://fvd.wangdashe.top

TS:   [a, b] = [b, a];
来源：http://gzv.ydzc1.top

Java: int t = a; a = b; b = t;
来源：http://jda.yfazqb.com

Go:   a, b = b, a
来源：http://lwi.shzxlz.cn

Ruby: a, b = b, a
来源：http://ukp.aizwys.cn

C#:   (a, b) = (b, a);
来源：http://xke.yonumen.top

[A20] 读取标准输入
来源：http://pvv.jinqigfzy.top

Py:   name = input("请输入：")
来源：http://emq.zdqjudy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://euj.tanke756.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jcl.9152youxi.cn

TS:   // Node.js：readline 模块
来源：http://lmf.shzxlz.cn

Java: new Scanner(System.in).nextLine()
来源：http://jys.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pdl.fktsv.cn

Ruby: gets.chomp
来源：http://raj.jiagoushi.top

C#:   Console.ReadLine();
来源：http://zos.jinqigufen.top

[A21] 保留指定小数位输出
来源：http://phv.dashuyun.cn

Py:   f"{3.14159:.2f}"
来源：http://xjp.sweek.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lvi.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://zkj.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://pgb.gaohongyu789.top

Java: String.format("%.2f", 3.14159)
来源：http://cux.tian-w.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ktn.xylfe.cn

Ruby: format("%.2f", 3.14159)
来源：http://zri.cucudq.cn

C#:   3.14159.ToString("F2")
来源：http://jgs.tian-w.cn

[A22] 获取字符串长度
来源：http://hjk.fzhhl.top

Py:   len(s)
来源：http://kan.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yvm.cashguo.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hfa.tianlin.xyz

TS:   s.length
来源：http://jmx.jlsjyb.cn

Java: s.length()
来源：http://yzc.shangyingyoupin.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oid.shanyushiyangtech.top

Ruby: s.length
来源：http://gok.yuanzhike.top

C#:   s.Length
来源：http://pkk.hywenlv.cn

[A23] 大小写转换
来源：http://zxh.hfpthk.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zwy.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xep.dashuyun.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://efz.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bbs.jinqigufen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hlq.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cqu.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zys.chenjidiqi.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://jfp.cdnleiting.top

[A24] 去除首尾空白
来源：http://kct.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ans.xziqi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rrf.daria6918.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://trl.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tto.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kyt.sxryk.cn

Go:   strings.TrimSpace(s)
来源：http://bbd.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aqj.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pvo.shangyingyoupin.top

[A25] 字符串比较
来源：http://hws.sysykeji.top

Py:   s1 == s2; s1 != s2
来源：http://zps.mhx1999.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iks.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hbk.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hhy.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vqz.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eiu.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dbd.yonumen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xkm.52xcode.cn

[A26] 类型转换总览
来源：http://lzw.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eoz.yuanzhike.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jgd.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ybi.uphjek.com

TS:   Number() String() Boolean() x as number
来源：http://gnc.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ith.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lrn.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xza.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xnp.haohaochexian.top

================================================================================
来源：http://qzv.gotoacloud.top

B. 流程控制
来源：http://ntz.yj20258888.top

================================================================================
来源：http://igt.chenlongwang.top

[B01] 条件判断 if / else
来源：http://yxw.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ebu.gaohongyu789.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://utv.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kux.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sak.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://ayl.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://arx.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zka.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sqm.nwbrower.top

[B02] 多分支 else if / elif
来源：http://res.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://voo.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nur.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kxc.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mez.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqg.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cgq.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nou.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://akl.yangfankeji.com

[B03] switch / match / case
来源：http://hea.jinyuanbaomall.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qna.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iys.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pmh.316326.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qdf.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://drh.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bzd.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bxu.jinqigufen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vps.zhijiandao.cn

[B04] for 计数循环
来源：http://tmg.yongpay.top

Py:   for i in range(10): print(i)
来源：http://fbu.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cfp.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pna.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://byj.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tay.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zrt.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://kiw.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wej.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://kdr.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://fme.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vys.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://vgt.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mdc.dianchejie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cli.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hnu.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://oox.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vfg.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://xaq.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cwe.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dpz.sjlbkw.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vdt.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jdh.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pgz.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mpt.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ruu.wangdashe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vle.shzxlz.cn

[B07] while 循环
来源：http://qqx.yongpay.top

Py:   while i < 10: i += 1
来源：http://zaj.jinghuilouyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qnp.jqgufenzy.top

JS:   while (i < 10) { i++; }
来源：http://vuy.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://cej.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://dtj.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dta.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://gfs.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://fbz.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://eud.zhijiandao.cn

Py:   # 无 do-while：用 while True + break
来源：http://quu.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dys.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://xcb.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://ffn.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://jgb.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://eyp.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cxl.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://cdh.jiagoushi.top

[B09] break 与 continue
来源：http://ebb.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fqw.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nqu.shanyushiyangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzw.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://phm.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ead.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ubw.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ctk.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkv.iojbl.cn

[B10] 遍历同时拿索引
来源：http://usm.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cno.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nik.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fmb.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tpk.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pmi.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nck.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vjy.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mrq.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://oyd.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://xhk.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://yhd.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ndk.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wtk.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tbf.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aez.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://kxc.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ywb.yj202588.top

[B12] 跳出多层循环
来源：http://wcu.pycfn.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://evi.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ivo.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aod.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cvz.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mwv.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pyf.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xcv.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eks.52xcode.cn

[B13] 判断是否为数字
来源：http://rhg.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://bmf.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://pvi.dashuyun.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xza.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dsc.yongpay.top

Java: x instanceof Number
来源：http://gwp.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://olt.hnqzz.top

Ruby: x.is_a?(Numeric)
来源：http://kfn.pycfn.com

C#:   x is int or double or decimal
来源：http://xap.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://qei.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xof.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oky.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://dgq.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://qnr.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kic.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ctk.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uuz.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ati.cucudq.cn

[B15] 布尔运算与取反
来源：http://lon.jinqigfzy.top

Py:   a and b or not c
来源：http://iru.cucudq.cn

PHP:  $a && $b || !$c
来源：http://dxr.tarul.cn

JS:   a && b || !c
来源：http://ork.guannengcc.top

TS:   a && b || !c
来源：http://pnl.xuanzx.com

Java: a && b || !c
来源：http://pgc.fengsongda.top

Go:   a && b || !c
来源：http://llz.svipenyu.cn

Ruby: a && b || !c
来源：http://dok.mhx1999.top

C#:   a && b || !c
来源：http://nbe.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ioe.fengsongda.top

Py:   if not data: return
来源：http://ofj.yj20258.top

PHP:  if (!$data) { return; }
来源：http://gyo.sysykeji.top

JS:   if (!data) return;
来源：http://bxb.tian-w.cn

TS:   if (!data) return;
来源：http://mot.quarkkingdee.top

Java: if (data == null) return;
来源：http://mtx.meibo888.top

Go:   if data == nil { return }
来源：http://ehx.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://uck.jqgufenzy.top

C#:   if (data == null) return;
来源：http://qve.316326.xyz

================================================================================
来源：http://vql.shangyingyoupin.top

C. 函数与作用域
来源：http://onu.jinghuilouyu.cn

================================================================================
来源：http://gyg.jinyuanbaomall.cn

[C01] 定义函数
来源：http://xwj.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://tjq.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qtx.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://exn.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mky.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eqz.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rsa.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://knb.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vtk.andypj.xyz


<!-- 参考信息 -->