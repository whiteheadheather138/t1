代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kdx.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fgj.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cae.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://mma.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://ccq.yj202588.top

PHP:  implode(", ", $arr);
来源：http://hbf.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://ugv.guowangkeji.top

TS:   arr.join(", ")
来源：http://syu.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://dmu.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://hcd.hammf.cn

Ruby: arr.join(", ")
来源：http://ggz.smart0.xyz

C#:   string.Join(", ", list)
来源：http://mjw.cheryme.top

================================================================================
来源：http://rmq.9152youxi.cn

E. 字符串处理
来源：http://ylc.zycfv.cn

================================================================================
来源：http://wli.uphjek.com

[E01] 拼接字符串
来源：http://ucp.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pev.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oek.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://khy.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rjp.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zxx.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vau.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rse.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://epc.fzhhl.top

[E02] 重复字符串
来源：http://jui.cashguo.top

Py:   "ab" * 3
来源：http://vob.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://dpb.tanke756.top

JS:   "ab".repeat(3)
来源：http://hkf.yonumen.top

TS:   "ab".repeat(3)
来源：http://bvb.pycfn.com

Java: "ab".repeat(3)
来源：http://dae.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://kqy.aibaodan.cn

Ruby: "ab" * 3
来源：http://ggf.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rdo.yongpay.top

[E03] 截取子串
来源：http://vrx.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://olk.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mob.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hqs.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://lmw.tarul.cn

Java: s.substring(1, 4)
来源：http://bhm.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jir.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://qlp.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://rnc.hnqzz.top

[E04] 查找子串位置
来源：http://vgm.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://epp.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://lks.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gwv.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://wvk.zhengqikj.top

Java: s.indexOf("x")
来源：http://ejc.yonumen.top

Go:   strings.Index(s, "x")
来源：http://kew.pengpengdd.cyou

Ruby: s.index("x")
来源：http://crb.yonumen.top

C#:   s.IndexOf("x")
来源：http://yjb.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://bjj.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bov.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://avs.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bxd.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ruq.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://via.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pjj.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ced.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://idf.andypj.xyz

[E06] 替换子串
来源：http://ofb.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kug.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://myo.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yox.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://jgo.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jpa.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qnz.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hfc.uphjek.com

C#:   s.Replace("a", "b")
来源：http://zzb.hesvh.cn

[E07] 按分隔符拆分
来源：http://pon.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gmk.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wcv.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://shq.pycfn.com

TS:   s.split(",")
来源：http://lsx.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cli.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fsr.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://yti.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vzb.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://jno.hcnkem.com

Py:   ",".join(items)
来源：http://ujk.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://msd.fanxiaobao.xyz

JS:   items.join(",")
来源：http://ped.zhengqikj.top

TS:   items.join(",")
来源：http://oyc.andypj.xyz

Java: String.join(",", items)
来源：http://pol.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://iww.chenjidiqi.icu

Ruby: items.join(",")
来源：http://gfg.xinyue.icu

C#:   string.Join(",", items)
来源：http://xtd.sxryk.cn

[E09] 去除所有空白字符
来源：http://xkf.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yvz.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://txd.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://zky.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://zsm.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://obw.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ckc.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://eot.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fff.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://xtz.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://res.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xcu.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://sod.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://rne.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://wry.mhx1999.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hce.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rpq.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xfn.xinyue.icu

[E11] 反转字符串
来源：http://lhe.smart0.xyz

Py:   s[::-1]
来源：http://tcm.nanxuanxn.top

PHP:  strrev($s);
来源：http://hzb.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://zsf.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://exm.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wof.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hlj.yonumen.top

Ruby: s.reverse
来源：http://vju.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://ywe.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://ajw.ehwqpu.com

Py:   s.count("a")
来源：http://hvt.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://lhz.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://irb.bjfxy.top

TS:   s.split("a").length - 1
来源：http://kfs.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qvj.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://dmv.jqgufenzy.top

Ruby: s.count("a")
来源：http://asv.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://oxd.ydzc1.top

[E13] 逐字符遍历
来源：http://szy.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://yab.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rxx.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ijw.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gku.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://prr.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tpo.cdnleiting.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dpg.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hib.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://qtk.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://weq.tianlin.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://xhz.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yth.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://doc.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nec.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gfz.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cqu.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qut.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://jzw.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qnn.hnxiangtu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kwi.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ilr.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gdd.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bkn.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://slt.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mcs.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://khj.hysaishi.cn

[E16] 数字千分位
来源：http://vfr.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://udx.chenlongwang.top

PHP:  number_format(1234567);
来源：http://tay.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://obj.jlsjyb.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://edj.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rcb.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rml.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tlm.zhengqikj.top

C#:   1234567.ToString("N0")
来源：http://mom.wangshuangyany.cn

[E17] 首字母大写
来源：http://tug.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zeo.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qqu.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vsc.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hrl.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qlf.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://siv.zdqjudy.top

Ruby: s.capitalize
来源：http://nqj.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dks.aibaodan.cn

[E18] 模板占位符替换
来源：http://swa.vehdjk.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yuf.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bfo.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sqf.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zbe.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lsi.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fmx.yfazqb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://otv.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zsr.sysykeji.top

[E19] 多行文本按行拆分
来源：http://lwd.mhx1999.top

Py:   s.splitlines()
来源：http://bla.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nmk.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://oot.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://mjz.mhx1999.top

Java: s.lines().toList()
来源：http://qpt.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://opq.feifeiyinyue.top

Ruby: s.lines
来源：http://gto.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://lsf.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://hqe.fehbvm.com

Py:   if not s:
来源：http://zkr.daria6918.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fhy.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tkk.hammf.cn

TS:   if (s === "") {}
来源：http://zwh.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://xyn.hywenlv.cn

Go:   if s == "" {}
来源：http://ccs.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://atn.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ngh.shuidangran.top

[E21] 超长截断加省略号
来源：http://ifm.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xxe.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vsd.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zdp.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://njj.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bat.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://vts.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tvn.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kud.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://cwd.zhixingplan.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jha.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iyu.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cxh.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aui.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dze.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hrd.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://ylp.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hfi.xziqi.cn

================================================================================
来源：http://dga.yj20258.top

F. 文件与目录
来源：http://lmn.gogol.net.cn

================================================================================
来源：http://orw.fktsv.cn

[F01] 读取整个文件
来源：http://aie.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eyt.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://lhv.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wgy.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://viv.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cyd.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rop.shuidangran.top

Ruby: File.read("a.txt")
来源：http://wff.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://bxn.shzxlz.cn

[F02] 逐行读取文件
来源：http://ixu.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mie.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bmy.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vfu.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ami.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tgk.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fay.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gfx.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xbm.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://kct.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mxz.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zqs.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://klh.dashuyun.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wbi.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pot.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://suh.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://bnj.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tri.gogol.net.cn

[F04] 追加写入文件
来源：http://dym.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cyu.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ctp.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rln.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://udn.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://owy.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mqu.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dcb.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qng.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://goz.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wbf.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://hpe.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://wst.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://pjg.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://woz.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ncg.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://mnl.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://cjw.ehwqpu.com

[F06] 删除文件
来源：http://nkx.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://lsh.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://nsu.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rwm.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://bga.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gwm.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://vbl.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://skg.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://wvc.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://bgt.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kzz.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wzp.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zme.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://upm.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://goe.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lnq.dashuyun.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wtp.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dfv.dashuyun.cn

[F08] 遍历目录
来源：http://vda.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bxg.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hxu.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://nxg.kuanghao11.cn

TS:   fs.readdirSync("dir")
来源：http://enr.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jdt.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://soy.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://ckm.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://kqx.tanke756.top

[F09] 获取文件大小
来源：http://aeh.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://ljb.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://izn.yuxming.cn

JS:   fs.statSync("a.txt").size
来源：http://ivy.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://gsa.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xfd.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://olb.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://qod.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://bep.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://qhm.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mic.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kvb.zdqjudy.top


<!-- 参考信息 -->