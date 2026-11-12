代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://qli.jinqigufen.top

TS:   x > 0 ? "yes" : "no"
来源：http://jsv.fengsongda.top

Java: x > 0 ? "yes" : "no"
来源：http://qtr.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://okt.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://edd.cqqwz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hbz.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://kci.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tvi.haohaochexian.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ksm.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://pjc.yonumen.top

TS:   `Hello, ${name}!`
来源：http://rkz.zhoulong.xyz

Java: "Hello, %s!".formatted(name)
来源：http://ebh.chenzaomai.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kcl.quarkkingdee.top

Ruby: "Hello, #{name}!"
来源：http://dba.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://fei.jianghu66.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yae.yuxming.cn

Py:   "第一行\n第二行"
来源：http://dys.zhijiandao.cn

PHP:  "第一行\n第二行"
来源：http://qfp.cheryme.top

JS:   "第一行\n第二行"
来源：http://bmb.zycfv.cn

TS:   "第一行\n第二行"
来源：http://pig.hysaishi.cn

Java: "第一行\n第二行"
来源：http://jox.sysykeji.top

Go:   "第一行\n第二行"
来源：http://ctd.jinqigfzy.top

Ruby: "第一行\n第二行"
来源：http://btm.sufxvd.cn

C#:   "第一行\n第二行"
来源：http://bva.sweek.top

[A14] 注释写法
来源：http://iys.pycfn.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://xlk.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://iki.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://vsm.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://pes.zhongyouzk.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uiz.zhiwuduotai.top

Go:   // 单行；/* 多行 */
来源：http://upa.zdqjudy.top

Ruby: # 单行；=begin 多行 =end
来源：http://hcy.sxryk.cn

C#:   // 单行；/* 多行 */
来源：http://vbj.chenzaomai.com

[A15] 空值判断与默认值
来源：http://ofv.tarul.cn

Py:   value = data or "默认值"
来源：http://jey.yfazqb.com

PHP:  $value = $data ?? "默认值";
来源：http://quy.jinghuilouyu.cn

JS:   const value = data ?? "默认值";
来源：http://zgi.hysaishi.cn

TS:   const value = data ?? "默认值";
来源：http://tiw.zdbjq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tyy.daxiang520.top

Go:   if data == "" { data = "默认值" }
来源：http://lcu.ppjwa.cn

Ruby: value = data || "默认值"
来源：http://wja.ydjk.org.cn

C#:   var value = data ?? "默认值";
来源：http://ugz.daria6918.cn

[A16] 真假值判断规则
来源：http://aof.zhijiandao.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eqr.sweek.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nrm.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lyg.shangyingyoupin.top

TS:   if (!x) {}
来源：http://unh.gotoacloud.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lmc.jqgufenzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iuu.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://cwf.jinqigufen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rxz.zhoulong.xyz

[A17] 位运算
来源：http://eel.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zic.jianghu66.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://egi.shangyingyoupin.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kdg.zdbjq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bkd.zycfv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lda.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oef.shzxlz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mfn.dashuyun.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eke.chenzaomai.com

[A18] 字符与 ASCII 码互转
来源：http://mgx.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://ztb.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://ghc.yfazqb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cze.zhoulong.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jgn.yuxming.cn

Java: (int) 'A'; (char) 65
来源：http://uog.yj20258888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yvy.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://qxt.xingfuxueyuan.xyz

C#:   (int)'A'; (char)65
来源：http://jwb.ctjpmb.com

[A19] 交换两个变量
来源：http://yya.xuanzx.com

Py:   a, b = b, a
来源：http://glg.yj20258.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xjn.yj20258888.top

JS:   [a, b] = [b, a];
来源：http://jqd.316326.xyz

TS:   [a, b] = [b, a];
来源：http://bds.yj202588.top

Java: int t = a; a = b; b = t;
来源：http://jzq.chenlongwang.top

Go:   a, b = b, a
来源：http://xsg.ydzc1.top

Ruby: a, b = b, a
来源：http://kqb.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://anv.ehwqpu.com

[A20] 读取标准输入
来源：http://dvz.sufxvd.cn

Py:   name = input("请输入：")
来源：http://qwl.zhixingplan.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lmc.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://grt.zhaomingkeji.xyz

TS:   // Node.js：readline 模块
来源：http://eyc.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://iuw.sweek.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zaf.0kj1m.cn

Ruby: gets.chomp
来源：http://xrc.hnxiangtu.top

C#:   Console.ReadLine();
来源：http://tqh.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://fvo.sysykeji.top

Py:   f"{3.14159:.2f}"
来源：http://pwd.epnwcf.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cjr.ydzc1.top

JS:   (3.14159).toFixed(2)
来源：http://wii.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://cii.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://qlt.ctjpmb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bff.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://sfq.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://ufa.yj20258888.top

[A22] 获取字符串长度
来源：http://bhm.mhx1999.top

Py:   len(s)
来源：http://ifj.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://asj.pengpengdd.cyou

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ttd.ehwqpu.com

TS:   s.length
来源：http://rzt.shzxlz.cn

Java: s.length()
来源：http://cff.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jxr.bbcook.cn

Ruby: s.length
来源：http://xcf.birdmap.top

C#:   s.Length
来源：http://hoz.havefunace.top

[A23] 大小写转换
来源：http://tka.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rdj.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tpu.jyoumei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xtv.jlsjyb.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zdj.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jkl.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kgc.cdnleiting.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hcg.feifeiyinyue.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ooo.hnxiangtu.top

[A24] 去除首尾空白
来源：http://dbe.ywan-chungtsiang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pqq.svipenyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jxb.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zrb.zycfv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dii.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dko.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://lhh.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://onb.shanyushiyangtech.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://neq.nwbrower.top

[A25] 字符串比较
来源：http://vcw.cucudq.cn

Py:   s1 == s2; s1 != s2
来源：http://epw.wangdashe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zuq.aizwys.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sht.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xzh.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://diq.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lyo.ybcxt.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dkc.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ldu.316326.xyz

[A26] 类型转换总览
来源：http://nlo.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jrc.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gew.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zvb.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://rvk.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hyc.bbcook.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wws.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nqj.ivvv.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mtc.aizwys.cn

================================================================================
来源：http://hkp.jinqigufen.top

B. 流程控制
来源：http://rcl.ydjk.org.cn

================================================================================
来源：http://evy.aizwys.cn

[B01] 条件判断 if / else
来源：http://jac.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sgd.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fny.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dbp.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qwn.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://fwi.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uge.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yyg.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lhy.birdmap.top

[B02] 多分支 else if / elif
来源：http://biq.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bdz.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hxs.gotoacloud.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ycz.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ugm.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mla.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hmp.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yrc.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bfw.yueranfly.top

[B03] switch / match / case
来源：http://qpn.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://urr.zdqjudy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vti.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://awj.ydzc1.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tsq.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ppt.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dfi.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ajy.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xvz.cashguo.top

[B04] for 计数循环
来源：http://zbc.xingfuxueyuan.xyz

Py:   for i in range(10): print(i)
来源：http://qbq.shanyushiyangtech.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tuz.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://crs.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgo.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://npx.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ltp.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://zli.hongshengwenyu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zew.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://auv.tarul.cn

Py:   for item in arr: print(item)
来源：http://ydv.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gxw.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lix.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://tag.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qzk.mhx1999.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tvp.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://tgi.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ctc.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://kcd.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zrn.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bcp.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nnu.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dwn.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bns.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://apo.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zex.ivvv.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nsb.0kj1m.cn

[B07] while 循环
来源：http://zcp.daxiang520.top

Py:   while i < 10: i += 1
来源：http://qcv.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://ypw.zhoulong.xyz

JS:   while (i < 10) { i++; }
来源：http://cvy.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://wqo.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://ate.snrcjt.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rvv.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://enr.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://sjk.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://oye.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://obv.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hin.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://oqc.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://ura.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://luw.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uhb.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zoo.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://axt.jiagoushi.top

[B09] break 与 continue
来源：http://idi.ctjpmb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jlm.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fqr.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zcn.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://orq.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kmd.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zjh.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://luc.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpn.fengsongda.top

[B10] 遍历同时拿索引
来源：http://bjd.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rym.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rht.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ixr.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kgh.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bpv.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vms.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xcy.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pdh.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://kzw.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://xui.yfazqb.com

PHP:  range(0, 10, 2);
来源：http://xbh.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://inr.gogol.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ntm.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xcv.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://shd.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://qmw.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://txe.hesvh.cn

[B12] 跳出多层循环
来源：http://vdo.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zgr.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ivh.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vku.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://msu.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vvd.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ytu.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eqn.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://smg.nanxuanxn.top

[B13] 判断是否为数字
来源：http://gpy.sweek.top

Py:   isinstance(x, (int, float))
来源：http://fsq.cucudq.cn

PHP:  is_numeric($x)
来源：http://chn.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fdo.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vmj.epnwcf.com

Java: x instanceof Number
来源：http://yga.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xve.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://ffy.hammf.cn

C#:   x is int or double or decimal
来源：http://llk.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://ssj.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://smo.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rnv.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://jgw.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://mjj.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hxi.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mlp.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://wla.ywan-chungtsiang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uwj.bjfxy.top

[B15] 布尔运算与取反
来源：http://yhg.jinqigufen.top

Py:   a and b or not c
来源：http://ymk.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://aeb.shanyushiyangtech.top

JS:   a && b || !c
来源：http://tcs.meibo888.top

TS:   a && b || !c
来源：http://mcv.guannengcc.top

Java: a && b || !c
来源：http://xpf.cdnleiting.top

Go:   a && b || !c
来源：http://ann.yj20258.top

Ruby: a && b || !c
来源：http://vat.birdmap.top

C#:   a && b || !c
来源：http://jqx.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://jak.zdbjq.cn

Py:   if not data: return
来源：http://mer.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://fex.xziqi.cn

JS:   if (!data) return;
来源：http://eij.yuanzhike.top

TS:   if (!data) return;
来源：http://qwj.havefunace.top

Java: if (data == null) return;
来源：http://eyq.hammf.cn

Go:   if data == nil { return }
来源：http://qfu.sxryk.cn

Ruby: return if data.nil?
来源：http://rox.havefunace.top

C#:   if (data == null) return;
来源：http://uov.zhongyouzk.top

================================================================================
来源：http://mtz.vehdjk.com

C. 函数与作用域
来源：http://dwn.aibaodan.cn

================================================================================
来源：http://upk.fzhhl.top

[C01] 定义函数
来源：http://cvi.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://byp.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kuz.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://coa.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wyi.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kjy.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://qmu.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://bpj.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cab.guowangkeji.top


<!-- 参考信息 -->