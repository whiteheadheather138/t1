代发 wailian999

[A10] 生成随机数
来源：http://psg.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://ibw.andypj.xyz

PHP:  random_int(1, 100);
来源：http://mzo.fzhhl.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oei.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ywe.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://hld.fengsongda.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://slz.chenjidiqi.icu

Ruby: rand(1..100)
来源：http://nql.fktsv.cn

C#:   new Random().Next(1, 101)
来源：http://ogz.sysykeji.top

[A11] 条件表达式（三元）
来源：http://yys.hfpthk.cn

Py:   "yes" if x > 0 else "no"
来源：http://dcl.cucudq.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zic.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://lvn.aibaodan.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cqd.zhixingplan.top

Java: x > 0 ? "yes" : "no"
来源：http://wdp.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xhg.daxiang520.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mdn.guowangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://bgf.pycfn.com

[A12] 字符串插值 / 格式化
来源：http://zbp.cashguo.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xyl.hnqzz.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gxc.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://nds.cucudq.cn

TS:   `Hello, ${name}!`
来源：http://kpf.guannengcc.top

Java: "Hello, %s!".formatted(name)
来源：http://fil.gotoacloud.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ltu.aibaodan.cn

Ruby: "Hello, #{name}!"
来源：http://hgl.hysaishi.cn

C#:   $"Hello, {name}!"
来源：http://tra.ctjpmb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://wuj.guannengcc.top

Py:   "第一行\n第二行"
来源：http://lua.jinyuanbaomall.cn

PHP:  "第一行\n第二行"
来源：http://ufn.nanxuanxn.top

JS:   "第一行\n第二行"
来源：http://znf.zhongyouzk.top

TS:   "第一行\n第二行"
来源：http://dkf.jinghuilouyu.cn

Java: "第一行\n第二行"
来源：http://mzy.jinqigufen.top

Go:   "第一行\n第二行"
来源：http://geu.daria6918.cn

Ruby: "第一行\n第二行"
来源：http://xym.cucudq.cn

C#:   "第一行\n第二行"
来源：http://snu.chenjidiqi.icu

[A14] 注释写法
来源：http://wdo.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vyh.sweek.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vjw.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://tiz.yj202588.top

TS:   // 单行；/* 多行 */
来源：http://otd.yfazqb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oon.yongpay.top

Go:   // 单行；/* 多行 */
来源：http://mla.dianchejie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wem.yangfankeji.com

C#:   // 单行；/* 多行 */
来源：http://jyw.zhiwuduotai.top

[A15] 空值判断与默认值
来源：http://iuv.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://tlj.pengpengdd.cyou

PHP:  $value = $data ?? "默认值";
来源：http://eoo.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://gvx.hysaishi.cn

TS:   const value = data ?? "默认值";
来源：http://xxf.c1oappe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jzb.bbcook.cn

Go:   if data == "" { data = "默认值" }
来源：http://hpw.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://oqe.yonumen.top

C#:   var value = data ?? "默认值";
来源：http://lqg.feifeiyinyue.top

[A16] 真假值判断规则
来源：http://hdw.nanxuanxn.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bye.jinqigfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://djb.xingfuxueyuan.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fwj.cucudq.cn

TS:   if (!x) {}
来源：http://frv.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://har.zhaomingkeji.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ipy.fanxiaobao.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://rvm.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iuu.jinqigfzy.top

[A17] 位运算
来源：http://jrg.zycfv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://snr.zdqjudy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jhb.cucudq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kwc.daria6918.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://isr.ppjwa.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kuv.fanxiaobao.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hwa.redwolf501.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xcp.ivvv.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://edd.ehwqpu.com

[A18] 字符与 ASCII 码互转
来源：http://wab.zhongyouzk.top

Py:   ord("A"); chr(65)
来源：http://xam.fktsv.cn

PHP:  ord("A"); chr(65)
来源：http://rdz.jlsjyb.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qhp.tarul.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lst.xuanzx.com

Java: (int) 'A'; (char) 65
来源：http://xhg.xuetiantiany.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pmc.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://qnq.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://tev.ehwqpu.com

[A19] 交换两个变量
来源：http://yzs.zdbjq.cn

Py:   a, b = b, a
来源：http://sdw.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://oim.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://coq.yanxiufei.cn

TS:   [a, b] = [b, a];
来源：http://zmq.jqgfzy.top

Java: int t = a; a = b; b = t;
来源：http://mtu.daria6918.cn

Go:   a, b = b, a
来源：http://rdv.gotoacloud.top

Ruby: a, b = b, a
来源：http://xoc.aibaodan.cn

C#:   (a, b) = (b, a);
来源：http://fxx.vqdsnc.cn

[A20] 读取标准输入
来源：http://ntv.meibo888.top

Py:   name = input("请输入：")
来源：http://ikm.hysaishi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wik.svipenyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gbd.bbcook.cn

TS:   // Node.js：readline 模块
来源：http://sef.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://zpf.mhx1999.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jvh.guowangkeji.top

Ruby: gets.chomp
来源：http://zia.birdmap.top

C#:   Console.ReadLine();
来源：http://vkw.yanxiufei.cn

[A21] 保留指定小数位输出
来源：http://pob.hywenlv.cn

Py:   f"{3.14159:.2f}"
来源：http://wnl.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nsp.sjlbkw.cn

JS:   (3.14159).toFixed(2)
来源：http://kfc.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://tas.hammf.cn

Java: String.format("%.2f", 3.14159)
来源：http://rqc.andypj.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vvz.gzhubu.top

Ruby: format("%.2f", 3.14159)
来源：http://ylv.xingfuxueyuan.xyz

C#:   3.14159.ToString("F2")
来源：http://qsn.daria6918.cn

[A22] 获取字符串长度
来源：http://sbo.jyoumei.cn

Py:   len(s)
来源：http://hbf.fengsongda.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mad.sufxvd.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nmh.haohaochexian.top

TS:   s.length
来源：http://ruu.52xcode.cn

Java: s.length()
来源：http://kvu.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nqt.gotoacloud.top

Ruby: s.length
来源：http://wdb.fktsv.cn

C#:   s.Length
来源：http://blv.epnwcf.com

[A23] 大小写转换
来源：http://rpt.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pov.aibaodan.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fbz.uphjek.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zgr.meibo888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://toq.yvedp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wfe.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://axd.tian-w.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zgl.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pti.redwolf501.top

[A24] 去除首尾空白
来源：http://npz.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yth.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://woh.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ays.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://knm.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dzj.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://osu.tianlin.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://afu.jlsjyb.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tvt.ydjk.org.cn

[A25] 字符串比较
来源：http://bpt.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://ili.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://weq.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yvq.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ekz.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pbg.jqgfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pol.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lpo.yfazqb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://npz.yj20258.top

[A26] 类型转换总览
来源：http://lmw.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cax.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wgr.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uwq.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://zzl.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xgd.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wbu.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wds.pycfn.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://czk.wangdashe.top

================================================================================
来源：http://jjk.yj20258888.top

B. 流程控制
来源：http://ihe.sxryk.cn

================================================================================
来源：http://cls.snrcjt.cn

[B01] 条件判断 if / else
来源：http://aop.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aup.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zwv.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ldg.gzhubu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yrk.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://oac.pengpengdd.cyou

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kuv.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mrv.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://udq.bbcook.cn

[B02] 多分支 else if / elif
来源：http://fat.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rhw.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ilf.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdo.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uvy.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gxn.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xpc.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tsf.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ege.dianchejie.cn

[B03] switch / match / case
来源：http://kax.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nzw.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oyg.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gqo.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rft.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dzo.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tbl.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xle.havefunace.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jqe.ctjpmb.com

[B04] for 计数循环
来源：http://vua.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://pfo.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tfa.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eyz.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgh.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pmk.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lkx.xuanzx.com

Ruby: 10.times { |i| puts i }
来源：http://aum.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mwd.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://yed.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://hkm.316326.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kkp.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qmp.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qqb.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://anz.sysykeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aig.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://yzq.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qul.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://nri.gotoacloud.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sxk.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mkx.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zst.bjfxy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qna.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://woy.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qpw.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cfz.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mxt.jinqigufen.top

[B07] while 循环
来源：http://uhq.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://bdt.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://cdb.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://ztn.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://eoy.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://npb.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://feq.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://oqo.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://ilz.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://wva.zdbjq.cn

Py:   # 无 do-while：用 while True + break
来源：http://uci.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://smd.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://uoy.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://ujd.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://vre.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://uol.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://fqw.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://oih.dashuyun.cn

[B09] break 与 continue
来源：http://qzw.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kgo.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ara.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://she.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hfi.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://biy.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lvo.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ctq.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvm.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://lol.havefunace.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iff.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qpu.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zwb.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qww.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jkw.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vax.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qbm.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gqn.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://ico.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://cxm.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://bds.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://enk.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ejv.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zsw.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://htx.iojbl.cn

Ruby: (0...10).step(2).to_a
来源：http://kho.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ptb.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://vvz.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://xyr.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://org.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://med.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ykv.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ibk.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fjw.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ldg.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rhw.zdbjq.cn

[B13] 判断是否为数字
来源：http://nit.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://onj.haohaochexian.top

PHP:  is_numeric($x)
来源：http://nkm.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vtg.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blh.zhixingplan.top

Java: x instanceof Number
来源：http://ppb.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ord.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://uum.zycfv.cn

C#:   x is int or double or decimal
来源：http://gko.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://eon.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cbd.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jjb.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://gjb.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://czj.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zpm.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gov.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://xvd.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zse.yuxming.cn

[B15] 布尔运算与取反
来源：http://nni.zhengqikj.top

Py:   a and b or not c
来源：http://dhx.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://wid.c1oappe.top

JS:   a && b || !c
来源：http://xhf.fktsv.cn

TS:   a && b || !c
来源：http://xhi.feifeiyinyue.top

Java: a && b || !c
来源：http://eyv.fktsv.cn

Go:   a && b || !c
来源：http://cvq.pengpengdd.cyou

Ruby: a && b || !c
来源：http://izn.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://pwd.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://myh.gotoacloud.top

Py:   if not data: return
来源：http://ccg.ydzc1.top

PHP:  if (!$data) { return; }
来源：http://rig.ppjwa.cn

JS:   if (!data) return;
来源：http://kok.zycfv.cn

TS:   if (!data) return;
来源：http://mze.yj20258.top

Java: if (data == null) return;
来源：http://onk.dashuyun.cn

Go:   if data == nil { return }
来源：http://sph.yangfankeji.com

Ruby: return if data.nil?
来源：http://jdo.chenzaomai.com

C#:   if (data == null) return;
来源：http://kko.vqdsnc.cn


<!-- 参考信息 -->