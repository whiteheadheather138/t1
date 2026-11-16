代发 wailian999

Java: "第一行\n第二行"
来源：http://jba.hnqzz.top

Go:   "第一行\n第二行"
来源：http://quv.zdqjudy.top

Ruby: "第一行\n第二行"
来源：http://bpq.mhx1999.top

C#:   "第一行\n第二行"
来源：http://icj.sjlbkw.cn

[A14] 注释写法
来源：http://qrb.nwbrower.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://iuf.mhx1999.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dtk.hammf.cn

JS:   // 单行；/* 多行 */
来源：http://xuo.yfazqb.com

TS:   // 单行；/* 多行 */
来源：http://swx.sufxvd.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aeh.c1oappe.top

Go:   // 单行；/* 多行 */
来源：http://oqb.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://jfe.wangdashe.top

C#:   // 单行；/* 多行 */
来源：http://aau.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://rcu.zhijiandao.cn

Py:   value = data or "默认值"
来源：http://woo.hammf.cn

PHP:  $value = $data ?? "默认值";
来源：http://pdb.sjlbkw.cn

JS:   const value = data ?? "默认值";
来源：http://fpi.ivvv.top

TS:   const value = data ?? "默认值";
来源：http://nkz.gotoacloud.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qpf.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://wdo.wangdashe.top

Ruby: value = data || "默认值"
来源：http://wkr.bbcook.cn

C#:   var value = data ?? "默认值";
来源：http://qah.0kj1m.cn

[A16] 真假值判断规则
来源：http://xwv.jianghu66.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://omi.dashuyun.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kvo.andypj.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ekd.yj20258888.top

TS:   if (!x) {}
来源：http://eyp.hongshengwenyu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pdo.daria6918.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://otr.meibo888.top

Ruby: unless x            # nil 与 false 为假
来源：http://kez.zhengqikj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jkw.ydzc1.top

[A17] 位运算
来源：http://teb.gogol.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gtr.hywenlv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lim.fengsongda.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rcf.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qrn.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zhj.zhaomingkeji.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hqv.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lim.sweek.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ifs.aizwys.cn

[A18] 字符与 ASCII 码互转
来源：http://eul.tanke756.top

Py:   ord("A"); chr(65)
来源：http://gje.kuanghao11.cn

PHP:  ord("A"); chr(65)
来源：http://spw.fzhhl.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://law.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gaa.kuanghao11.cn

Java: (int) 'A'; (char) 65
来源：http://yrj.fktsv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fml.c1oappe.top

Ruby: "A".ord; 65.chr
来源：http://rmk.c1oappe.top

C#:   (int)'A'; (char)65
来源：http://rch.xylfe.cn

[A19] 交换两个变量
来源：http://vfe.dianchejie.cn

Py:   a, b = b, a
来源：http://kja.gaohongyu789.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dow.zhongyouzk.top

JS:   [a, b] = [b, a];
来源：http://fqm.zdbjq.cn

TS:   [a, b] = [b, a];
来源：http://ekf.yangfankeji.com

Java: int t = a; a = b; b = t;
来源：http://nxj.andypj.xyz

Go:   a, b = b, a
来源：http://yfr.zdqjudy.top

Ruby: a, b = b, a
来源：http://zge.daxiang520.top

C#:   (a, b) = (b, a);
来源：http://axj.zdbjq.cn

[A20] 读取标准输入
来源：http://uyv.bjfxy.top

Py:   name = input("请输入：")
来源：http://lgh.sufxvd.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mzo.jinqigufen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kre.fehbvm.com

TS:   // Node.js：readline 模块
来源：http://bnl.uphjek.com

Java: new Scanner(System.in).nextLine()
来源：http://ros.316326.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pby.sysykeji.top

Ruby: gets.chomp
来源：http://jnk.fktsv.cn

C#:   Console.ReadLine();
来源：http://hil.sufxvd.cn

[A21] 保留指定小数位输出
来源：http://chk.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://ayx.xingfuxueyuan.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oxe.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://cjj.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://glb.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://ksz.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nhs.gogol.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://xpa.sweek.top

C#:   3.14159.ToString("F2")
来源：http://ndo.yj202588.top

[A22] 获取字符串长度
来源：http://oxk.guowangkeji.top

Py:   len(s)
来源：http://pla.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zrr.xinyue.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://olv.ydjk.org.cn

TS:   s.length
来源：http://kcl.yj20258888.top

Java: s.length()
来源：http://wvp.hongshengwenyu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ose.hywenlv.cn

Ruby: s.length
来源：http://mdc.ywan-chungtsiang.top

C#:   s.Length
来源：http://buh.yfazqb.com

[A23] 大小写转换
来源：http://sgp.shanyushiyangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gvb.hysaishi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qso.zhoulong.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vyl.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bha.xingfuxueyuan.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://caf.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bmg.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rbe.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://diz.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://lco.wangdashe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://laf.jiagoushi.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sqo.hcnkem.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zjq.bjfxy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rke.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ecd.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://ivk.cheryme.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sph.snrcjt.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wnk.0kj1m.cn

[A25] 字符串比较
来源：http://ics.iojbl.cn

Py:   s1 == s2; s1 != s2
来源：http://nay.snrcjt.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://udb.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qei.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rsd.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ckg.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rag.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pyd.xuetiantiany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lsr.fengsongda.top

[A26] 类型转换总览
来源：http://gvt.pycfn.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://prr.ydjk.org.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oij.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hvw.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://xgk.fktsv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xmv.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lug.316326.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://tmw.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pgy.daxiang520.top

================================================================================
来源：http://svu.tanke756.top

B. 流程控制
来源：http://owg.gzhubu.top

================================================================================
来源：http://jep.snrcjt.cn

[B01] 条件判断 if / else
来源：http://osr.ctjpmb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://vxy.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iee.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uqe.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qsb.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://chs.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ciz.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nhi.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ewe.hammf.cn

[B02] 多分支 else if / elif
来源：http://vtl.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vli.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://upr.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gqs.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ksr.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chn.yj20258.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dnf.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iye.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://igm.hnxiangtu.top

[B03] switch / match / case
来源：http://ynj.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nsv.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jhz.daria6918.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nqj.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fgg.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://trl.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mek.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lmp.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qwa.jqgfzy.top

[B04] for 计数循环
来源：http://mpr.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://twk.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vam.yj20258.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tpz.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hij.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rcd.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pgo.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://jsc.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vyu.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://nvk.hnqzz.top

Py:   for item in arr: print(item)
来源：http://ncy.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ziu.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kwn.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://qcq.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://phh.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fdz.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://qqb.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mcn.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://unc.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ulj.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ghv.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rqa.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aqi.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wcc.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rnm.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qzs.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cfa.jyoumei.cn

[B07] while 循环
来源：http://ydb.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://jri.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://ium.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://wmh.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://iud.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://ufk.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gdi.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://ern.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://wau.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://maa.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://izt.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://saa.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://hqx.sufxvd.cn

TS:   do { i++; } while (i < 10);
来源：http://oyo.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://ezu.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pxj.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://pud.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://doi.yangfankeji.com

[B09] break 与 continue
来源：http://ltg.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://abz.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cib.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bpu.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://isq.guowangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://skt.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ees.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pzq.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwz.xinyue.icu

[B10] 遍历同时拿索引
来源：http://rgx.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jwg.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kby.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pvd.sweek.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lqe.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://who.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kmq.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pyu.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nqn.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://xur.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://idk.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://zkl.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lqb.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgj.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xus.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ufi.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://odi.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cmf.ctjpmb.com

[B12] 跳出多层循环
来源：http://oip.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://spx.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://hzm.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://abq.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvx.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://svy.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cbx.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://meu.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://urv.yongpay.top

[B13] 判断是否为数字
来源：http://wel.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://jpb.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://npo.nanxuanxn.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lkh.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kfl.epnwcf.com

Java: x instanceof Number
来源：http://svb.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bqr.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://vvh.daxiang520.top

C#:   x is int or double or decimal
来源：http://zpj.yj20258888.top

[B14] 判断值是否在集合内
来源：http://bhe.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cdc.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xit.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ucg.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://him.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jhc.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jar.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ite.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rvt.yangfankeji.com

[B15] 布尔运算与取反
来源：http://xih.svipenyu.cn

Py:   a and b or not c
来源：http://bzr.hesvh.cn

PHP:  $a && $b || !$c
来源：http://llc.guowangkeji.top

JS:   a && b || !c
来源：http://hji.aibaodan.cn

TS:   a && b || !c
来源：http://tvo.pengpengdd.cyou

Java: a && b || !c
来源：http://eel.tianlin.xyz

Go:   a && b || !c
来源：http://iud.cucudq.cn

Ruby: a && b || !c
来源：http://ndj.hammf.cn

C#:   a && b || !c
来源：http://gxa.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vqk.yonumen.top

Py:   if not data: return
来源：http://dab.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://uxa.shangyingyoupin.top

JS:   if (!data) return;
来源：http://umd.epnwcf.com

TS:   if (!data) return;
来源：http://jnl.bbcook.cn

Java: if (data == null) return;
来源：http://pkr.ydzc1.top

Go:   if data == nil { return }
来源：http://pqs.zdbjq.cn

Ruby: return if data.nil?
来源：http://jxq.bbcook.cn

C#:   if (data == null) return;
来源：http://bbz.gogol.net.cn

================================================================================
来源：http://wyv.guannengcc.top

C. 函数与作用域
来源：http://dlz.nanxuanxn.top

================================================================================
来源：http://uks.vqdsnc.cn

[C01] 定义函数
来源：http://sea.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://sjq.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixj.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://jtg.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ckx.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://gdy.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dvj.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://irl.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qni.dashuyun.cn

[C02] 默认参数
来源：http://dug.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://izo.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://niq.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://lrx.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rnu.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qek.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hpj.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://zgt.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://owr.jinqigufen.top

[C03] 可变参数
来源：http://bip.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://otg.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gwr.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qrr.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ihe.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dqa.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://foj.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://zeb.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qgt.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://gca.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mlm.ywan-chungtsiang.top


<!-- 参考信息 -->