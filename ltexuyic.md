代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://acb.pengpengdd.cyou

[A15] 空值判断与默认值
来源：http://sll.cucudq.cn

Py:   value = data or "默认值"
来源：http://siw.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://dkk.guannengcc.top

JS:   const value = data ?? "默认值";
来源：http://gle.ydzc1.top

TS:   const value = data ?? "默认值";
来源：http://rdj.andypj.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://aoh.aibaodan.cn

Go:   if data == "" { data = "默认值" }
来源：http://goc.xuetiantiany.cn

Ruby: value = data || "默认值"
来源：http://wpb.kuanghao11.cn

C#:   var value = data ?? "默认值";
来源：http://mcn.wangshuangyany.cn

[A16] 真假值判断规则
来源：http://oue.zhengqikj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://duf.ybcxt.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hfg.zhoulong.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ffq.hesvh.cn

TS:   if (!x) {}
来源：http://pph.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wry.chenjidiqi.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oam.jqgufenzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://ndn.9152youxi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fhm.tanke756.top

[A17] 位运算
来源：http://pac.birdmap.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qcw.fktsv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kvf.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mxe.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kpc.cucudq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://air.zdbjq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://usr.zhoulong.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pyf.zdbjq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tic.nanxinkj.top

[A18] 字符与 ASCII 码互转
来源：http://xos.nanxinkj.top

Py:   ord("A"); chr(65)
来源：http://ygt.sysykeji.top

PHP:  ord("A"); chr(65)
来源：http://gaw.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zfr.hfpthk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dcw.meibo888.top

Java: (int) 'A'; (char) 65
来源：http://yvn.aizwys.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ssu.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://lgw.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://aso.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://xzm.birdmap.top

Py:   a, b = b, a
来源：http://jnb.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://nqt.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://dtf.zycfv.cn

TS:   [a, b] = [b, a];
来源：http://ayl.tarul.cn

Java: int t = a; a = b; b = t;
来源：http://zim.0kj1m.cn

Go:   a, b = b, a
来源：http://btu.snrcjt.cn

Ruby: a, b = b, a
来源：http://eug.tarul.cn

C#:   (a, b) = (b, a);
来源：http://nwe.yuanzhike.top

[A20] 读取标准输入
来源：http://bfp.gogol.net.cn

Py:   name = input("请输入：")
来源：http://pgi.xingfuxueyuan.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://aem.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hpr.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://xpf.jinyuanbaomall.cn

Java: new Scanner(System.in).nextLine()
来源：http://buw.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gtl.xuanzx.com

Ruby: gets.chomp
来源：http://ber.andypj.xyz

C#:   Console.ReadLine();
来源：http://jat.gotoacloud.top

[A21] 保留指定小数位输出
来源：http://nnf.svipenyu.cn

Py:   f"{3.14159:.2f}"
来源：http://lmo.ybcxt.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pua.zhaomingkeji.xyz

JS:   (3.14159).toFixed(2)
来源：http://sgt.kuanghao11.cn

TS:   (3.14159).toFixed(2)
来源：http://wnr.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://lrg.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wyc.yj202588.top

Ruby: format("%.2f", 3.14159)
来源：http://tbu.hnqzz.top

C#:   3.14159.ToString("F2")
来源：http://zdp.meibo888.top

[A22] 获取字符串长度
来源：http://exq.kuanghao11.cn

Py:   len(s)
来源：http://hmh.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gbe.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kqc.bjfxy.top

TS:   s.length
来源：http://qqd.ybcxt.top

Java: s.length()
来源：http://eof.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ole.yj20258.top

Ruby: s.length
来源：http://prs.mhx1999.top

C#:   s.Length
来源：http://frl.daxiang520.top

[A23] 大小写转换
来源：http://yhy.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ats.cqqwz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kym.yfazqb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://krd.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://svu.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dur.dianchejie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gyn.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zlq.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ffn.quarkkingdee.top

[A24] 去除首尾空白
来源：http://snf.iojbl.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zsv.yj20258.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oga.meibo888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eln.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pgh.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rrl.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://yxa.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wth.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gwx.jinqigufen.top

[A25] 字符串比较
来源：http://gkz.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://pkn.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://osp.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://snw.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://phs.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zkk.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tsw.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hdk.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ljt.cdnleiting.top

[A26] 类型转换总览
来源：http://yun.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://isx.sysykeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://moe.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://miw.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://enl.yj202588.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ote.yuanzhike.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xkm.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hnk.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ndm.yj20258888.top

================================================================================
来源：http://xrg.yj20258888.top

B. 流程控制
来源：http://qks.uphjek.com

================================================================================
来源：http://wrb.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://znn.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://apz.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ytp.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lug.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fxh.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ojy.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tal.redwolf501.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bmw.nanxinkj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lyi.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://zti.hysaishi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://veu.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kfh.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jme.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbi.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qts.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://haj.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xdh.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ntf.yj20258888.top

[B03] switch / match / case
来源：http://pmk.ivvv.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xqu.jqgufenzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://erq.haohaochexian.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://won.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ljf.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wea.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xgq.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jgk.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zrs.zhiwuduotai.top

[B04] for 计数循环
来源：http://rky.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://hxa.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://myf.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://spd.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ihk.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zpn.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cjv.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://imi.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kzh.yongpay.top

[B05] 遍历数组 / 列表
来源：http://mqt.yj20258888.top

Py:   for item in arr: print(item)
来源：http://cdm.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xfe.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nya.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uev.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mab.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yrs.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://fri.yuxming.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://koe.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://xqw.hysaishi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://spj.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xif.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ujs.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zkq.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xyy.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ewf.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qsd.jinqigufen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xnv.jiagoushi.top

[B07] while 循环
来源：http://efz.xuetiantiany.cn

Py:   while i < 10: i += 1
来源：http://vln.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://szx.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://ovm.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://otx.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://qgx.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gvw.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://gng.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://tlh.ivvv.top

[B08] do-while（至少执行一次）
来源：http://oew.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://qvz.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://abm.xuanzx.com

JS:   do { i++; } while (i < 10);
来源：http://nqy.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://tan.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://jjj.cashguo.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pzp.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hdt.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://lcc.gzhubu.top

[B09] break 与 continue
来源：http://bcw.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tcd.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cmb.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvw.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzv.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kjx.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bvf.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://anj.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wzl.yuxming.cn

[B10] 遍历同时拿索引
来源：http://fia.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fgj.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zyx.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wzp.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bld.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://adn.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://add.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jia.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lnl.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://sdg.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://fmq.xuetiantiany.cn

PHP:  range(0, 10, 2);
来源：http://grh.yfazqb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qme.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vza.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ezc.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gzi.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://spt.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gpr.fengsongda.top

[B12] 跳出多层循环
来源：http://mws.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zgc.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xjz.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vce.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sjq.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kfj.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jjh.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jcx.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ann.sjlbkw.cn

[B13] 判断是否为数字
来源：http://liy.pengpengdd.cyou

Py:   isinstance(x, (int, float))
来源：http://ong.wangdashe.top

PHP:  is_numeric($x)
来源：http://mmm.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qut.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jpw.xinyue.icu

Java: x instanceof Number
来源：http://cqa.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iex.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://sfo.ybcxt.top

C#:   x is int or double or decimal
来源：http://idq.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://qjl.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mmb.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dbq.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://qtq.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://tli.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jey.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ply.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://rul.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ojj.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://rxg.hnxiangtu.top

Py:   a and b or not c
来源：http://fpw.fktsv.cn

PHP:  $a && $b || !$c
来源：http://yiz.shzxlz.cn

JS:   a && b || !c
来源：http://ezw.ehwqpu.com

TS:   a && b || !c
来源：http://rdo.52xcode.cn

Java: a && b || !c
来源：http://kmw.yueranfly.top

Go:   a && b || !c
来源：http://ykr.zhengqikj.top

Ruby: a && b || !c
来源：http://luc.xinyue.icu

C#:   a && b || !c
来源：http://frg.andypj.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://sxb.fehbvm.com

Py:   if not data: return
来源：http://hmi.gogol.net.cn

PHP:  if (!$data) { return; }
来源：http://pdd.chenlongwang.top

JS:   if (!data) return;
来源：http://hct.meibo888.top

TS:   if (!data) return;
来源：http://qnv.316326.xyz

Java: if (data == null) return;
来源：http://gmm.sjlbkw.cn

Go:   if data == nil { return }
来源：http://yxf.fengsongda.top

Ruby: return if data.nil?
来源：http://wbm.fehbvm.com

C#:   if (data == null) return;
来源：http://yoa.epnwcf.com

================================================================================
来源：http://ecw.zhoulong.xyz

C. 函数与作用域
来源：http://egj.hammf.cn

================================================================================
来源：http://ibp.hfpthk.cn

[C01] 定义函数
来源：http://ill.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://lsm.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gqi.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://dei.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oyj.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cib.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://piy.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://wuc.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eqr.iojbl.cn

[C02] 默认参数
来源：http://ajz.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://jnb.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://rbk.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://kgl.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://unm.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mkn.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://poq.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://ylc.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://vjj.mhx1999.top

[C03] 可变参数
来源：http://cis.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://rmw.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yse.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bly.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cun.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wcx.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qny.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://upj.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://crl.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://wsw.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://odb.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://esi.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gcx.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://awn.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://jsv.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://dli.chenlongwang.top

Ruby: f(a: 1, b: 2)
来源：http://uzg.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://cbg.jianghu66.top

[C05] 返回多个值
来源：http://rop.cucudq.cn

Py:   return a, b
来源：http://uwo.chenlongwang.top

PHP:  return [$a, $b];
来源：http://cfk.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://cdt.shuidangran.top

TS:   return { a, b };
来源：http://qna.yj20258888.top


<!-- 参考信息 -->