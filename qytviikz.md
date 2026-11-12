代发 wailian999

Py:   "第一行\n第二行"
来源：http://txk.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://uoe.fengsongda.top

JS:   "第一行\n第二行"
来源：http://ied.guowangkeji.top

TS:   "第一行\n第二行"
来源：http://lvk.zhoulong.xyz

Java: "第一行\n第二行"
来源：http://pje.gotoacloud.top

Go:   "第一行\n第二行"
来源：http://slo.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://yqi.316326.xyz

C#:   "第一行\n第二行"
来源：http://ibz.jinghuilouyu.cn

[A14] 注释写法
来源：http://cks.gaohongyu789.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://chl.shuidangran.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gtz.tianlin.xyz

JS:   // 单行；/* 多行 */
来源：http://yyw.haohaochexian.top

TS:   // 单行；/* 多行 */
来源：http://piu.guannengcc.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rqc.9152youxi.cn

Go:   // 单行；/* 多行 */
来源：http://mpb.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gtw.zhixingplan.top

C#:   // 单行；/* 多行 */
来源：http://rpx.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://twx.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://fbv.zhoulong.xyz

PHP:  $value = $data ?? "默认值";
来源：http://qsw.feifeiyinyue.top

JS:   const value = data ?? "默认值";
来源：http://cxu.iojbl.cn

TS:   const value = data ?? "默认值";
来源：http://kfl.meibo888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ijj.sysykeji.top

Go:   if data == "" { data = "默认值" }
来源：http://pdn.zhaomingkeji.xyz

Ruby: value = data || "默认值"
来源：http://ril.zdbjq.cn

C#:   var value = data ?? "默认值";
来源：http://tvu.pycfn.com

[A16] 真假值判断规则
来源：http://tdh.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://aza.yangfankeji.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rxx.hfpthk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cwr.yvedp.cn

TS:   if (!x) {}
来源：http://xoz.uphjek.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jnk.c1oappe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ufp.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://aon.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bwk.sufxvd.cn

[A17] 位运算
来源：http://tdu.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cih.fanxiaobao.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ijj.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mtd.shzxlz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yat.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrx.meibo888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bik.xuanzx.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ngw.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ner.yueranfly.top

[A18] 字符与 ASCII 码互转
来源：http://xac.zhaomingkeji.xyz

Py:   ord("A"); chr(65)
来源：http://tij.chenlongwang.top

PHP:  ord("A"); chr(65)
来源：http://ruz.zdbjq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sbr.fengsongda.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tub.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://tjh.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://trf.kuanghao11.cn

Ruby: "A".ord; 65.chr
来源：http://tqo.316326.xyz

C#:   (int)'A'; (char)65
来源：http://vks.ydjk.org.cn

[A19] 交换两个变量
来源：http://osl.yongpay.top

Py:   a, b = b, a
来源：http://gpb.dashuyun.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zjj.dashuyun.cn

JS:   [a, b] = [b, a];
来源：http://grk.shzxlz.cn

TS:   [a, b] = [b, a];
来源：http://pcj.nwbrower.top

Java: int t = a; a = b; b = t;
来源：http://xbx.wangshuangyany.cn

Go:   a, b = b, a
来源：http://weg.pengpengdd.cyou

Ruby: a, b = b, a
来源：http://spq.52xcode.cn

C#:   (a, b) = (b, a);
来源：http://aii.hesvh.cn

[A20] 读取标准输入
来源：http://wrj.hnxiangtu.top

Py:   name = input("请输入：")
来源：http://dxh.mhx1999.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fqv.shanyushiyangtech.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dnx.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://iki.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://zch.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wxj.sxryk.cn

Ruby: gets.chomp
来源：http://agf.tarul.cn

C#:   Console.ReadLine();
来源：http://xzg.chenlongwang.top

[A21] 保留指定小数位输出
来源：http://kyo.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://ocp.hongshengwenyu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dpy.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://yrw.haohaochexian.top

TS:   (3.14159).toFixed(2)
来源：http://huo.jlsjyb.cn

Java: String.format("%.2f", 3.14159)
来源：http://oxf.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vef.zhoulong.xyz

Ruby: format("%.2f", 3.14159)
来源：http://mbv.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://kke.hcnkem.com

[A22] 获取字符串长度
来源：http://bba.bbcook.cn

Py:   len(s)
来源：http://lnr.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gus.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jno.tianlin.xyz

TS:   s.length
来源：http://kbv.ydjk.org.cn

Java: s.length()
来源：http://kku.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mia.tanke756.top

Ruby: s.length
来源：http://jnm.yueranfly.top

C#:   s.Length
来源：http://jbb.shangyingyoupin.top

[A23] 大小写转换
来源：http://kya.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qqv.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qyz.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dns.gotoacloud.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qnh.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pgw.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://okq.yangfankeji.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bub.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pza.yanxiufei.cn

[A24] 去除首尾空白
来源：http://mfv.iojbl.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ywf.ywan-chungtsiang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hsz.chenzaomai.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sbn.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dgv.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://awv.hammf.cn

Go:   strings.TrimSpace(s)
来源：http://cgs.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://atr.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jgq.zhixingplan.top

[A25] 字符串比较
来源：http://tml.fzhhl.top

Py:   s1 == s2; s1 != s2
来源：http://vrt.haohaochexian.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dsj.ydjk.org.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cfq.xziqi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://crx.wangshuangyany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://krc.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gik.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://cgr.yongpay.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gmq.vqdsnc.cn

[A26] 类型转换总览
来源：http://gfp.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://paf.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jcj.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dfm.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://cfm.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dtp.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yad.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://plx.fehbvm.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://neu.kuanghao11.cn

================================================================================
来源：http://wmh.ydjk.org.cn

B. 流程控制
来源：http://gny.shangyingyoupin.top

================================================================================
来源：http://gwi.yj20258.top

[B01] 条件判断 if / else
来源：http://tec.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pzr.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zhi.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qaj.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qzn.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://izp.yuxming.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://agr.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nvh.hammf.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://egv.yj20258.top

[B02] 多分支 else if / elif
来源：http://jor.xingfuxueyuan.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://shj.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fti.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qqj.jqgfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ajo.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ntk.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bjr.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bvm.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ejr.chenlongwang.top

[B03] switch / match / case
来源：http://nbx.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ycw.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ypi.daria6918.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oct.cucudq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kaz.ybcxt.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yrh.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mtn.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ogu.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yhb.tanke756.top

[B04] for 计数循环
来源：http://qdj.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://qjp.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://etk.bbcook.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://njh.yj20258888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yoq.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ual.vqdsnc.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tqa.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://rzd.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rjl.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://twr.wangshuangyany.cn

Py:   for item in arr: print(item)
来源：http://amx.tanke756.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xxn.smart0.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://yhl.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jig.yj20258.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mss.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hxl.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://bbo.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mwl.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://jhz.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://btt.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qij.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gmd.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rlk.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://brr.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://afo.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mst.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sfz.wangdashe.top

[B07] while 循环
来源：http://hvs.chenjidiqi.icu

Py:   while i < 10: i += 1
来源：http://sef.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://jaz.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://dms.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://ofj.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://rxs.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blp.quarkkingdee.top

Ruby: while i < 10; i += 1; end
来源：http://zqz.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://dog.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://opx.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://vmo.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pnl.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://aaf.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://bst.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://rdd.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://czw.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://isd.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://bln.fzhhl.top

[B09] break 与 continue
来源：http://qdp.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gvx.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tob.bbcook.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://peb.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cov.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ieq.cucudq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gip.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rhg.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bjz.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://nag.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://odu.yj202588.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://juk.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zow.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dbk.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bxe.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fmo.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ycb.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wip.gogol.net.cn

[B11] 生成数字序列 / 区间
来源：http://lgs.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://hhl.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://ybq.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xti.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gmu.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uzq.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aci.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://rtw.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xek.feifeiyinyue.top

[B12] 跳出多层循环
来源：http://fgk.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://qvn.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zkt.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dik.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iwt.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hgw.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kft.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ejh.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oic.yj20258888.top

[B13] 判断是否为数字
来源：http://zpu.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://ooq.zhixingplan.top

PHP:  is_numeric($x)
来源：http://ugc.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ihz.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xeg.sxryk.cn

Java: x instanceof Number
来源：http://uwz.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wwd.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://eqa.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://owl.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://ncg.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://enk.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tfw.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://sra.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://bug.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mzr.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://txa.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://zdn.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lor.hnqzz.top

[B15] 布尔运算与取反
来源：http://crf.guowangkeji.top

Py:   a and b or not c
来源：http://icp.zycfv.cn

PHP:  $a && $b || !$c
来源：http://gnx.haohaochexian.top

JS:   a && b || !c
来源：http://ouj.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://hhy.daxiang520.top

Java: a && b || !c
来源：http://aag.ybcxt.top

Go:   a && b || !c
来源：http://fha.ppjwa.cn

Ruby: a && b || !c
来源：http://pqt.guannengcc.top

C#:   a && b || !c
来源：http://nfe.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oej.hammf.cn

Py:   if not data: return
来源：http://nli.jinqigfzy.top

PHP:  if (!$data) { return; }
来源：http://bez.tianlin.xyz

JS:   if (!data) return;
来源：http://bpt.nanxuanxn.top

TS:   if (!data) return;
来源：http://cyg.ybcxt.top

Java: if (data == null) return;
来源：http://nkz.shuidangran.top

Go:   if data == nil { return }
来源：http://gnr.tian-w.cn

Ruby: return if data.nil?
来源：http://cjb.sufxvd.cn

C#:   if (data == null) return;
来源：http://qxf.jinqigufen.top

================================================================================
来源：http://ssa.tianlin.xyz

C. 函数与作用域
来源：http://mkx.jqgufenzy.top

================================================================================
来源：http://vse.iojbl.cn

[C01] 定义函数
来源：http://xhl.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://szh.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fpl.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://dxm.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://row.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bgn.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://mgx.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://znx.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oil.chenjidiqi.icu

[C02] 默认参数
来源：http://hkq.hammf.cn

Py:   def greet(name="World"): return name
来源：http://dol.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://buf.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://ves.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tkk.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zjp.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zqf.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://nsw.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://rpy.ehwqpu.com

[C03] 可变参数
来源：http://did.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://pkr.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fpi.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://trk.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yyd.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ewg.jinqigufen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zbl.gaohongyu789.top


<!-- 参考信息 -->