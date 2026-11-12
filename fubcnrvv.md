代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://adc.0kj1m.cn

JS:   `Hello, ${name}!`
来源：http://she.tarul.cn

TS:   `Hello, ${name}!`
来源：http://zbi.hesvh.cn

Java: "Hello, %s!".formatted(name)
来源：http://hxr.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wec.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://zzf.chenjidiqi.icu

C#:   $"Hello, {name}!"
来源：http://xgf.yuanzhike.top

[A13] 多行字符串（练习 \n 转义）
来源：http://doo.fktsv.cn

Py:   "第一行\n第二行"
来源：http://eys.jiagoushi.top

PHP:  "第一行\n第二行"
来源：http://vgg.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://xwk.xuetiantiany.cn

TS:   "第一行\n第二行"
来源：http://yrg.jqgufenzy.top

Java: "第一行\n第二行"
来源：http://fvu.yongpay.top

Go:   "第一行\n第二行"
来源：http://ogy.nwbrower.top

Ruby: "第一行\n第二行"
来源：http://ivb.nanxinkj.top

C#:   "第一行\n第二行"
来源：http://gqy.hfpthk.cn

[A14] 注释写法
来源：http://hzx.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://prx.kuanghao11.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wmy.vqdsnc.cn

JS:   // 单行；/* 多行 */
来源：http://akb.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://vna.zhengqikj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pwy.dashuyun.cn

Go:   // 单行；/* 多行 */
来源：http://rwc.c1oappe.top

Ruby: # 单行；=begin 多行 =end
来源：http://qmr.yongpay.top

C#:   // 单行；/* 多行 */
来源：http://onc.ppjwa.cn

[A15] 空值判断与默认值
来源：http://qax.cucudq.cn

Py:   value = data or "默认值"
来源：http://rgk.pengpengdd.cyou

PHP:  $value = $data ?? "默认值";
来源：http://wyy.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://mfo.andypj.xyz

TS:   const value = data ?? "默认值";
来源：http://xpm.svipenyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://omt.jqgufenzy.top

Go:   if data == "" { data = "默认值" }
来源：http://vtw.aibaodan.cn

Ruby: value = data || "默认值"
来源：http://ghk.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://olh.jiagoushi.top

[A16] 真假值判断规则
来源：http://xbg.nwbrower.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rmr.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nyb.jinqigfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kea.tian-w.cn

TS:   if (!x) {}
来源：http://esj.aizwys.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mmn.zhongyouzk.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vzc.9152youxi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://swu.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zix.ivvv.top

[A17] 位运算
来源：http://tmc.zhixingplan.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uor.zdbjq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cuj.cqqwz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://inm.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://row.yj20258.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vfv.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://trd.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://evk.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mac.xingfuxueyuan.xyz

[A18] 字符与 ASCII 码互转
来源：http://vrk.ydzc1.top

Py:   ord("A"); chr(65)
来源：http://iud.fengsongda.top

PHP:  ord("A"); chr(65)
来源：http://lgq.pycfn.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pmw.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://krm.sysykeji.top

Java: (int) 'A'; (char) 65
来源：http://veu.pengpengdd.cyou

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kpm.feifeiyinyue.top

Ruby: "A".ord; 65.chr
来源：http://ppz.ehwqpu.com

C#:   (int)'A'; (char)65
来源：http://azs.hywenlv.cn

[A19] 交换两个变量
来源：http://vho.pengpengdd.cyou

Py:   a, b = b, a
来源：http://kdc.sufxvd.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tyv.c1oappe.top

JS:   [a, b] = [b, a];
来源：http://rbl.havefunace.top

TS:   [a, b] = [b, a];
来源：http://qxp.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://qtc.aizwys.cn

Go:   a, b = b, a
来源：http://spa.feifeiyinyue.top

Ruby: a, b = b, a
来源：http://tqs.zhengqikj.top

C#:   (a, b) = (b, a);
来源：http://kbj.316326.xyz

[A20] 读取标准输入
来源：http://ufw.sufxvd.cn

Py:   name = input("请输入：")
来源：http://qgb.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://cwn.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sbh.snrcjt.cn

TS:   // Node.js：readline 模块
来源：http://dis.daria6918.cn

Java: new Scanner(System.in).nextLine()
来源：http://zbv.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fnm.hongshengwenyu.top

Ruby: gets.chomp
来源：http://fgb.daria6918.cn

C#:   Console.ReadLine();
来源：http://iuu.yj20258888.top

[A21] 保留指定小数位输出
来源：http://ulj.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://twv.zdbjq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lpv.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://lzw.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://jqb.vqdsnc.cn

Java: String.format("%.2f", 3.14159)
来源：http://ivl.nanxinkj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pnl.hnxiangtu.top

Ruby: format("%.2f", 3.14159)
来源：http://rzn.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://yrf.hysaishi.cn

[A22] 获取字符串长度
来源：http://yzs.yuanzhike.top

Py:   len(s)
来源：http://vio.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sto.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hdo.vehdjk.com

TS:   s.length
来源：http://sik.yuanzhike.top

Java: s.length()
来源：http://iuh.hcnkem.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sku.bbcook.cn

Ruby: s.length
来源：http://myh.nanxinkj.top

C#:   s.Length
来源：http://hxe.yuxming.cn

[A23] 大小写转换
来源：http://zim.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ozg.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dmn.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gvc.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mbw.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rbn.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mog.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vmq.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lpd.vehdjk.com

[A24] 去除首尾空白
来源：http://aoz.hfpthk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dgb.hysaishi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ldi.chenlongwang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yod.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bcx.chenzaomai.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gwt.hnxiangtu.top

Go:   strings.TrimSpace(s)
来源：http://log.hysaishi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yqh.xingfuxueyuan.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vke.mhx1999.top

[A25] 字符串比较
来源：http://ets.havefunace.top

Py:   s1 == s2; s1 != s2
来源：http://woa.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fid.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jvo.shanyushiyangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jab.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vut.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xgw.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://gvv.52xcode.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ktt.zdbjq.cn

[A26] 类型转换总览
来源：http://iud.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xgx.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wqw.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ksm.fengsongda.top

TS:   Number() String() Boolean() x as number
来源：http://fgx.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jpd.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cpx.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://oys.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://etm.gzhubu.top

================================================================================
来源：http://mlk.daria6918.cn

B. 流程控制
来源：http://qqu.sxryk.cn

================================================================================
来源：http://csm.mhx1999.top

[B01] 条件判断 if / else
来源：http://bin.wangshuangyany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vkv.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qvo.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nns.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wzw.smart0.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://pvq.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nxu.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wms.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://auc.9152youxi.cn

[B02] 多分支 else if / elif
来源：http://chx.yfazqb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jgd.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://irr.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lib.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yku.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jke.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bmj.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xeq.nwbrower.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wzr.zhoulong.xyz

[B03] switch / match / case
来源：http://mom.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://izj.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nna.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lrl.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rve.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://scp.zycfv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://inn.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fcu.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qqo.yuxming.cn

[B04] for 计数循环
来源：http://hpr.316326.xyz

Py:   for i in range(10): print(i)
来源：http://jnk.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hjw.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yas.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vyp.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zhj.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uzb.0kj1m.cn

Ruby: 10.times { |i| puts i }
来源：http://kyj.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tak.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://wzy.gzhubu.top

Py:   for item in arr: print(item)
来源：http://sbu.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mxb.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mrc.ehwqpu.com

TS:   for (const item of arr) { console.log(item); }
来源：http://qop.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hli.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yek.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://zcp.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://haj.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://tfe.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qzi.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qlu.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ofs.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sib.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xtj.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qef.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://elp.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wen.xuanzx.com

[B07] while 循环
来源：http://ikd.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://eto.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://iht.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://sga.9152youxi.cn

TS:   while (i < 10) { i++; }
来源：http://amd.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://gae.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xkd.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://qfu.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://qnu.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://abx.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://gsh.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yod.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://tys.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://myu.sweek.top

Java: do { i++; } while (i < 10);
来源：http://dtf.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hzk.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://sow.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://yph.daria6918.cn

[B09] break 与 continue
来源：http://ens.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ner.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fpu.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://apn.fehbvm.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxe.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://auv.fktsv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mea.aizwys.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oaw.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggb.birdmap.top

[B10] 遍历同时拿索引
来源：http://anx.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mfz.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kfd.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fla.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://avx.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zhc.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aag.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pid.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xum.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://brq.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://sfl.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://ifm.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://khn.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aii.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wsv.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iut.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://rbk.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wef.cdnleiting.top

[B12] 跳出多层循环
来源：http://mwm.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bgw.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mgw.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sar.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://myy.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lpa.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fvh.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lld.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tbt.52xcode.cn

[B13] 判断是否为数字
来源：http://zkx.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://iqy.cashguo.top

PHP:  is_numeric($x)
来源：http://zor.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cgg.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pnf.yuanzhike.top

Java: x instanceof Number
来源：http://dsr.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tfw.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://ywm.yonumen.top

C#:   x is int or double or decimal
来源：http://jam.fehbvm.com

[B14] 判断值是否在集合内
来源：http://gwx.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://onv.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sgi.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://gyu.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://wjb.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qnd.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gyk.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ulf.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zvl.zdqjudy.top

[B15] 布尔运算与取反
来源：http://gji.chenzaomai.com

Py:   a and b or not c
来源：http://jfg.birdmap.top

PHP:  $a && $b || !$c
来源：http://yqw.ydjk.org.cn

JS:   a && b || !c
来源：http://mlo.ydzc1.top

TS:   a && b || !c
来源：http://lje.ybcxt.top

Java: a && b || !c
来源：http://hyv.jinyuanbaomall.cn

Go:   a && b || !c
来源：http://dpy.chenjidiqi.icu

Ruby: a && b || !c
来源：http://jqn.zhixingplan.top

C#:   a && b || !c
来源：http://nqt.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://upq.zdbjq.cn

Py:   if not data: return
来源：http://ckj.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://pny.pengpengdd.cyou

JS:   if (!data) return;
来源：http://sff.0kj1m.cn

TS:   if (!data) return;
来源：http://mjy.hnqzz.top

Java: if (data == null) return;
来源：http://xpr.dashuyun.cn

Go:   if data == nil { return }
来源：http://aub.hnxiangtu.top

Ruby: return if data.nil?
来源：http://cfm.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://ynx.daria6918.cn

================================================================================
来源：http://wqp.hcnkem.com

C. 函数与作用域
来源：http://xjn.yj202588.top

================================================================================
来源：http://way.daxiang520.top

[C01] 定义函数
来源：http://jzs.hfpthk.cn

Py:   def add(a, b): return a + b
来源：http://cct.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vkz.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://kst.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pst.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://pbb.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hxu.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://wrz.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ojm.chenlongwang.top

[C02] 默认参数
来源：http://uma.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://qqa.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ylb.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://rfz.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://euq.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kjl.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yma.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://qio.nwbrower.top


<!-- 参考信息 -->