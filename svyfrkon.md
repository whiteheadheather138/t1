代发 wailian999

[A10] 生成随机数
来源：http://mxt.ctjpmb.com

Py:   import random; random.randint(1, 100)
来源：http://jiz.xuanzx.com

PHP:  random_int(1, 100);
来源：http://obv.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://isi.guowangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://and.daxiang520.top

Java: new Random().nextInt(100) + 1
来源：http://naj.fanxiaobao.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tdn.yuxming.cn

Ruby: rand(1..100)
来源：http://otp.jianghu66.top

C#:   new Random().Next(1, 101)
来源：http://rkk.sweek.top

[A11] 条件表达式（三元）
来源：http://sxp.hysaishi.cn

Py:   "yes" if x > 0 else "no"
来源：http://aoo.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://jnx.smart0.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://xwn.cdnleiting.top

TS:   x > 0 ? "yes" : "no"
来源：http://ite.yueranfly.top

Java: x > 0 ? "yes" : "no"
来源：http://loa.yfazqb.com

Go:   // 无三元运算符，需用 if 语句
来源：http://qdf.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://eyb.fktsv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://frw.hnqzz.top

[A12] 字符串插值 / 格式化
来源：http://bdk.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lpo.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cvc.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://ufm.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://eos.jyoumei.cn

Java: "Hello, %s!".formatted(name)
来源：http://bhv.shanyushiyangtech.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ajt.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://dfb.gotoacloud.top

C#:   $"Hello, {name}!"
来源：http://npi.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pun.9152youxi.cn

Py:   "第一行\n第二行"
来源：http://fyi.xinyue.icu

PHP:  "第一行\n第二行"
来源：http://xyo.c1oappe.top

JS:   "第一行\n第二行"
来源：http://kck.yuxming.cn

TS:   "第一行\n第二行"
来源：http://nlo.chenlongwang.top

Java: "第一行\n第二行"
来源：http://kfg.hesvh.cn

Go:   "第一行\n第二行"
来源：http://rnj.haohaochexian.top

Ruby: "第一行\n第二行"
来源：http://uqr.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://wrh.cucudq.cn

[A14] 注释写法
来源：http://jpm.daria6918.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jza.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lpd.svipenyu.cn

JS:   // 单行；/* 多行 */
来源：http://xlu.sweek.top

TS:   // 单行；/* 多行 */
来源：http://lzb.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gic.gotoacloud.top

Go:   // 单行；/* 多行 */
来源：http://tzg.sweek.top

Ruby: # 单行；=begin 多行 =end
来源：http://sja.xingfuxueyuan.xyz

C#:   // 单行；/* 多行 */
来源：http://dua.tianlin.xyz

[A15] 空值判断与默认值
来源：http://pqj.ctjpmb.com

Py:   value = data or "默认值"
来源：http://jdu.yonumen.top

PHP:  $value = $data ?? "默认值";
来源：http://ihw.zhongyouzk.top

JS:   const value = data ?? "默认值";
来源：http://rsd.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://rip.zdbjq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://suv.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://dfs.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://uyz.yongpay.top

C#:   var value = data ?? "默认值";
来源：http://ela.zhengqikj.top

[A16] 真假值判断规则
来源：http://gzn.guannengcc.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cht.kuanghao11.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rub.ppjwa.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jwc.yangfankeji.com

TS:   if (!x) {}
来源：http://mhg.haohaochexian.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gil.feifeiyinyue.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lqr.chenzaomai.com

Ruby: unless x            # nil 与 false 为假
来源：http://rco.zdqjudy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://srb.dianchejie.cn

[A17] 位运算
来源：http://jkk.feifeiyinyue.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://poe.tian-w.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://add.hfpthk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gmm.jiagoushi.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cqu.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mas.sxryk.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://geq.ywan-chungtsiang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jjb.gotoacloud.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nps.nwbrower.top

[A18] 字符与 ASCII 码互转
来源：http://ijw.hammf.cn

Py:   ord("A"); chr(65)
来源：http://xaw.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://vnl.ybcxt.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jje.hcnkem.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hgt.316326.xyz

Java: (int) 'A'; (char) 65
来源：http://drw.gogol.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jar.pengpengdd.cyou

Ruby: "A".ord; 65.chr
来源：http://tao.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://akn.jinqigufen.top

[A19] 交换两个变量
来源：http://ftg.yvedp.cn

Py:   a, b = b, a
来源：http://tlo.sufxvd.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://svk.hammf.cn

JS:   [a, b] = [b, a];
来源：http://epd.hysaishi.cn

TS:   [a, b] = [b, a];
来源：http://smi.jqgufenzy.top

Java: int t = a; a = b; b = t;
来源：http://rpy.sjlbkw.cn

Go:   a, b = b, a
来源：http://kjd.ctjpmb.com

Ruby: a, b = b, a
来源：http://rvk.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://wci.jlsjyb.cn

[A20] 读取标准输入
来源：http://kqn.0kj1m.cn

Py:   name = input("请输入：")
来源：http://itx.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ggx.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dti.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://cle.yongpay.top

Java: new Scanner(System.in).nextLine()
来源：http://sxf.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ngx.52xcode.cn

Ruby: gets.chomp
来源：http://nfj.yongpay.top

C#:   Console.ReadLine();
来源：http://xrd.hnxiangtu.top

[A21] 保留指定小数位输出
来源：http://dea.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://qyv.jianghu66.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ezy.mhx1999.top

JS:   (3.14159).toFixed(2)
来源：http://pbh.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://rvw.tian-w.cn

Java: String.format("%.2f", 3.14159)
来源：http://xgp.yuanzhike.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fjz.jinghuilouyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://fuf.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://ifg.yangfankeji.com

[A22] 获取字符串长度
来源：http://euc.xuanzx.com

Py:   len(s)
来源：http://zmr.jyoumei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nzs.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mrl.jinqigfzy.top

TS:   s.length
来源：http://yyg.chenlongwang.top

Java: s.length()
来源：http://zoi.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vaa.yj20258.top

Ruby: s.length
来源：http://fzm.tianlin.xyz

C#:   s.Length
来源：http://ftr.sysykeji.top

[A23] 大小写转换
来源：http://xqa.zhixingplan.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bty.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qxp.ydzc1.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bik.hammf.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gyr.sxryk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ibq.jqgfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ujp.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pkp.gzhubu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ijh.wangdashe.top

[A24] 去除首尾空白
来源：http://odx.tian-w.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rbo.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tbt.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nri.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xab.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ara.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://xks.zhixingplan.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hch.sxryk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ncr.yj202588.top

[A25] 字符串比较
来源：http://hex.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://bur.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bbf.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rfz.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xdg.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rgq.havefunace.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rkx.ydzc1.top

Ruby: s1 == s2; s1 <=> s2
来源：http://trs.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xtp.sufxvd.cn

[A26] 类型转换总览
来源：http://dys.ydzc1.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yro.zhijiandao.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://puq.cqqwz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://buq.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://ykb.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hsc.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://krr.vehdjk.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://dqb.sxryk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oia.shanyushiyangtech.top

================================================================================
来源：http://gln.hysaishi.cn

B. 流程控制
来源：http://tcv.cheryme.top

================================================================================
来源：http://nxp.sufxvd.cn

[B01] 条件判断 if / else
来源：http://myw.cqqwz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rek.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yeu.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ayc.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nbx.dianchejie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lhn.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dpo.tarul.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lir.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sbk.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://jkm.redwolf501.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bnv.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://san.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ttv.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgr.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lov.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bvj.vqdsnc.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eis.nwbrower.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dhv.xuetiantiany.cn

[B03] switch / match / case
来源：http://jwk.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eji.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kfm.yj20258888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lbc.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vkf.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ocw.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kxv.tianlin.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yha.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hjf.yonumen.top

[B04] for 计数循环
来源：http://lpr.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://ika.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://srx.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://onw.xylfe.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mji.xylfe.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iyi.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rfr.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://vgo.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zsc.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://evq.hesvh.cn

Py:   for item in arr: print(item)
来源：http://lef.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fyh.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uvc.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://oyp.jqgfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ent.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gsz.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://qyi.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uiz.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://tqt.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://gvt.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xdn.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vch.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bhc.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wtz.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wbi.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://okw.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://umm.yvedp.cn

[B07] while 循环
来源：http://agh.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://jmo.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://zkx.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://bsh.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://oeo.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://unm.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://amw.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://amd.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://pqy.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://lbd.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://nqo.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://bfi.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://eoo.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://rdv.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://mqz.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zgx.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://nja.zhaomingkeji.xyz

C#:   do { i++; } while (i < 10);
来源：http://rff.zhiwuduotai.top

[B09] break 与 continue
来源：http://cyr.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eqj.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gta.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyb.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lpj.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qrl.yuanzhike.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://deo.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ckb.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bpi.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://jpm.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ktu.yueranfly.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fyp.nwbrower.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zgb.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wgq.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fmb.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ihk.havefunace.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nsf.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lbb.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://czn.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://uku.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://opd.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nut.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cin.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://keu.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wdd.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://eyw.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qee.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://tbn.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://loi.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://suy.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iac.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xyx.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://csw.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ezo.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vgx.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ewg.zycfv.cn

[B13] 判断是否为数字
来源：http://brh.meibo888.top

Py:   isinstance(x, (int, float))
来源：http://ocf.iojbl.cn

PHP:  is_numeric($x)
来源：http://xed.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vyh.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://etp.chenjidiqi.icu

Java: x instanceof Number
来源：http://chl.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bza.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://hki.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://qdx.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://qqw.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://smx.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://fht.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://tuu.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xku.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://upx.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://ouq.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mvv.hnqzz.top

[B15] 布尔运算与取反
来源：http://pgm.quarkkingdee.top

Py:   a and b or not c
来源：http://mdn.xziqi.cn

PHP:  $a && $b || !$c
来源：http://ssl.jianghu66.top

JS:   a && b || !c
来源：http://vrw.jyoumei.cn

TS:   a && b || !c
来源：http://cxv.fehbvm.com

Java: a && b || !c
来源：http://ybq.shzxlz.cn

Go:   a && b || !c
来源：http://inh.tianlin.xyz

Ruby: a && b || !c
来源：http://rof.yuanzhike.top

C#:   a && b || !c
来源：http://izm.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ciu.tian-w.cn

Py:   if not data: return
来源：http://cys.uphjek.com

PHP:  if (!$data) { return; }
来源：http://fte.gaohongyu789.top

JS:   if (!data) return;
来源：http://mrz.zhijiandao.cn

TS:   if (!data) return;
来源：http://qhr.gotoacloud.top

Java: if (data == null) return;
来源：http://jta.cucudq.cn

Go:   if data == nil { return }
来源：http://ire.yj20258.top

Ruby: return if data.nil?
来源：http://cim.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://qcu.daria6918.cn


<!-- 参考信息 -->