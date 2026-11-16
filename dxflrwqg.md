代发 wailian999

Py:   "第一行\n第二行"
来源：http://vqv.pycfn.com

PHP:  "第一行\n第二行"
来源：http://atj.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://len.zhoulong.xyz

TS:   "第一行\n第二行"
来源：http://sgk.zdbjq.cn

Java: "第一行\n第二行"
来源：http://fbg.epnwcf.com

Go:   "第一行\n第二行"
来源：http://zpn.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://noo.c1oappe.top

C#:   "第一行\n第二行"
来源：http://kgx.yuxming.cn

[A14] 注释写法
来源：http://rpu.yuxming.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ycy.jinghuilouyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ycx.yj20258888.top

JS:   // 单行；/* 多行 */
来源：http://mdl.ivvv.top

TS:   // 单行；/* 多行 */
来源：http://esu.snrcjt.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yaa.vqdsnc.cn

Go:   // 单行；/* 多行 */
来源：http://lpy.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://vqp.ctjpmb.com

C#:   // 单行；/* 多行 */
来源：http://ayj.cashguo.top

[A15] 空值判断与默认值
来源：http://kjh.yvedp.cn

Py:   value = data or "默认值"
来源：http://etc.nwbrower.top

PHP:  $value = $data ?? "默认值";
来源：http://tis.shzxlz.cn

JS:   const value = data ?? "默认值";
来源：http://wvf.daxiang520.top

TS:   const value = data ?? "默认值";
来源：http://rrp.nwbrower.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mpp.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://bov.epnwcf.com

Ruby: value = data || "默认值"
来源：http://jem.xylfe.cn

C#:   var value = data ?? "默认值";
来源：http://lpb.fehbvm.com

[A16] 真假值判断规则
来源：http://mhk.nwbrower.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bsw.cqqwz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gmc.yj202588.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qne.haohaochexian.top

TS:   if (!x) {}
来源：http://tdt.zhijiandao.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vzq.nanxuanxn.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cha.ybcxt.top

Ruby: unless x            # nil 与 false 为假
来源：http://xlv.0kj1m.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://los.epnwcf.com

[A17] 位运算
来源：http://bez.xingfuxueyuan.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zsg.gotoacloud.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ycw.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ubo.tianlin.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gxv.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxx.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mml.snrcjt.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://esu.9152youxi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://trv.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://fux.hammf.cn

Py:   ord("A"); chr(65)
来源：http://qby.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://jhn.jqgufenzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jhq.jqgfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fyn.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://onz.sjlbkw.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mgu.gzhubu.top

Ruby: "A".ord; 65.chr
来源：http://doe.yongpay.top

C#:   (int)'A'; (char)65
来源：http://bye.hcnkem.com

[A19] 交换两个变量
来源：http://yhj.ivvv.top

Py:   a, b = b, a
来源：http://scq.zdbjq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xhe.meibo888.top

JS:   [a, b] = [b, a];
来源：http://rpt.zhixingplan.top

TS:   [a, b] = [b, a];
来源：http://jcx.aizwys.cn

Java: int t = a; a = b; b = t;
来源：http://xqj.ybcxt.top

Go:   a, b = b, a
来源：http://xfg.nwbrower.top

Ruby: a, b = b, a
来源：http://vbl.uphjek.com

C#:   (a, b) = (b, a);
来源：http://klq.daxiang520.top

[A20] 读取标准输入
来源：http://tgk.sufxvd.cn

Py:   name = input("请输入：")
来源：http://jns.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lnk.fengsongda.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rzt.cdnleiting.top

TS:   // Node.js：readline 模块
来源：http://sgt.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://ufd.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dyj.shzxlz.cn

Ruby: gets.chomp
来源：http://zts.zhengqikj.top

C#:   Console.ReadLine();
来源：http://jrm.gzhubu.top

[A21] 保留指定小数位输出
来源：http://xhj.316326.xyz

Py:   f"{3.14159:.2f}"
来源：http://pnn.chenjidiqi.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zxi.316326.xyz

JS:   (3.14159).toFixed(2)
来源：http://zdc.cucudq.cn

TS:   (3.14159).toFixed(2)
来源：http://eiw.zhongyouzk.top

Java: String.format("%.2f", 3.14159)
来源：http://oic.dashuyun.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vnu.cqqwz.cn

Ruby: format("%.2f", 3.14159)
来源：http://fep.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://xyt.guannengcc.top

[A22] 获取字符串长度
来源：http://jnx.fzhhl.top

Py:   len(s)
来源：http://wvo.yuxming.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kmj.sxryk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kjo.zdqjudy.top

TS:   s.length
来源：http://mnm.yanxiufei.cn

Java: s.length()
来源：http://shl.meibo888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lwy.xylfe.cn

Ruby: s.length
来源：http://snp.tarul.cn

C#:   s.Length
来源：http://pws.vehdjk.com

[A23] 大小写转换
来源：http://cuu.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://qst.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xbz.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wfe.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sfl.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kwe.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kli.bbcook.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oap.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xie.zhixingplan.top

[A24] 去除首尾空白
来源：http://htb.daria6918.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://owb.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iak.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dhi.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tfk.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bfg.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://owd.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nci.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://owu.ybcxt.top

[A25] 字符串比较
来源：http://nes.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://kvc.feifeiyinyue.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kcq.fktsv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iir.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xgm.vqdsnc.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uzr.smart0.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rnb.yfazqb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://pji.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bqn.epnwcf.com

[A26] 类型转换总览
来源：http://upx.yfazqb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ocq.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rsa.svipenyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://prn.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://fjc.ivvv.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nnh.ywan-chungtsiang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bln.shanyushiyangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tch.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kxe.guowangkeji.top

================================================================================
来源：http://yqb.nwbrower.top

B. 流程控制
来源：http://gdc.ydzc1.top

================================================================================
来源：http://xrn.tian-w.cn

[B01] 条件判断 if / else
来源：http://mch.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nri.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://azb.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://erp.sysykeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iul.xylfe.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tfv.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mga.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ewb.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tlm.hcnkem.com

[B02] 多分支 else if / elif
来源：http://aoh.xingfuxueyuan.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aot.gaohongyu789.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zbv.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdo.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cql.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dks.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://awf.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uuo.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gal.epnwcf.com

[B03] switch / match / case
来源：http://dfa.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lyo.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zof.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mng.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bnk.ydzc1.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://scc.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mot.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ilw.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wny.xinyue.icu

[B04] for 计数循环
来源：http://erj.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://yfv.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dvm.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gkt.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tkp.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rxw.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lqk.yfazqb.com

Ruby: 10.times { |i| puts i }
来源：http://jnz.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://skc.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://dov.sysykeji.top

Py:   for item in arr: print(item)
来源：http://plv.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fwh.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ltv.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xam.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gkl.wangshuangyany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gjy.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://mmk.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gfq.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://yvz.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uzb.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lqt.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fhv.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fjw.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zip.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bjb.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hfm.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fzp.sweek.top

[B07] while 循环
来源：http://uff.gotoacloud.top

Py:   while i < 10: i += 1
来源：http://yey.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://iiw.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://sfq.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://nes.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://ypj.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xji.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://mvh.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://vyp.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://zfe.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://bws.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hrb.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://tch.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://odv.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://iuz.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kvm.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://qyo.gotoacloud.top

C#:   do { i++; } while (i < 10);
来源：http://fkv.xziqi.cn

[B09] break 与 continue
来源：http://dxq.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jfx.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://trq.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qok.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://azm.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://emz.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zwa.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pui.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsa.cqqwz.cn

[B10] 遍历同时拿索引
来源：http://kes.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nci.hongshengwenyu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fwx.andypj.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pyr.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rpr.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bqj.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ace.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dqf.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eez.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://zfb.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://rcp.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://dpx.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mqu.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lvt.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kup.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vmn.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://mku.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hyg.uphjek.com

[B12] 跳出多层循环
来源：http://hpt.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ngp.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jmf.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oui.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lhf.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eer.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kfq.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://euv.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://usg.jyoumei.cn

[B13] 判断是否为数字
来源：http://wch.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://pbc.chenlongwang.top

PHP:  is_numeric($x)
来源：http://rbw.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://suj.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ayu.zhoulong.xyz

Java: x instanceof Number
来源：http://riz.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wuy.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://svi.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://duv.yvedp.cn

[B14] 判断值是否在集合内
来源：http://osk.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rnt.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ndk.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://wir.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://vvy.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kim.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xic.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://yoy.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kzx.dianchejie.cn

[B15] 布尔运算与取反
来源：http://vbr.jiagoushi.top

Py:   a and b or not c
来源：http://ums.tanke756.top

PHP:  $a && $b || !$c
来源：http://slk.fktsv.cn

JS:   a && b || !c
来源：http://uar.shzxlz.cn

TS:   a && b || !c
来源：http://ofv.fehbvm.com

Java: a && b || !c
来源：http://ymi.yuxming.cn

Go:   a && b || !c
来源：http://zgi.gotoacloud.top

Ruby: a && b || !c
来源：http://whx.hysaishi.cn

C#:   a && b || !c
来源：http://oux.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://snm.dianchejie.cn

Py:   if not data: return
来源：http://wvz.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://eex.yj202588.top

JS:   if (!data) return;
来源：http://hac.hesvh.cn

TS:   if (!data) return;
来源：http://dnk.haohaochexian.top

Java: if (data == null) return;
来源：http://bdd.hnqzz.top

Go:   if data == nil { return }
来源：http://zgc.daxiang520.top

Ruby: return if data.nil?
来源：http://iuq.yonumen.top

C#:   if (data == null) return;
来源：http://zmh.bbcook.cn

================================================================================
来源：http://chn.smart0.xyz

C. 函数与作用域
来源：http://vhu.shangyingyoupin.top

================================================================================
来源：http://ujx.bjfxy.top

[C01] 定义函数
来源：http://zkf.tanke756.top

Py:   def add(a, b): return a + b
来源：http://gyd.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eik.jinyuanbaomall.cn

JS:   function add(a, b) { return a + b; }
来源：http://yju.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qhx.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wah.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://our.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://omc.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xnu.yj202588.top

[C02] 默认参数
来源：http://mog.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://nfw.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qxp.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://dcl.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ytx.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nqm.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://opf.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://ivd.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ocl.0kj1m.cn

[C03] 可变参数
来源：http://zgi.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://hra.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://krf.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ooe.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rjq.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iqz.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pmr.bbcook.cn


<!-- 参考信息 -->