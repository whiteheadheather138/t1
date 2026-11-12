代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mwc.jianghu66.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://frk.hcnkem.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://odz.shanyushiyangtech.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gtb.hammf.cn

[A10] 生成随机数
来源：http://vei.meibo888.top

Py:   import random; random.randint(1, 100)
来源：http://gsv.shangyingyoupin.top

PHP:  random_int(1, 100);
来源：http://lnn.aizwys.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lsr.nwbrower.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zzr.ywan-chungtsiang.top

Java: new Random().nextInt(100) + 1
来源：http://djk.pengpengdd.cyou

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dou.yueranfly.top

Ruby: rand(1..100)
来源：http://bax.yueranfly.top

C#:   new Random().Next(1, 101)
来源：http://tvl.gogol.net.cn

[A11] 条件表达式（三元）
来源：http://qtp.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://txz.mhx1999.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yua.svipenyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pyl.shanyushiyangtech.top

TS:   x > 0 ? "yes" : "no"
来源：http://blo.xziqi.cn

Java: x > 0 ? "yes" : "no"
来源：http://pbr.kuanghao11.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dnv.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wgo.ehwqpu.com

C#:   x > 0 ? "yes" : "no"
来源：http://tfh.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://tdm.hywenlv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aqm.yvedp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://klg.pycfn.com

JS:   `Hello, ${name}!`
来源：http://gwf.gaohongyu789.top

TS:   `Hello, ${name}!`
来源：http://nln.yj202588.top

Java: "Hello, %s!".formatted(name)
来源：http://lus.havefunace.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hxh.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://ukm.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://gze.zycfv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://unn.jlsjyb.cn

Py:   "第一行\n第二行"
来源：http://rpn.ybcxt.top

PHP:  "第一行\n第二行"
来源：http://snu.shanyushiyangtech.top

JS:   "第一行\n第二行"
来源：http://wtn.vehdjk.com

TS:   "第一行\n第二行"
来源：http://azt.fanxiaobao.xyz

Java: "第一行\n第二行"
来源：http://foe.chenlongwang.top

Go:   "第一行\n第二行"
来源：http://agk.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://fms.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://uyd.xingfuxueyuan.xyz

[A14] 注释写法
来源：http://vxf.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wtl.hysaishi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://asi.zycfv.cn

JS:   // 单行；/* 多行 */
来源：http://vln.aibaodan.cn

TS:   // 单行；/* 多行 */
来源：http://gzb.nanxinkj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gpl.yuxming.cn

Go:   // 单行；/* 多行 */
来源：http://isv.ehwqpu.com

Ruby: # 单行；=begin 多行 =end
来源：http://mxr.ehwqpu.com

C#:   // 单行；/* 多行 */
来源：http://hes.aibaodan.cn

[A15] 空值判断与默认值
来源：http://jiq.shanyushiyangkeji.top

Py:   value = data or "默认值"
来源：http://mli.zycfv.cn

PHP:  $value = $data ?? "默认值";
来源：http://tsz.xinyue.icu

JS:   const value = data ?? "默认值";
来源：http://xbb.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://pnp.hcnkem.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://aib.yvedp.cn

Go:   if data == "" { data = "默认值" }
来源：http://tgb.gogol.net.cn

Ruby: value = data || "默认值"
来源：http://rmr.yj20258888.top

C#:   var value = data ?? "默认值";
来源：http://axa.yonumen.top

[A16] 真假值判断规则
来源：http://ore.yanxiufei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tid.andypj.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xfe.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nhd.yueranfly.top

TS:   if (!x) {}
来源：http://xhf.316326.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ymz.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bgy.jianghu66.top

Ruby: unless x            # nil 与 false 为假
来源：http://tay.fzhhl.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bik.yfazqb.com

[A17] 位运算
来源：http://fht.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nss.gogol.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rtp.shanyushiyangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://and.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fej.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://leh.zhoulong.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jyc.aibaodan.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hnn.chenjidiqi.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gng.jinghuilouyu.cn

[A18] 字符与 ASCII 码互转
来源：http://dfg.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://fxe.tanke756.top

PHP:  ord("A"); chr(65)
来源：http://ond.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iig.nwbrower.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ezi.jqgfzy.top

Java: (int) 'A'; (char) 65
来源：http://xgg.yanxiufei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kbf.jyoumei.cn

Ruby: "A".ord; 65.chr
来源：http://wht.yanxiufei.cn

C#:   (int)'A'; (char)65
来源：http://qmu.zhoulong.xyz

[A19] 交换两个变量
来源：http://rvu.ydzc1.top

Py:   a, b = b, a
来源：http://tgm.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kcw.meibo888.top

JS:   [a, b] = [b, a];
来源：http://izs.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://jld.guannengcc.top

Java: int t = a; a = b; b = t;
来源：http://zav.aibaodan.cn

Go:   a, b = b, a
来源：http://ejv.svipenyu.cn

Ruby: a, b = b, a
来源：http://ecf.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://lsw.snrcjt.cn

[A20] 读取标准输入
来源：http://elm.aizwys.cn

Py:   name = input("请输入：")
来源：http://tua.zhixingplan.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ezm.kuanghao11.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wed.tianlin.xyz

TS:   // Node.js：readline 模块
来源：http://zuq.cucudq.cn

Java: new Scanner(System.in).nextLine()
来源：http://jdr.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://htm.jqgfzy.top

Ruby: gets.chomp
来源：http://vns.ppjwa.cn

C#:   Console.ReadLine();
来源：http://tbo.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://elw.wangdashe.top

Py:   f"{3.14159:.2f}"
来源：http://rrv.sweek.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://irl.chenzaomai.com

JS:   (3.14159).toFixed(2)
来源：http://ksj.feifeiyinyue.top

TS:   (3.14159).toFixed(2)
来源：http://zxn.svipenyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://eun.xinyue.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xii.ywan-chungtsiang.top

Ruby: format("%.2f", 3.14159)
来源：http://seo.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://zyu.vqdsnc.cn

[A22] 获取字符串长度
来源：http://jfd.zhixingplan.top

Py:   len(s)
来源：http://ytv.yonumen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ehg.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fsz.yj20258888.top

TS:   s.length
来源：http://gmg.jinyuanbaomall.cn

Java: s.length()
来源：http://wuu.redwolf501.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gqx.cheryme.top

Ruby: s.length
来源：http://aie.jianghu66.top

C#:   s.Length
来源：http://rqk.xuetiantiany.cn

[A23] 大小写转换
来源：http://xop.snrcjt.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fmb.fengsongda.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hwl.andypj.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bpx.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vzy.vehdjk.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ieu.zhiwuduotai.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bwe.0kj1m.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mrp.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://usq.ivvv.top

[A24] 去除首尾空白
来源：http://ngc.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nsl.zhijiandao.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cwz.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rdi.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mfc.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fhq.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://npx.zhengqikj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wzs.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pae.jqgufenzy.top

[A25] 字符串比较
来源：http://gxf.shanyushiyangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://nir.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bhp.c1oappe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yvl.ppjwa.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yci.ydzc1.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qks.vqdsnc.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yga.daria6918.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tja.dianchejie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rzs.kuanghao11.cn

[A26] 类型转换总览
来源：http://ovc.dashuyun.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dyj.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rie.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yzu.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://iki.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bor.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oog.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://jbd.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rqs.aizwys.cn

================================================================================
来源：http://hzz.yanxiufei.cn

B. 流程控制
来源：http://bth.bbcook.cn

================================================================================
来源：http://tfx.xziqi.cn

[B01] 条件判断 if / else
来源：http://kbn.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://fnn.zhiwuduotai.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eiz.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://urm.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://haj.cqqwz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bxl.cheryme.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bah.jiagoushi.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cju.jianghu66.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nme.hesvh.cn

[B02] 多分支 else if / elif
来源：http://lzi.jiagoushi.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vgb.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ahz.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lyv.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvu.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dvv.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yql.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zwr.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxe.xylfe.cn

[B03] switch / match / case
来源：http://ejz.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pok.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cds.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bgj.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pkc.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zuz.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uun.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gwo.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gmj.hcnkem.com

[B04] for 计数循环
来源：http://kfr.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://enn.tian-w.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kpm.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://idp.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dxf.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dkm.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bme.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://uhg.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://txs.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://meo.tarul.cn

Py:   for item in arr: print(item)
来源：http://klg.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lmt.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ozs.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://hzy.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dfi.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uad.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://joa.hysaishi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hrx.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://vdi.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://new.snrcjt.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sli.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mes.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fbf.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hvs.sxryk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cdm.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ysc.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wmr.sufxvd.cn

[B07] while 循环
来源：http://cqk.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://nyw.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://aak.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://fon.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://qyx.sweek.top

Java: while (i < 10) { i++; }
来源：http://aom.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://edb.hywenlv.cn

Ruby: while i < 10; i += 1; end
来源：http://qlc.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://spq.pycfn.com

[B08] do-while（至少执行一次）
来源：http://fkn.sysykeji.top

Py:   # 无 do-while：用 while True + break
来源：http://czl.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xhx.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://ldi.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://hjw.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://psj.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://spk.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://hyv.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://odf.shanyushiyangtech.top

[B09] break 与 continue
来源：http://kse.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://byl.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lgo.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rko.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://din.hongshengwenyu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqz.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://paa.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lew.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kcg.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://prf.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xbw.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kml.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pef.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lxn.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bda.hcnkem.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ppa.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ogs.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gfw.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://gsq.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://nja.uphjek.com

PHP:  range(0, 10, 2);
来源：http://jeh.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://swx.ybcxt.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ngz.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qee.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xdk.yueranfly.top

Ruby: (0...10).step(2).to_a
来源：http://ioc.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mnl.gaohongyu789.top

[B12] 跳出多层循环
来源：http://soj.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rez.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://prb.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ziy.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jpu.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ujv.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pnp.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wsb.snrcjt.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dex.cdnleiting.top

[B13] 判断是否为数字
来源：http://mka.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://oim.52xcode.cn

PHP:  is_numeric($x)
来源：http://ngd.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iiw.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tkq.0kj1m.cn

Java: x instanceof Number
来源：http://gie.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://too.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://gtd.gotoacloud.top

C#:   x is int or double or decimal
来源：http://mla.yvedp.cn

[B14] 判断值是否在集合内
来源：http://vlh.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rhh.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lkg.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://gne.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://cuu.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kts.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hoi.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gxd.iojbl.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gog.xuanzx.com

[B15] 布尔运算与取反
来源：http://bkm.ydjk.org.cn

Py:   a and b or not c
来源：http://pgg.316326.xyz

PHP:  $a && $b || !$c
来源：http://ajf.fzhhl.top

JS:   a && b || !c
来源：http://utr.nwbrower.top

TS:   a && b || !c
来源：http://fud.yueranfly.top

Java: a && b || !c
来源：http://ikd.hysaishi.cn

Go:   a && b || !c
来源：http://znv.dashuyun.cn

Ruby: a && b || !c
来源：http://zdb.jlsjyb.cn

C#:   a && b || !c
来源：http://znm.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://hxq.quarkkingdee.top

Py:   if not data: return
来源：http://bij.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://tru.smart0.xyz

JS:   if (!data) return;
来源：http://iai.andypj.xyz

TS:   if (!data) return;
来源：http://jeu.zhijiandao.cn


<!-- 参考信息 -->