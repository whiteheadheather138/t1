代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eno.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://ocb.daria6918.cn

C#:   $"Hello, {name}!"
来源：http://inw.quarkkingdee.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tvj.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://bbx.ydjk.org.cn

PHP:  "第一行\n第二行"
来源：http://iyo.epnwcf.com

JS:   "第一行\n第二行"
来源：http://xar.fanxiaobao.xyz

TS:   "第一行\n第二行"
来源：http://uol.snrcjt.cn

Java: "第一行\n第二行"
来源：http://mnp.guannengcc.top

Go:   "第一行\n第二行"
来源：http://msh.vqdsnc.cn

Ruby: "第一行\n第二行"
来源：http://vha.uphjek.com

C#:   "第一行\n第二行"
来源：http://cnl.c1oappe.top

[A14] 注释写法
来源：http://rxm.gotoacloud.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://frn.jianghu66.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lfk.gzhubu.top

JS:   // 单行；/* 多行 */
来源：http://ehc.c1oappe.top

TS:   // 单行；/* 多行 */
来源：http://apq.jlsjyb.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jfm.zdbjq.cn

Go:   // 单行；/* 多行 */
来源：http://djg.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://wmg.havefunace.top

C#:   // 单行；/* 多行 */
来源：http://fyf.svipenyu.cn

[A15] 空值判断与默认值
来源：http://hrf.ydjk.org.cn

Py:   value = data or "默认值"
来源：http://hni.guannengcc.top

PHP:  $value = $data ?? "默认值";
来源：http://mpl.dashuyun.cn

JS:   const value = data ?? "默认值";
来源：http://ujj.jinghuilouyu.cn

TS:   const value = data ?? "默认值";
来源：http://jqz.hongshengwenyu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wwa.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://eox.wangshuangyany.cn

Ruby: value = data || "默认值"
来源：http://kfq.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://cej.zhixingplan.top

[A16] 真假值判断规则
来源：http://jao.yuanzhike.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vmy.ybcxt.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://syt.jqgufenzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uoc.jlsjyb.cn

TS:   if (!x) {}
来源：http://uzk.vqdsnc.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ebx.ydzc1.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yeu.nwbrower.top

Ruby: unless x            # nil 与 false 为假
来源：http://vum.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sxz.0kj1m.cn

[A17] 位运算
来源：http://wfh.daria6918.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zuo.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://aqy.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jak.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gnj.0kj1m.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hla.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://juw.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jtf.jinghuilouyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://npt.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://wah.ydjk.org.cn

Py:   ord("A"); chr(65)
来源：http://fka.yj20258.top

PHP:  ord("A"); chr(65)
来源：http://yly.fengsongda.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://krx.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mrw.xuetiantiany.cn

Java: (int) 'A'; (char) 65
来源：http://xul.daxiang520.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pcq.yj20258888.top

Ruby: "A".ord; 65.chr
来源：http://agz.chenzaomai.com

C#:   (int)'A'; (char)65
来源：http://vkr.ywan-chungtsiang.top

[A19] 交换两个变量
来源：http://rel.aizwys.cn

Py:   a, b = b, a
来源：http://itw.shuidangran.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sql.sweek.top

JS:   [a, b] = [b, a];
来源：http://vwv.xingfuxueyuan.xyz

TS:   [a, b] = [b, a];
来源：http://orb.xingfuxueyuan.xyz

Java: int t = a; a = b; b = t;
来源：http://vxp.wangdashe.top

Go:   a, b = b, a
来源：http://yho.daxiang520.top

Ruby: a, b = b, a
来源：http://dpf.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://siz.sjlbkw.cn

[A20] 读取标准输入
来源：http://fdh.zhengqikj.top

Py:   name = input("请输入：")
来源：http://ddk.redwolf501.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ctz.redwolf501.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://msm.smart0.xyz

TS:   // Node.js：readline 模块
来源：http://qle.guannengcc.top

Java: new Scanner(System.in).nextLine()
来源：http://tuf.yueranfly.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wbq.kuanghao11.cn

Ruby: gets.chomp
来源：http://irv.daria6918.cn

C#:   Console.ReadLine();
来源：http://nyv.zhongyouzk.top

[A21] 保留指定小数位输出
来源：http://rlg.yuxming.cn

Py:   f"{3.14159:.2f}"
来源：http://rfg.shangyingyoupin.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qem.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://nim.yj20258.top

TS:   (3.14159).toFixed(2)
来源：http://mpo.zhoulong.xyz

Java: String.format("%.2f", 3.14159)
来源：http://djm.gogol.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zwx.kuanghao11.cn

Ruby: format("%.2f", 3.14159)
来源：http://opf.tarul.cn

C#:   3.14159.ToString("F2")
来源：http://twk.jqgfzy.top

[A22] 获取字符串长度
来源：http://sjt.jinqigfzy.top

Py:   len(s)
来源：http://ogb.jinghuilouyu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yox.hywenlv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rvq.redwolf501.top

TS:   s.length
来源：http://yan.andypj.xyz

Java: s.length()
来源：http://szj.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zpx.ppjwa.cn

Ruby: s.length
来源：http://atk.yuanzhike.top

C#:   s.Length
来源：http://nhj.xuetiantiany.cn

[A23] 大小写转换
来源：http://jfc.zhixingplan.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hpw.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://upu.nanxinkj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sed.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kxt.gotoacloud.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wdh.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://smn.yj20258888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wrc.fehbvm.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ckv.cdnleiting.top

[A24] 去除首尾空白
来源：http://aaa.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://waj.ppjwa.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gyn.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://boy.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://irl.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wwl.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://mrr.jqgfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://njr.tian-w.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dpz.epnwcf.com

[A25] 字符串比较
来源：http://efb.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://tto.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eeg.c1oappe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://flk.xuetiantiany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mzc.jinqigufen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nxq.jlsjyb.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://olt.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yqk.chenzaomai.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hjb.cdnleiting.top

[A26] 类型转换总览
来源：http://zfk.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vuy.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cag.ppjwa.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ljj.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://bhz.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nms.kuanghao11.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lcs.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://eph.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dxr.yongpay.top

================================================================================
来源：http://emq.zhoulong.xyz

B. 流程控制
来源：http://uno.cashguo.top

================================================================================
来源：http://qht.bbcook.cn

[B01] 条件判断 if / else
来源：http://zlg.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hfq.fanxiaobao.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wxw.iojbl.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ubm.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ndp.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xvx.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zca.zycfv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jfd.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mli.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://pnc.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iqb.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nxs.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vwu.smart0.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqi.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sgg.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://das.zhaomingkeji.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ecp.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://whm.aibaodan.cn

[B03] switch / match / case
来源：http://qdy.uphjek.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vyv.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rsf.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eca.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gjw.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fzx.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ena.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vna.bbcook.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bfk.quarkkingdee.top

[B04] for 计数循环
来源：http://iio.cashguo.top

Py:   for i in range(10): print(i)
来源：http://zyw.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fkh.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tdd.sxryk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pxx.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nmb.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jxe.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://vft.jianghu66.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ntq.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://iav.shuidangran.top

Py:   for item in arr: print(item)
来源：http://yby.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ano.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fjp.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cod.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jkl.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fzh.wangshuangyany.cn

Ruby: arr.each { |item| puts item }
来源：http://mrl.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zyc.cashguo.top

[B06] 遍历字典 / 对象
来源：http://lga.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vzu.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bda.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mmt.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jhy.yonumen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yum.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dxo.jinghuilouyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vma.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xgn.yj20258888.top

[B07] while 循环
来源：http://qjx.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://lmr.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://lme.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://oqu.guannengcc.top

TS:   while (i < 10) { i++; }
来源：http://uos.birdmap.top

Java: while (i < 10) { i++; }
来源：http://dkv.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://toh.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://klt.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://fqy.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://hbh.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://mfg.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wsf.quarkkingdee.top

JS:   do { i++; } while (i < 10);
来源：http://rpc.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://tls.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://rza.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dju.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://zhn.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://gtw.wangdashe.top

[B09] break 与 continue
来源：http://urf.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ype.nanxuanxn.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mix.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dxs.uphjek.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ofp.jinghuilouyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aau.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mim.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gzb.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eho.meibo888.top

[B10] 遍历同时拿索引
来源：http://zoi.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uaq.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iba.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gda.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uym.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rgr.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qfo.havefunace.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qej.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aaq.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://pos.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://xxi.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://lnb.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://obs.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ltm.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vsn.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iec.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://kbw.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kzw.yj20258.top

[B12] 跳出多层循环
来源：http://usc.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gax.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zip.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rqb.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wwf.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bzl.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://axu.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rsl.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oxh.zhoulong.xyz

[B13] 判断是否为数字
来源：http://nhn.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://caa.jinqigufen.top

PHP:  is_numeric($x)
来源：http://ppn.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cub.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nwn.gogol.net.cn

Java: x instanceof Number
来源：http://urj.yuanzhike.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wzn.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://jrf.chenlongwang.top

C#:   x is int or double or decimal
来源：http://fkn.smart0.xyz

[B14] 判断值是否在集合内
来源：http://crn.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://guc.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ogh.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://erg.shangyingyoupin.top

TS:   [1, 2, 3].includes(x)
来源：http://yoo.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://rxd.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tab.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://jjz.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lnx.c1oappe.top

[B15] 布尔运算与取反
来源：http://xyj.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://xku.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://bci.uphjek.com

JS:   a && b || !c
来源：http://jog.jqgufenzy.top

TS:   a && b || !c
来源：http://ged.smart0.xyz

Java: a && b || !c
来源：http://haw.yueranfly.top

Go:   a && b || !c
来源：http://gyy.zhixingplan.top

Ruby: a && b || !c
来源：http://bds.kuanghao11.cn

C#:   a && b || !c
来源：http://pgl.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xbe.yj20258.top

Py:   if not data: return
来源：http://jyt.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://exq.yj20258888.top

JS:   if (!data) return;
来源：http://oqm.zdqjudy.top

TS:   if (!data) return;
来源：http://imm.hysaishi.cn

Java: if (data == null) return;
来源：http://cdt.ydzc1.top

Go:   if data == nil { return }
来源：http://gsd.c1oappe.top

Ruby: return if data.nil?
来源：http://pzz.sufxvd.cn

C#:   if (data == null) return;
来源：http://uul.yanxiufei.cn

================================================================================
来源：http://pkl.wangdashe.top

C. 函数与作用域
来源：http://qwt.sufxvd.cn

================================================================================
来源：http://tqs.cqqwz.cn

[C01] 定义函数
来源：http://fea.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://max.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hhl.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://nzk.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eba.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tkw.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://nxi.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://usv.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bua.ppjwa.cn

[C02] 默认参数
来源：http://lpc.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://mtd.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ggi.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://rzv.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lso.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tlh.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://byv.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://bby.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://vts.cdnleiting.top

[C03] 可变参数
来源：http://afy.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://pxg.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jce.aibaodan.cn


<!-- 参考信息 -->