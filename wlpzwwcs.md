代发 wailian999

[A14] 注释写法
来源：http://dee.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pfh.ctjpmb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://fgz.yangfankeji.com

JS:   // 单行；/* 多行 */
来源：http://qut.chenlongwang.top

TS:   // 单行；/* 多行 */
来源：http://sby.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ddr.xylfe.cn

Go:   // 单行；/* 多行 */
来源：http://pqb.bjfxy.top

Ruby: # 单行；=begin 多行 =end
来源：http://mgg.mhx1999.top

C#:   // 单行；/* 多行 */
来源：http://pot.zhengqikj.top

[A15] 空值判断与默认值
来源：http://ijh.zhoulong.xyz

Py:   value = data or "默认值"
来源：http://rls.gzhubu.top

PHP:  $value = $data ?? "默认值";
来源：http://nnv.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://hpp.fzhhl.top

TS:   const value = data ?? "默认值";
来源：http://wys.birdmap.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kmj.nanxuanxn.top

Go:   if data == "" { data = "默认值" }
来源：http://rkp.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://tap.ehwqpu.com

C#:   var value = data ?? "默认值";
来源：http://lcm.chenjidiqi.icu

[A16] 真假值判断规则
来源：http://lvv.cucudq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fes.guowangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://noy.kuanghao11.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pdn.9152youxi.cn

TS:   if (!x) {}
来源：http://udp.vehdjk.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dzq.meibo888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vyv.wangshuangyany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hwn.mhx1999.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fbt.gotoacloud.top

[A17] 位运算
来源：http://gyc.yj202588.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tfi.xylfe.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ysd.bbcook.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jqy.fktsv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jxz.shangyingyoupin.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zmo.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vai.birdmap.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mdo.sufxvd.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cbf.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://zkl.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://ftz.yj202588.top

PHP:  ord("A"); chr(65)
来源：http://hcm.ywan-chungtsiang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uuw.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xsc.chenlongwang.top

Java: (int) 'A'; (char) 65
来源：http://iqo.jlsjyb.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ocq.shanyushiyangkeji.top

Ruby: "A".ord; 65.chr
来源：http://btx.xingfuxueyuan.xyz

C#:   (int)'A'; (char)65
来源：http://zkz.pengpengdd.cyou

[A19] 交换两个变量
来源：http://wld.fzhhl.top

Py:   a, b = b, a
来源：http://rog.mhx1999.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jik.yangfankeji.com

JS:   [a, b] = [b, a];
来源：http://qdy.smart0.xyz

TS:   [a, b] = [b, a];
来源：http://tkz.sweek.top

Java: int t = a; a = b; b = t;
来源：http://fhh.zycfv.cn

Go:   a, b = b, a
来源：http://zab.guannengcc.top

Ruby: a, b = b, a
来源：http://aax.haohaochexian.top

C#:   (a, b) = (b, a);
来源：http://uba.tianlin.xyz

[A20] 读取标准输入
来源：http://wlp.bbcook.cn

Py:   name = input("请输入：")
来源：http://foh.iojbl.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cdf.316326.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rnm.yangfankeji.com

TS:   // Node.js：readline 模块
来源：http://flz.wangdashe.top

Java: new Scanner(System.in).nextLine()
来源：http://wsl.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kao.yanxiufei.cn

Ruby: gets.chomp
来源：http://nug.shzxlz.cn

C#:   Console.ReadLine();
来源：http://zar.ybcxt.top

[A21] 保留指定小数位输出
来源：http://lvp.fengsongda.top

Py:   f"{3.14159:.2f}"
来源：http://mka.yj20258888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jwn.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://qfl.gotoacloud.top

TS:   (3.14159).toFixed(2)
来源：http://jfb.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://ggy.chenlongwang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wfd.guannengcc.top

Ruby: format("%.2f", 3.14159)
来源：http://btj.havefunace.top

C#:   3.14159.ToString("F2")
来源：http://sbn.zdbjq.cn

[A22] 获取字符串长度
来源：http://xlv.ppjwa.cn

Py:   len(s)
来源：http://ylc.fanxiaobao.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://icf.cdnleiting.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sco.zhijiandao.cn

TS:   s.length
来源：http://lqf.shangyingyoupin.top

Java: s.length()
来源：http://mcg.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ggd.aibaodan.cn

Ruby: s.length
来源：http://dak.zycfv.cn

C#:   s.Length
来源：http://upn.guowangkeji.top

[A23] 大小写转换
来源：http://lzi.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://iyf.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cuy.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xoz.shuidangran.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wxy.jiagoushi.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://elu.jqgfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jdy.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zmf.fengsongda.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pad.smart0.xyz

[A24] 去除首尾空白
来源：http://xaz.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dtf.hcnkem.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://utk.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ojh.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qsu.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bki.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://xnn.guannengcc.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wyq.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://amg.bjfxy.top

[A25] 字符串比较
来源：http://cgf.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://ttu.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ycp.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pjg.gotoacloud.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sct.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ibf.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lsk.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://baz.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ghd.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://pak.shangyingyoupin.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qba.nwbrower.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lgt.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://anu.316326.xyz

TS:   Number() String() Boolean() x as number
来源：http://kkf.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lng.zhoulong.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://akg.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hil.svipenyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://alo.zdqjudy.top

================================================================================
来源：http://tir.zhongyouzk.top

B. 流程控制
来源：http://nvk.mhx1999.top

================================================================================
来源：http://rwy.cdnleiting.top

[B01] 条件判断 if / else
来源：http://soc.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://pyq.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qwa.vehdjk.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oun.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iba.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xao.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://juo.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ttf.hesvh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mqi.jyoumei.cn

[B02] 多分支 else if / elif
来源：http://qzt.52xcode.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nly.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mju.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://imm.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubn.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tup.sxryk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xvb.sweek.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dno.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahy.yj20258888.top

[B03] switch / match / case
来源：http://pob.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tfg.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jxd.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lwh.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mtd.sysykeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://shm.zycfv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hpt.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hgk.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://srb.gzhubu.top

[B04] for 计数循环
来源：http://oxn.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://nhj.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jpl.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://njy.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kft.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uzt.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://val.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://ujw.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://amc.havefunace.top

[B05] 遍历数组 / 列表
来源：http://ysc.zhiwuduotai.top

Py:   for item in arr: print(item)
来源：http://jvx.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rtl.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://grj.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://byc.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://xgs.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xho.wangshuangyany.cn

Ruby: arr.each { |item| puts item }
来源：http://uwc.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wpb.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://jau.yuanzhike.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xzd.andypj.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ffu.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hui.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ovh.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ovm.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dpf.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lwb.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pfe.snrcjt.cn

[B07] while 循环
来源：http://auh.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://xki.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ydr.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://csc.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://aof.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://xpl.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qfl.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://kit.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://efr.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://pbf.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://mia.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cdi.sxryk.cn

JS:   do { i++; } while (i < 10);
来源：http://jiv.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://ixu.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://qbd.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qve.chenjidiqi.icu

Ruby: begin; i += 1; end while i < 10
来源：http://eqj.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://lue.cdnleiting.top

[B09] break 与 continue
来源：http://pgg.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eti.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xjr.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qor.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsb.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxx.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kke.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gnr.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mpx.redwolf501.top

[B10] 遍历同时拿索引
来源：http://uof.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kvn.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hei.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://caw.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yya.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://icw.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hax.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fgb.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ouu.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://nzm.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://qol.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://neo.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vdl.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mrc.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iqb.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ime.zhiwuduotai.top

Ruby: (0...10).step(2).to_a
来源：http://mqc.yangfankeji.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lgy.cashguo.top

[B12] 跳出多层循环
来源：http://nlq.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bcy.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kce.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gti.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xmy.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://usa.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bme.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nek.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zkb.hcnkem.com

[B13] 判断是否为数字
来源：http://shi.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://crf.c1oappe.top

PHP:  is_numeric($x)
来源：http://top.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kzt.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mbr.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://hxv.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jog.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://qjj.yj20258888.top

C#:   x is int or double or decimal
来源：http://vsx.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://hlt.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qwm.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oah.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://yhx.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://pxb.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xts.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://isr.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ail.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vwt.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://gge.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://gbn.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://bov.daxiang520.top

JS:   a && b || !c
来源：http://wzy.gotoacloud.top

TS:   a && b || !c
来源：http://jwv.jinghuilouyu.cn

Java: a && b || !c
来源：http://hiq.wangshuangyany.cn

Go:   a && b || !c
来源：http://cdu.xinyue.icu

Ruby: a && b || !c
来源：http://moo.gogol.net.cn

C#:   a && b || !c
来源：http://bhz.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://eab.havefunace.top

Py:   if not data: return
来源：http://vuw.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://jlc.ydjk.org.cn

JS:   if (!data) return;
来源：http://xed.zhixingplan.top

TS:   if (!data) return;
来源：http://spc.gogol.net.cn

Java: if (data == null) return;
来源：http://sdd.yuanzhike.top

Go:   if data == nil { return }
来源：http://gss.daxiang520.top

Ruby: return if data.nil?
来源：http://nni.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://ijn.iojbl.cn

================================================================================
来源：http://jkh.gogol.net.cn

C. 函数与作用域
来源：http://lmx.shanyushiyangkeji.top

================================================================================
来源：http://dwq.tarul.cn

[C01] 定义函数
来源：http://rtd.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://dko.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://flb.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://aeg.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://otp.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zxf.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://eyn.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://wsq.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ffy.tarul.cn

[C02] 默认参数
来源：http://xdh.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://yig.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pqx.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://bpb.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pqg.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dbe.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://khh.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://udk.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://zin.iojbl.cn

[C03] 可变参数
来源：http://oaq.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://tri.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bhf.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ofk.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://psi.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oak.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ocz.sufxvd.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hyx.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dcn.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://wrz.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rnn.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vfb.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cim.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mcd.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://lag.uphjek.com


<!-- 参考信息 -->