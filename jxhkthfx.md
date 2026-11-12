代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://lbg.xuetiantiany.cn

Go:   fmt.Println("Hello, World!")
来源：http://xal.316326.xyz

Ruby: puts "Hello, World!"
来源：http://cvb.birdmap.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cgx.cqqwz.cn

[A02] 变量声明与赋值
来源：http://alc.cqqwz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wau.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rwa.hywenlv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hba.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zmv.feifeiyinyue.top

Java: String name = "Alex"; int age = 20;
来源：http://tzl.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://wvk.ydzc1.top

Ruby: name = "Alex"; age = 20
来源：http://zeq.aibaodan.cn

C#:   string name = "Alex"; int age = 20;
来源：http://puq.yj20258888.top

[A03] 常量定义
来源：http://xia.haohaochexian.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wft.quarkkingdee.top

PHP:  const PI = 3.14159;
来源：http://iuw.gaohongyu789.top

JS:   const PI = 3.14159;
来源：http://bfl.fanxiaobao.xyz

TS:   const PI: number = 3.14159;
来源：http://frf.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://lwt.xingfuxueyuan.xyz

Go:   const PI = 3.14159
来源：http://pqf.cdnleiting.top

Ruby: PI = 3.14159
来源：http://kwe.quarkkingdee.top

C#:   const double PI = 3.14159;
来源：http://nxj.sxryk.cn

[A04] 判断变量类型
来源：http://pjh.fzhhl.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tba.fktsv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fvp.ywan-chungtsiang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sqe.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://ymg.meibo888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ulu.fzhhl.top

Go:   reflect.TypeOf(x).Name()
来源：http://wgt.svipenyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oho.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://xbr.iojbl.cn

[A05] 整数除法与取模
来源：http://hfq.xinyue.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://med.yueranfly.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ztz.wangshuangyany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lgj.ehwqpu.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nsg.sysykeji.top

Java: 7 / 2; 7 % 2
来源：http://brt.chenzaomai.com

Go:   7 / 2; 7 % 2
来源：http://apm.hcnkem.com

Ruby: 7 / 2; 7 % 2
来源：http://mre.tarul.cn

C#:   7 / 2; 7 % 2
来源：http://meg.mhx1999.top

[A06] 字符串转数字
来源：http://fcj.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://zub.zhengqikj.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fgt.vqdsnc.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zle.zhaomingkeji.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://nxd.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://omv.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://smy.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://oqz.tarul.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cap.cashguo.top

[A07] 数字转字符串
来源：http://bfr.hywenlv.cn

Py:   str(42)
来源：http://tlg.bjfxy.top

PHP:  (string) 42; strval(42)
来源：http://nbj.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://nwr.hnxiangtu.top

TS:   String(42)
来源：http://kii.jinyuanbaomall.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wgo.ivvv.top

Go:   strconv.Itoa(42)
来源：http://vae.jiagoushi.top

Ruby: 42.to_s
来源：http://ums.nanxinkj.top

C#:   42.ToString()
来源：http://bqo.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://pfl.xuetiantiany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jdq.zhongyouzk.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vpf.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qbj.havefunace.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eod.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yln.tianlin.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tpn.hfpthk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zgi.gzhubu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kwh.tianlin.xyz

[A09] 绝对值与最大最小值
来源：http://mze.nanxinkj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uvd.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bwu.yj202588.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kpx.sjlbkw.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qob.jinqigfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ldq.tanke756.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bzl.nanxuanxn.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yxw.dianchejie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qvl.zycfv.cn

[A10] 生成随机数
来源：http://wbg.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://siy.hysaishi.cn

PHP:  random_int(1, 100);
来源：http://ycm.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kfg.dashuyun.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cjg.wangshuangyany.cn

Java: new Random().nextInt(100) + 1
来源：http://gwn.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kqg.guannengcc.top

Ruby: rand(1..100)
来源：http://lwy.yuanzhike.top

C#:   new Random().Next(1, 101)
来源：http://fty.xingfuxueyuan.xyz

[A11] 条件表达式（三元）
来源：http://ast.shanyushiyangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://sqp.daria6918.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rlj.smart0.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://oes.chenzaomai.com

TS:   x > 0 ? "yes" : "no"
来源：http://cll.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://mbk.yj202588.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dku.smart0.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://kgw.yj20258888.top

C#:   x > 0 ? "yes" : "no"
来源：http://ncx.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://jat.pengpengdd.cyou

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wia.cheryme.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vad.sysykeji.top

JS:   `Hello, ${name}!`
来源：http://xwk.yangfankeji.com

TS:   `Hello, ${name}!`
来源：http://qjm.yj20258.top

Java: "Hello, %s!".formatted(name)
来源：http://mnl.sjlbkw.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sya.cashguo.top

Ruby: "Hello, #{name}!"
来源：http://ive.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://txc.hnxiangtu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dto.daria6918.cn

Py:   "第一行\n第二行"
来源：http://ehr.ydjk.org.cn

PHP:  "第一行\n第二行"
来源：http://dgp.chenjidiqi.icu

JS:   "第一行\n第二行"
来源：http://usf.sysykeji.top

TS:   "第一行\n第二行"
来源：http://ycs.chenzaomai.com

Java: "第一行\n第二行"
来源：http://anr.bbcook.cn

Go:   "第一行\n第二行"
来源：http://mtp.cashguo.top

Ruby: "第一行\n第二行"
来源：http://chl.shuidangran.top

C#:   "第一行\n第二行"
来源：http://cvl.hysaishi.cn

[A14] 注释写法
来源：http://dnh.jinqigfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://opx.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://csr.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://wju.jqgfzy.top

TS:   // 单行；/* 多行 */
来源：http://mao.meibo888.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jmf.fzhhl.top

Go:   // 单行；/* 多行 */
来源：http://awk.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hxr.bjfxy.top

C#:   // 单行；/* 多行 */
来源：http://cnj.9152youxi.cn

[A15] 空值判断与默认值
来源：http://cpj.zhongyouzk.top

Py:   value = data or "默认值"
来源：http://unh.wangdashe.top

PHP:  $value = $data ?? "默认值";
来源：http://hjb.hesvh.cn

JS:   const value = data ?? "默认值";
来源：http://rsv.daxiang520.top

TS:   const value = data ?? "默认值";
来源：http://vhq.kuanghao11.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zvk.0kj1m.cn

Go:   if data == "" { data = "默认值" }
来源：http://dmv.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://dds.jqgufenzy.top

C#:   var value = data ?? "默认值";
来源：http://yoc.xziqi.cn

[A16] 真假值判断规则
来源：http://izg.meibo888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dnd.epnwcf.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oro.epnwcf.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ceu.hnxiangtu.top

TS:   if (!x) {}
来源：http://ryg.yj202588.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cyn.cashguo.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://krc.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mgv.yonumen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ctx.52xcode.cn

[A17] 位运算
来源：http://akk.nwbrower.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://buj.smart0.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mpy.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zle.xuetiantiany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zkt.zhixingplan.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lkj.jiagoushi.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iup.zhengqikj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jbq.hnqzz.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nax.zycfv.cn

[A18] 字符与 ASCII 码互转
来源：http://tcz.zycfv.cn

Py:   ord("A"); chr(65)
来源：http://qpp.ybcxt.top

PHP:  ord("A"); chr(65)
来源：http://aqt.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pzi.nanxinkj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ann.nwbrower.top

Java: (int) 'A'; (char) 65
来源：http://hqh.nanxuanxn.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dot.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://hje.jianghu66.top

C#:   (int)'A'; (char)65
来源：http://qod.hcnkem.com

[A19] 交换两个变量
来源：http://vhs.daria6918.cn

Py:   a, b = b, a
来源：http://kob.yvedp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ruc.aizwys.cn

JS:   [a, b] = [b, a];
来源：http://zcb.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://szq.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://ddi.ywan-chungtsiang.top

Go:   a, b = b, a
来源：http://aup.fengsongda.top

Ruby: a, b = b, a
来源：http://zat.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://wgn.yonumen.top

[A20] 读取标准输入
来源：http://aic.ehwqpu.com

Py:   name = input("请输入：")
来源：http://qxp.ctjpmb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://kvm.gotoacloud.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bku.cashguo.top

TS:   // Node.js：readline 模块
来源：http://hti.hesvh.cn

Java: new Scanner(System.in).nextLine()
来源：http://ezb.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vnw.pycfn.com

Ruby: gets.chomp
来源：http://dwm.jinqigufen.top

C#:   Console.ReadLine();
来源：http://lkh.fehbvm.com

[A21] 保留指定小数位输出
来源：http://cxh.zdqjudy.top

Py:   f"{3.14159:.2f}"
来源：http://lty.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jar.pycfn.com

JS:   (3.14159).toFixed(2)
来源：http://auo.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://sna.xuanzx.com

Java: String.format("%.2f", 3.14159)
来源：http://fts.pycfn.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kym.sufxvd.cn

Ruby: format("%.2f", 3.14159)
来源：http://smu.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://lij.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://fjl.jinqigufen.top

Py:   len(s)
来源：http://qke.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pxx.ehwqpu.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eoo.pycfn.com

TS:   s.length
来源：http://yue.yvedp.cn

Java: s.length()
来源：http://uxt.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iqz.shzxlz.cn

Ruby: s.length
来源：http://uwg.zhijiandao.cn

C#:   s.Length
来源：http://yyy.jinghuilouyu.cn

[A23] 大小写转换
来源：http://ugb.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fbv.wangdashe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qhc.ydzc1.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lqj.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hjc.sufxvd.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wli.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://asd.yj20258.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nzy.fehbvm.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ros.yuanzhike.top

[A24] 去除首尾空白
来源：http://how.zhiwuduotai.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bzo.0kj1m.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hun.xziqi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gbl.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://chm.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fua.hesvh.cn

Go:   strings.TrimSpace(s)
来源：http://kon.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jwy.havefunace.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://erh.haohaochexian.top

[A25] 字符串比较
来源：http://kgt.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://chi.zhijiandao.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ohy.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oxz.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zdi.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jpo.smart0.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aus.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qjt.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://isq.fktsv.cn

[A26] 类型转换总览
来源：http://sbh.uphjek.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gcs.sxryk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://udm.zhixingplan.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sga.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://tuw.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vfa.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ouv.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://lrb.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fvp.birdmap.top

================================================================================
来源：http://han.gogol.net.cn

B. 流程控制
来源：http://hni.ybcxt.top

================================================================================
来源：http://ebm.zycfv.cn

[B01] 条件判断 if / else
来源：http://zru.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zdh.gaohongyu789.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://htq.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tes.sysykeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yky.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://ctk.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bpw.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://via.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wrj.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://yeb.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gbc.yj20258.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mtv.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://all.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aew.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gyo.birdmap.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cis.zhengqikj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jsr.zhijiandao.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cvd.guowangkeji.top

[B03] switch / match / case
来源：http://pei.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pxr.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zdp.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zxz.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vjg.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ihr.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lrl.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vgq.zdqjudy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zhm.9152youxi.cn

[B04] for 计数循环
来源：http://xkn.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://fag.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wrl.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://obk.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dyi.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qmw.sysykeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fsp.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://xxp.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yqw.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://uvi.yangfankeji.com

Py:   for item in arr: print(item)
来源：http://nfa.cucudq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bir.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bka.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jrp.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://oro.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fki.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://iev.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wdc.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://cbg.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iug.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gci.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kib.dianchejie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rfc.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://byk.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://syl.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ers.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://slr.yongpay.top

[B07] while 循环
来源：http://ers.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://zfl.cheryme.top

PHP:  while ($i < 10) { $i++; }
来源：http://hie.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://tja.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://alf.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://atk.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lek.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://ala.feifeiyinyue.top

C#:   while (i < 10) { i++; }
来源：http://gno.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://fko.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://unx.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://oxs.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://xcn.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://qii.jianghu66.top


<!-- 参考信息 -->