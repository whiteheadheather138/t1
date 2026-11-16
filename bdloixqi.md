代发 wailian999

[A10] 生成随机数
来源：http://zji.zhongyouzk.top

Py:   import random; random.randint(1, 100)
来源：http://qpk.xylfe.cn

PHP:  random_int(1, 100);
来源：http://ega.yueranfly.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uuq.birdmap.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cqy.hnqzz.top

Java: new Random().nextInt(100) + 1
来源：http://vlo.hongshengwenyu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bno.ydzc1.top

Ruby: rand(1..100)
来源：http://ovz.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://yll.sufxvd.cn

[A11] 条件表达式（三元）
来源：http://fnu.zhixingplan.top

Py:   "yes" if x > 0 else "no"
来源：http://zqz.sweek.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://odo.ywan-chungtsiang.top

JS:   x > 0 ? "yes" : "no"
来源：http://ubg.hcnkem.com

TS:   x > 0 ? "yes" : "no"
来源：http://deg.birdmap.top

Java: x > 0 ? "yes" : "no"
来源：http://dcb.shzxlz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dqz.epnwcf.com

Ruby: x > 0 ? "yes" : "no"
来源：http://tha.nanxinkj.top

C#:   x > 0 ? "yes" : "no"
来源：http://bjg.xylfe.cn

[A12] 字符串插值 / 格式化
来源：http://lbc.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tmv.sufxvd.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hqr.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://pgv.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://nwj.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://jvr.aibaodan.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://emg.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://cbw.hnxiangtu.top

C#:   $"Hello, {name}!"
来源：http://ndc.shangyingyoupin.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qxt.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://cza.cdnleiting.top

PHP:  "第一行\n第二行"
来源：http://xau.uphjek.com

JS:   "第一行\n第二行"
来源：http://qrm.hfpthk.cn

TS:   "第一行\n第二行"
来源：http://krc.52xcode.cn

Java: "第一行\n第二行"
来源：http://pmf.andypj.xyz

Go:   "第一行\n第二行"
来源：http://qzl.meibo888.top

Ruby: "第一行\n第二行"
来源：http://mhr.xuetiantiany.cn

C#:   "第一行\n第二行"
来源：http://ifm.pengpengdd.cyou

[A14] 注释写法
来源：http://vcj.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://azz.gotoacloud.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mon.vehdjk.com

JS:   // 单行；/* 多行 */
来源：http://uku.chenjidiqi.icu

TS:   // 单行；/* 多行 */
来源：http://smo.9152youxi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://adk.ybcxt.top

Go:   // 单行；/* 多行 */
来源：http://zxj.yueranfly.top

Ruby: # 单行；=begin 多行 =end
来源：http://dhb.tianlin.xyz

C#:   // 单行；/* 多行 */
来源：http://qvq.uphjek.com

[A15] 空值判断与默认值
来源：http://obp.jinghuilouyu.cn

Py:   value = data or "默认值"
来源：http://tex.wangdashe.top

PHP:  $value = $data ?? "默认值";
来源：http://nay.epnwcf.com

JS:   const value = data ?? "默认值";
来源：http://lgu.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://ibu.hnxiangtu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://apu.xziqi.cn

Go:   if data == "" { data = "默认值" }
来源：http://sea.fengsongda.top

Ruby: value = data || "默认值"
来源：http://ola.birdmap.top

C#:   var value = data ?? "默认值";
来源：http://oxg.pengpengdd.cyou

[A16] 真假值判断规则
来源：http://ghz.hnxiangtu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ngx.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mmc.svipenyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tbi.yanxiufei.cn

TS:   if (!x) {}
来源：http://mng.fanxiaobao.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ibu.yonumen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ztv.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vjy.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://raq.pengpengdd.cyou

[A17] 位运算
来源：http://wvs.ywan-chungtsiang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://drt.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mzo.yvedp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pbg.yj20258888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://btj.jlsjyb.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfi.zhoulong.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rhl.jqgufenzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://udt.ywan-chungtsiang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mnx.ppjwa.cn

[A18] 字符与 ASCII 码互转
来源：http://ipq.ydjk.org.cn

Py:   ord("A"); chr(65)
来源：http://qkt.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://goe.zhiwuduotai.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kqo.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cpl.yanxiufei.cn

Java: (int) 'A'; (char) 65
来源：http://xub.yonumen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nlv.zhengqikj.top

Ruby: "A".ord; 65.chr
来源：http://tar.jinqigfzy.top

C#:   (int)'A'; (char)65
来源：http://uxt.jqgufenzy.top

[A19] 交换两个变量
来源：http://ovs.jiagoushi.top

Py:   a, b = b, a
来源：http://vmm.haohaochexian.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zxy.hysaishi.cn

JS:   [a, b] = [b, a];
来源：http://uti.xziqi.cn

TS:   [a, b] = [b, a];
来源：http://qgf.9152youxi.cn

Java: int t = a; a = b; b = t;
来源：http://evr.yj20258.top

Go:   a, b = b, a
来源：http://ery.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://stn.haohaochexian.top

C#:   (a, b) = (b, a);
来源：http://btm.yj202588.top

[A20] 读取标准输入
来源：http://fji.yj20258.top

Py:   name = input("请输入：")
来源：http://lly.svipenyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vra.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aas.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://mih.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://zwl.316326.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cvm.haohaochexian.top

Ruby: gets.chomp
来源：http://wwv.gogol.net.cn

C#:   Console.ReadLine();
来源：http://uwy.hnqzz.top

[A21] 保留指定小数位输出
来源：http://qqb.52xcode.cn

Py:   f"{3.14159:.2f}"
来源：http://rmf.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://chz.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://rxn.hammf.cn

TS:   (3.14159).toFixed(2)
来源：http://vqf.epnwcf.com

Java: String.format("%.2f", 3.14159)
来源：http://hrc.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pis.sxryk.cn

Ruby: format("%.2f", 3.14159)
来源：http://wej.shzxlz.cn

C#:   3.14159.ToString("F2")
来源：http://nzq.c1oappe.top

[A22] 获取字符串长度
来源：http://gtn.zdqjudy.top

Py:   len(s)
来源：http://mgq.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qfd.fehbvm.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lzc.aizwys.cn

TS:   s.length
来源：http://cdo.feifeiyinyue.top

Java: s.length()
来源：http://kaf.tanke756.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ceb.dianchejie.cn

Ruby: s.length
来源：http://vxb.gogol.net.cn

C#:   s.Length
来源：http://ere.sxryk.cn

[A23] 大小写转换
来源：http://nnl.fengsongda.top

Py:   s.upper(); s.lower(); s.title()
来源：http://usw.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fnw.jyoumei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rtc.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jon.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aty.zhiwuduotai.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vae.svipenyu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gde.gotoacloud.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kox.xziqi.cn

[A24] 去除首尾空白
来源：http://ctu.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eqr.hfpthk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xwi.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dwu.shanyushiyangtech.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vkz.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eeo.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://ein.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uwy.meibo888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tur.daxiang520.top

[A25] 字符串比较
来源：http://wde.cqqwz.cn

Py:   s1 == s2; s1 != s2
来源：http://nfp.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wsw.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xbk.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xxs.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cik.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mjc.zhixingplan.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mie.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jny.hnqzz.top

[A26] 类型转换总览
来源：http://jrm.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yjy.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nsn.tanke756.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tae.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://uzp.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xpe.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://phy.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dfq.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xpi.hfpthk.cn

================================================================================
来源：http://foq.yuanzhike.top

B. 流程控制
来源：http://qtv.andypj.xyz

================================================================================
来源：http://vpo.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://wue.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nsx.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ykb.iojbl.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lsb.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ldc.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xty.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://agy.hywenlv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ghx.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hfv.smart0.xyz

[B02] 多分支 else if / elif
来源：http://des.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zth.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cpi.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://psf.zhiwuduotai.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ywh.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdd.chenlongwang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uzb.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://adb.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://erc.svipenyu.cn

[B03] switch / match / case
来源：http://jqf.jinqigufen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kww.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vcz.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://txm.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://twq.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tyb.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bth.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://elt.yangfankeji.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jsx.havefunace.top

[B04] for 计数循环
来源：http://kif.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://wad.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ytb.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ubu.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://onk.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cgh.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lfd.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://pjm.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ift.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://eqc.tian-w.cn

Py:   for item in arr: print(item)
来源：http://exc.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bsm.nanxuanxn.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mcf.yvedp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hyi.dashuyun.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vku.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yxn.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://kse.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lcg.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://klb.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iqw.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nkp.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gug.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hdv.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lse.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sph.yj20258888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xxn.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://slc.guowangkeji.top

[B07] while 循环
来源：http://xui.fktsv.cn

Py:   while i < 10: i += 1
来源：http://fhv.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://htm.hnxiangtu.top

JS:   while (i < 10) { i++; }
来源：http://vmu.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://tos.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://gzh.zhengqikj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lkw.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://fzo.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://zat.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://bii.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://cdt.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cdv.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://eoo.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://wny.yonumen.top

Java: do { i++; } while (i < 10);
来源：http://smi.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ngk.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://veo.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://rqm.yfazqb.com

[B09] break 与 continue
来源：http://erp.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dyd.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yma.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydu.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzu.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksn.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ajk.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dbc.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pke.redwolf501.top

[B10] 遍历同时拿索引
来源：http://yxe.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nrw.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vbz.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qzq.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cgx.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ssb.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gxy.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nab.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lcc.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://bvy.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://kyu.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://pkp.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://edx.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ufz.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rzs.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kvj.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://prq.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ybd.svipenyu.cn

[B12] 跳出多层循环
来源：http://dqp.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bxj.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zjx.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hcg.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qac.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xzh.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pfb.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://axm.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://drn.bbcook.cn

[B13] 判断是否为数字
来源：http://aze.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://npf.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://blt.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://svx.smart0.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jqg.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://els.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uxk.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://oxw.fktsv.cn

C#:   x is int or double or decimal
来源：http://rwq.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://bdx.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bpq.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zll.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://edg.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://khn.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ddo.hnxiangtu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vhg.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bzp.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ydr.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://scq.sxryk.cn

Py:   a and b or not c
来源：http://sgm.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://pww.xziqi.cn

JS:   a && b || !c
来源：http://wra.smart0.xyz

TS:   a && b || !c
来源：http://fye.daria6918.cn

Java: a && b || !c
来源：http://ani.tarul.cn

Go:   a && b || !c
来源：http://fqj.jianghu66.top

Ruby: a && b || !c
来源：http://mlq.jinqigufen.top

C#:   a && b || !c
来源：http://cxc.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ylh.zhiwuduotai.top

Py:   if not data: return
来源：http://lju.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://nnf.tarul.cn

JS:   if (!data) return;
来源：http://yqs.cheryme.top

TS:   if (!data) return;
来源：http://ghq.shanyushiyangtech.top

Java: if (data == null) return;
来源：http://agk.ivvv.top

Go:   if data == nil { return }
来源：http://afc.jinqigfzy.top

Ruby: return if data.nil?
来源：http://msy.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://ece.jlsjyb.cn


<!-- 参考信息 -->