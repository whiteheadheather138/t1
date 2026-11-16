代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fkc.hesvh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://giw.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cgl.yongpay.top

[D26] 数组转字符串
来源：http://nas.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://dyr.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://fpc.tian-w.cn

JS:   arr.join(", ")
来源：http://bxu.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://wcc.quarkkingdee.top

Java: String.join(", ", list)
来源：http://joz.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://uzi.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://aeq.yvedp.cn

C#:   string.Join(", ", list)
来源：http://euq.kuanghao11.cn

================================================================================
来源：http://avz.zhixingplan.top

E. 字符串处理
来源：http://mhz.tian-w.cn

================================================================================
来源：http://swk.havefunace.top

[E01] 拼接字符串
来源：http://nkl.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rmv.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vvv.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://clh.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wxj.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://txz.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wjo.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ksi.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ikw.haohaochexian.top

[E02] 重复字符串
来源：http://ydq.kuanghao11.cn

Py:   "ab" * 3
来源：http://tul.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://ubr.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://yvm.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://qoc.c1oappe.top

Java: "ab".repeat(3)
来源：http://tjo.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://kqp.havefunace.top

Ruby: "ab" * 3
来源：http://zyj.wangshuangyany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pae.zhaomingkeji.xyz

[E03] 截取子串
来源：http://bdf.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mku.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wyi.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yyp.316326.xyz

TS:   s.slice(1, 4)
来源：http://dqg.nwbrower.top

Java: s.substring(1, 4)
来源：http://ald.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nrs.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fqd.yonumen.top

C#:   s.Substring(1, 3)
来源：http://lea.shzxlz.cn

[E04] 查找子串位置
来源：http://mzw.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://mrt.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://fhw.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fab.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://lxe.ivvv.top

Java: s.indexOf("x")
来源：http://bcq.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://kmz.fzhhl.top

Ruby: s.index("x")
来源：http://bin.xinyue.icu

C#:   s.IndexOf("x")
来源：http://eoy.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ovl.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jar.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dgp.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxh.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zeq.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://knd.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nbk.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qrq.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ybi.fktsv.cn

[E06] 替换子串
来源：http://eix.guannengcc.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aua.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://nhy.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qsj.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://luf.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ist.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uxy.sxryk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nco.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://sdl.hcnkem.com

[E07] 按分隔符拆分
来源：http://jsf.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hxu.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bdl.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iqd.zhixingplan.top

TS:   s.split(",")
来源：http://uwu.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://hjk.vqdsnc.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bnd.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://ftv.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://awd.uphjek.com

[E08] 数组按分隔符合并
来源：http://iee.yuanzhike.top

Py:   ",".join(items)
来源：http://lmw.pycfn.com

PHP:  implode(",", $items);
来源：http://nid.aizwys.cn

JS:   items.join(",")
来源：http://bot.chenzaomai.com

TS:   items.join(",")
来源：http://tsa.316326.xyz

Java: String.join(",", items)
来源：http://zxi.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://ufb.cucudq.cn

Ruby: items.join(",")
来源：http://dnx.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://vtk.ehwqpu.com

[E09] 去除所有空白字符
来源：http://nyo.shuidangran.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://brv.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zrx.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://orq.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://vwq.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://oon.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://brv.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qpz.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hqk.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://mlp.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dvt.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qgc.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://owc.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://rsy.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://utz.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://oco.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aia.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ncu.zdqjudy.top

[E11] 反转字符串
来源：http://ebw.hesvh.cn

Py:   s[::-1]
来源：http://eni.zhijiandao.cn

PHP:  strrev($s);
来源：http://efr.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://yis.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://dks.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sqg.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ein.xuetiantiany.cn

Ruby: s.reverse
来源：http://ldm.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tgr.nwbrower.top

[E12] 统计某字符出现次数
来源：http://zdh.c1oappe.top

Py:   s.count("a")
来源：http://bgu.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://vnd.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://jdp.sxryk.cn

TS:   s.split("a").length - 1
来源：http://yal.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kmr.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://yhk.ctjpmb.com

Ruby: s.count("a")
来源：http://elb.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://iym.hywenlv.cn

[E13] 逐字符遍历
来源：http://wjp.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://ils.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uur.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ltu.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cmn.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ynm.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rqu.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ugz.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pge.andypj.xyz

[E14] URL 编码与 Base64
来源：http://dkz.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vmq.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://njv.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nmx.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ypm.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://auq.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bhe.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cbe.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mrm.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://jtm.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pkc.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nfu.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jor.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gnv.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zlx.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dyo.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kaf.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ftp.bjfxy.top

[E16] 数字千分位
来源：http://xcs.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://moa.jqgfzy.top

PHP:  number_format(1234567);
来源：http://cuu.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://odd.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://uzn.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ahb.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eqy.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://erq.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://ezl.0kj1m.cn

[E17] 首字母大写
来源：http://yxm.yj202588.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hpb.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://owy.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ytk.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://epl.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kqz.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fua.shangyingyoupin.top

Ruby: s.capitalize
来源：http://pkm.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pjv.chenlongwang.top

[E18] 模板占位符替换
来源：http://esb.bjfxy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://omp.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://umz.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uav.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ofz.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iqn.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xjr.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dng.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hew.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://xvt.wangshuangyany.cn

Py:   s.splitlines()
来源：http://cxz.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rdk.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://usa.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://may.sxryk.cn

Java: s.lines().toList()
来源：http://rif.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://qrd.hfpthk.cn

Ruby: s.lines
来源：http://mrx.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://ick.hammf.cn

[E20] 判断字符串是否为空
来源：http://vsi.redwolf501.top

Py:   if not s:
来源：http://onv.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://peb.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zba.zhaomingkeji.xyz

TS:   if (s === "") {}
来源：http://tge.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://vdb.iojbl.cn

Go:   if s == "" {}
来源：http://kdw.mhx1999.top

Ruby: if s.empty?
来源：http://hri.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zww.gogol.net.cn

[E21] 超长截断加省略号
来源：http://alw.meibo888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nzr.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nhn.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wox.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ube.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahb.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://bvv.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://loq.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zmz.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://qhh.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://txe.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://paq.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://the.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mhl.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eyw.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wml.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://qms.jlsjyb.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nou.yangfankeji.com

================================================================================
来源：http://kjx.sufxvd.cn

F. 文件与目录
来源：http://smg.nanxuanxn.top

================================================================================
来源：http://qlv.hnxiangtu.top

[F01] 读取整个文件
来源：http://wac.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nhv.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://lkh.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ust.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vlk.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://glx.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fle.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://gug.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://vgl.yonumen.top

[F02] 逐行读取文件
来源：http://zoa.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pfv.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nct.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rkf.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ndg.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mmj.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ftn.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yco.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bqb.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://qjm.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hho.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eit.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qio.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zoh.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mvt.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://whl.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://kks.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pbo.guowangkeji.top

[F04] 追加写入文件
来源：http://nrx.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nyr.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://khp.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ztv.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xsi.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vxr.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fyq.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vsm.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wha.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://pih.jqgfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xys.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://lnp.fengsongda.top

JS:   fs.existsSync("a.txt")
来源：http://wyl.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://zzn.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cls.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://smb.yongpay.top

Ruby: File.exist?("a.txt")
来源：http://dhx.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://iww.zycfv.cn

[F06] 删除文件
来源：http://bln.uphjek.com

Py:   os.remove("a.txt")
来源：http://gap.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://cms.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://njo.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dny.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://abf.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://pbf.tanke756.top

Ruby: File.delete("a.txt")
来源：http://hbc.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://kop.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://sov.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://euh.jlsjyb.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://osk.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cxu.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ani.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://afk.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oxh.sysykeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nfx.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://spy.jinghuilouyu.cn

[F08] 遍历目录
来源：http://izr.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dvh.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://amr.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://yyd.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://ifs.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lkv.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gmk.yuxming.cn

Ruby: Dir.children("dir")
来源：http://pgd.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://asm.ehwqpu.com

[F09] 获取文件大小
来源：http://vdd.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://wkp.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://bup.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://vux.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://yas.gzhubu.top

Java: Files.size(Path.of("a.txt"))
来源：http://uwb.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://igm.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://pic.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://ldv.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://iuw.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vnx.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ynp.tianlin.xyz


<!-- 参考信息 -->