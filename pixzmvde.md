代发 wailian999

[A14] 注释写法
来源：http://xbe.vehdjk.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://iqx.zdqjudy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ngs.bbcook.cn

JS:   // 单行；/* 多行 */
来源：http://pxh.hongshengwenyu.top

TS:   // 单行；/* 多行 */
来源：http://zjp.fktsv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oof.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://tvz.bjfxy.top

Ruby: # 单行；=begin 多行 =end
来源：http://upb.jinqigfzy.top

C#:   // 单行；/* 多行 */
来源：http://yfm.andypj.xyz

[A15] 空值判断与默认值
来源：http://fsy.zhoulong.xyz

Py:   value = data or "默认值"
来源：http://auv.ppjwa.cn

PHP:  $value = $data ?? "默认值";
来源：http://ecm.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://ttm.nanxuanxn.top

TS:   const value = data ?? "默认值";
来源：http://krs.zhijiandao.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://alw.yuanzhike.top

Go:   if data == "" { data = "默认值" }
来源：http://gvx.yvedp.cn

Ruby: value = data || "默认值"
来源：http://pxs.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://irr.xylfe.cn

[A16] 真假值判断规则
来源：http://wko.tarul.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iof.fanxiaobao.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vkb.jqgfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ybj.tian-w.cn

TS:   if (!x) {}
来源：http://yzi.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vcw.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gey.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://tpm.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cxg.epnwcf.com

[A17] 位运算
来源：http://gjl.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eoy.cqqwz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jmk.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pwd.tian-w.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qls.jinyuanbaomall.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://myh.bjfxy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://thu.xziqi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nul.nanxinkj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://afv.jiagoushi.top

[A18] 字符与 ASCII 码互转
来源：http://mze.snrcjt.cn

Py:   ord("A"); chr(65)
来源：http://hwq.zhaomingkeji.xyz

PHP:  ord("A"); chr(65)
来源：http://jlu.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hhd.cashguo.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tyj.cucudq.cn

Java: (int) 'A'; (char) 65
来源：http://wtr.jianghu66.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qgr.jiagoushi.top

Ruby: "A".ord; 65.chr
来源：http://dpc.ivvv.top

C#:   (int)'A'; (char)65
来源：http://fms.ehwqpu.com

[A19] 交换两个变量
来源：http://vgv.bjfxy.top

Py:   a, b = b, a
来源：http://ras.fanxiaobao.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://ink.xinyue.icu

JS:   [a, b] = [b, a];
来源：http://zhx.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://vdm.smart0.xyz

Java: int t = a; a = b; b = t;
来源：http://fpe.guowangkeji.top

Go:   a, b = b, a
来源：http://gqx.chenzaomai.com

Ruby: a, b = b, a
来源：http://fsc.yj20258888.top

C#:   (a, b) = (b, a);
来源：http://eqk.jinqigfzy.top

[A20] 读取标准输入
来源：http://lvl.hongshengwenyu.top

Py:   name = input("请输入：")
来源：http://ysf.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yzl.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pte.fzhhl.top

TS:   // Node.js：readline 模块
来源：http://qye.zhaomingkeji.xyz

Java: new Scanner(System.in).nextLine()
来源：http://gdw.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aeo.gaohongyu789.top

Ruby: gets.chomp
来源：http://nxf.xuanzx.com

C#:   Console.ReadLine();
来源：http://dvw.chenjidiqi.icu

[A21] 保留指定小数位输出
来源：http://tsa.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://xlc.yuanzhike.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ojn.sysykeji.top

JS:   (3.14159).toFixed(2)
来源：http://feh.hesvh.cn

TS:   (3.14159).toFixed(2)
来源：http://pob.hysaishi.cn

Java: String.format("%.2f", 3.14159)
来源：http://qtv.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tva.vqdsnc.cn

Ruby: format("%.2f", 3.14159)
来源：http://bif.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://prn.yueranfly.top

[A22] 获取字符串长度
来源：http://nnb.tanke756.top

Py:   len(s)
来源：http://evf.yueranfly.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tll.zhoulong.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://udd.xinyue.icu

TS:   s.length
来源：http://ikv.ydzc1.top

Java: s.length()
来源：http://ndd.jqgfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lhl.daria6918.cn

Ruby: s.length
来源：http://nyo.jlsjyb.cn

C#:   s.Length
来源：http://xyp.dashuyun.cn

[A23] 大小写转换
来源：http://ywp.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://jwg.yuanzhike.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ppo.ppjwa.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fbg.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rvq.zycfv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mxl.yanxiufei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://elj.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lmc.jinyuanbaomall.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pyx.gaohongyu789.top

[A24] 去除首尾空白
来源：http://lmf.52xcode.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wwp.bbcook.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ois.jinqigfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jhw.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wbk.shangyingyoupin.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cra.aibaodan.cn

Go:   strings.TrimSpace(s)
来源：http://kix.52xcode.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gwc.cdnleiting.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iaf.nanxinkj.top

[A25] 字符串比较
来源：http://msw.sufxvd.cn

Py:   s1 == s2; s1 != s2
来源：http://nku.pycfn.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hhj.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://idq.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qez.ydjk.org.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xqs.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jfa.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cpf.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gjf.yongpay.top

[A26] 类型转换总览
来源：http://cii.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gmw.jqgfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dkj.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://inb.zdqjudy.top

TS:   Number() String() Boolean() x as number
来源：http://joc.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yvz.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sqw.hongshengwenyu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nci.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lbt.cucudq.cn

================================================================================
来源：http://ujd.shzxlz.cn

B. 流程控制
来源：http://vir.vqdsnc.cn

================================================================================
来源：http://rxc.jyoumei.cn

[B01] 条件判断 if / else
来源：http://fpo.ydzc1.top

Py:   result = "正" if x > 0 else "非正"
来源：http://crm.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zzh.shzxlz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rlt.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ghz.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uhc.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cag.quarkkingdee.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dql.316326.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tvl.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://vfz.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lxg.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kta.havefunace.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbb.ywan-chungtsiang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yzo.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bjf.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bhp.haohaochexian.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nrg.mhx1999.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rxa.pycfn.com

[B03] switch / match / case
来源：http://kke.jqgufenzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zas.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wlr.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://avm.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qky.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aea.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sgl.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jiw.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rkp.svipenyu.cn

[B04] for 计数循环
来源：http://xnx.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://vbp.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jgk.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mwo.sxryk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zkb.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cnj.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hbo.hongshengwenyu.top

Ruby: 10.times { |i| puts i }
来源：http://sag.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bov.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://asj.zycfv.cn

Py:   for item in arr: print(item)
来源：http://ami.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ggh.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wiy.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qcf.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://hon.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ecq.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://mpx.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jjp.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://dof.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://qlx.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rso.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rci.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vvt.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cav.chenjidiqi.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iar.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iof.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xqe.nwbrower.top

[B07] while 循环
来源：http://qmn.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://kxv.hcnkem.com

PHP:  while ($i < 10) { $i++; }
来源：http://ned.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://xzw.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://pit.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://rxg.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wco.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://mel.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://kxz.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://zhb.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://moe.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mqu.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://qhu.jinyuanbaomall.cn

TS:   do { i++; } while (i < 10);
来源：http://qem.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://unr.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ueb.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://qvm.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://lgg.shangyingyoupin.top

[B09] break 与 continue
来源：http://pbw.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cad.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lcs.fktsv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mqv.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpr.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lfx.hfpthk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jyi.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pmk.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sgi.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://zfx.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://knh.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ucy.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zoz.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oih.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kyx.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cli.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zvk.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eyx.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://mqd.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://uli.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://uvk.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gpm.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jhv.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oeh.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wkn.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://juv.sxryk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ndw.yuanzhike.top

[B12] 跳出多层循环
来源：http://wmz.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xym.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yal.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgq.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rwt.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yyu.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://onu.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qdh.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kwf.cdnleiting.top

[B13] 判断是否为数字
来源：http://kyx.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://rzm.shuidangran.top

PHP:  is_numeric($x)
来源：http://ckv.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ckj.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lxg.pengpengdd.cyou

Java: x instanceof Number
来源：http://cde.cqqwz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mza.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://dyl.yongpay.top

C#:   x is int or double or decimal
来源：http://cko.cashguo.top

[B14] 判断值是否在集合内
来源：http://exh.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ytt.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zhe.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://mmw.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://prh.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://rfp.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ybe.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://pkh.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ryy.yongpay.top

[B15] 布尔运算与取反
来源：http://zcp.hcnkem.com

Py:   a and b or not c
来源：http://eal.gzhubu.top

PHP:  $a && $b || !$c
来源：http://hid.yj20258888.top

JS:   a && b || !c
来源：http://ufv.hcnkem.com

TS:   a && b || !c
来源：http://lyj.jiagoushi.top

Java: a && b || !c
来源：http://jwc.vqdsnc.cn

Go:   a && b || !c
来源：http://lbi.zhongyouzk.top

Ruby: a && b || !c
来源：http://jup.pengpengdd.cyou

C#:   a && b || !c
来源：http://bmc.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://sxo.zycfv.cn

Py:   if not data: return
来源：http://rrh.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://yfr.fktsv.cn

JS:   if (!data) return;
来源：http://ott.xuanzx.com

TS:   if (!data) return;
来源：http://bfb.sysykeji.top

Java: if (data == null) return;
来源：http://cyx.dianchejie.cn

Go:   if data == nil { return }
来源：http://oqk.uphjek.com

Ruby: return if data.nil?
来源：http://rfo.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://vcb.sxryk.cn

================================================================================
来源：http://xai.redwolf501.top

C. 函数与作用域
来源：http://fyz.sweek.top

================================================================================
来源：http://owc.mhx1999.top

[C01] 定义函数
来源：http://toa.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://gvd.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kot.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://tev.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sud.svipenyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gsj.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://dgt.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://opp.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ujw.fengsongda.top

[C02] 默认参数
来源：http://tiq.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://vsh.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mpc.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://crv.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://bgo.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://juc.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kye.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://qkn.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://azo.jyoumei.cn

[C03] 可变参数
来源：http://gvp.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://ymh.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://huz.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nfj.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lmx.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mfu.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oij.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://kqu.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rhj.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://vzj.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fub.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rin.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nze.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://evc.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://hgn.quarkkingdee.top


<!-- 参考信息 -->