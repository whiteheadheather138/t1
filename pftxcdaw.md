代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://qyg.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://lkx.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://ygk.yanxiufei.cn

TS:   arr.join(", ")
来源：http://oaf.shuidangran.top

Java: String.join(", ", list)
来源：http://dfd.jianghu66.top

Go:   strings.Join(strs, ", ")
来源：http://bci.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://tjb.sweek.top

C#:   string.Join(", ", list)
来源：http://xie.yongpay.top

================================================================================
来源：http://opa.9152youxi.cn

E. 字符串处理
来源：http://err.jlsjyb.cn

================================================================================
来源：http://aaj.meibo888.top

[E01] 拼接字符串
来源：http://swx.ydzc1.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ulh.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cwg.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jci.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://grg.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yvw.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://htp.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cfa.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cbt.ydjk.org.cn

[E02] 重复字符串
来源：http://zqu.cdnleiting.top

Py:   "ab" * 3
来源：http://igr.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://ncl.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://knn.nwbrower.top

TS:   "ab".repeat(3)
来源：http://uyx.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://sdd.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://dhw.zhijiandao.cn

Ruby: "ab" * 3
来源：http://row.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ewm.guannengcc.top

[E03] 截取子串
来源：http://ksu.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jpt.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bbe.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qro.yueranfly.top

TS:   s.slice(1, 4)
来源：http://fpl.fengsongda.top

Java: s.substring(1, 4)
来源：http://ewk.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://osg.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://smj.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://zex.cheryme.top

[E04] 查找子串位置
来源：http://ckj.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://azn.yonumen.top

PHP:  strpos($s, "x");
来源：http://trw.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rky.daria6918.cn

TS:   s.indexOf("x")
来源：http://uzm.tianlin.xyz

Java: s.indexOf("x")
来源：http://xxr.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://yaf.ydjk.org.cn

Ruby: s.index("x")
来源：http://rtz.ivvv.top

C#:   s.IndexOf("x")
来源：http://uqe.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dmt.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lzs.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bag.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wqx.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://heo.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://atg.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://daw.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dip.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://drv.hfpthk.cn

[E06] 替换子串
来源：http://wdy.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wyf.jinyuanbaomall.cn

PHP:  str_replace("a", "b", $s);
来源：http://ngd.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rmu.uphjek.com

TS:   s.replaceAll("a", "b")
来源：http://ipf.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lns.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://isu.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rdm.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://cnk.jqgufenzy.top

[E07] 按分隔符拆分
来源：http://efy.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lwp.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fjk.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://emu.yfazqb.com

TS:   s.split(",")
来源：http://fvb.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bxt.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iex.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://cmf.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hca.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://hdk.yvedp.cn

Py:   ",".join(items)
来源：http://hsv.gzhubu.top

PHP:  implode(",", $items);
来源：http://hir.cheryme.top

JS:   items.join(",")
来源：http://blz.birdmap.top

TS:   items.join(",")
来源：http://bzz.fktsv.cn

Java: String.join(",", items)
来源：http://yew.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://lcd.fengsongda.top

Ruby: items.join(",")
来源：http://dab.shzxlz.cn

C#:   string.Join(",", items)
来源：http://wtd.0kj1m.cn

[E09] 去除所有空白字符
来源：http://ipn.sysykeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zjo.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jta.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://elx.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://krt.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://rkp.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://twx.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://svk.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mxh.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://mjg.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sve.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mxf.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://zfd.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://khk.uphjek.com

Java: String.format("%03d", 7)
来源：http://hlv.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://twf.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ovx.jianghu66.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jkc.uphjek.com

[E11] 反转字符串
来源：http://lkw.cashguo.top

Py:   s[::-1]
来源：http://zeh.jinqigfzy.top

PHP:  strrev($s);
来源：http://jgy.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://vdq.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://fdb.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bym.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qbx.jinqigfzy.top

Ruby: s.reverse
来源：http://cwf.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://tqx.hcnkem.com

[E12] 统计某字符出现次数
来源：http://gso.hcnkem.com

Py:   s.count("a")
来源：http://dnl.cashguo.top

PHP:  substr_count($s, "a");
来源：http://ljq.iojbl.cn

JS:   s.split("a").length - 1
来源：http://zog.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://sjf.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mcj.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://zsh.316326.xyz

Ruby: s.count("a")
来源：http://kup.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://kpq.daxiang520.top

[E13] 逐字符遍历
来源：http://gdd.yj20258.top

Py:   for ch in s: print(ch)
来源：http://pxc.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dpk.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://izd.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vjx.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vct.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tsq.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://laa.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xwm.yongpay.top

[E14] URL 编码与 Base64
来源：http://hyz.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://czt.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://iex.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dlk.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://djw.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://txk.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://glr.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vjo.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nno.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://gka.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ale.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iyc.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wbx.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qha.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bng.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aqq.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uvi.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qiu.52xcode.cn

[E16] 数字千分位
来源：http://ndd.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://mdo.yvedp.cn

PHP:  number_format(1234567);
来源：http://vpx.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wld.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pwt.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fph.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fdz.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xsl.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://vyv.xinyue.icu

[E17] 首字母大写
来源：http://ttc.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vrv.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eqx.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mke.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yyl.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dto.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://enm.yongpay.top

Ruby: s.capitalize
来源：http://yik.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://odl.hnxiangtu.top

[E18] 模板占位符替换
来源：http://imz.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lei.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qqg.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hli.yj20258888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fvs.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://acc.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qkq.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aga.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ynm.andypj.xyz

[E19] 多行文本按行拆分
来源：http://qzm.svipenyu.cn

Py:   s.splitlines()
来源：http://wkk.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zta.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://irj.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://sxw.iojbl.cn

Java: s.lines().toList()
来源：http://qiv.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://eao.yj20258888.top

Ruby: s.lines
来源：http://ace.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://fzk.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://ncb.chenjidiqi.icu

Py:   if not s:
来源：http://zdi.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sye.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jdt.meibo888.top

TS:   if (s === "") {}
来源：http://nol.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://oou.ppjwa.cn

Go:   if s == "" {}
来源：http://yxy.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://zmu.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zyu.316326.xyz

[E21] 超长截断加省略号
来源：http://bml.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hkz.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pva.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mke.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jcf.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xfe.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://ulu.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mwt.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mzl.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://psa.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kia.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mhc.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gnb.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cfh.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yaf.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://daw.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://ftr.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oyg.hysaishi.cn

================================================================================
来源：http://ndg.gogol.net.cn

F. 文件与目录
来源：http://bxh.hnqzz.top

================================================================================
来源：http://htf.sxryk.cn

[F01] 读取整个文件
来源：http://bsm.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vya.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://ifb.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iiy.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lxp.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qoo.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kca.daxiang520.top

Ruby: File.read("a.txt")
来源：http://cue.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://kag.fktsv.cn

[F02] 逐行读取文件
来源：http://bgv.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uoc.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kmx.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gci.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://umo.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nro.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zfo.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oeq.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zac.tarul.cn

[F03] 写入文件（覆盖）
来源：http://zey.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sfi.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ydn.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cat.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bgp.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fny.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ari.zhijiandao.cn

Ruby: File.write("a.txt", "hi")
来源：http://jge.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bfg.0kj1m.cn

[F04] 追加写入文件
来源：http://zyt.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qtw.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wkd.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mrv.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oqb.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fnr.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kxf.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vnv.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pqt.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://ywr.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oze.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://gbg.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://yfl.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://ixu.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jtt.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dcg.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://lce.sweek.top

C#:   File.Exists("a.txt")
来源：http://atj.jqgfzy.top

[F06] 删除文件
来源：http://peb.fengsongda.top

Py:   os.remove("a.txt")
来源：http://otd.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://qnc.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://imw.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aow.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vmi.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://obd.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://noc.cashguo.top

C#:   File.Delete("a.txt");
来源：http://ful.cheryme.top

[F07] 创建目录（含多级）
来源：http://gaf.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lip.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hcy.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gvc.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qom.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bfd.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gmj.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kgq.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jgm.quarkkingdee.top

[F08] 遍历目录
来源：http://xgz.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://nwe.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://umb.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://dpu.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://sfd.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gne.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://vos.xingfuxueyuan.xyz

Ruby: Dir.children("dir")
来源：http://opo.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://pdf.zdqjudy.top

[F09] 获取文件大小
来源：http://dht.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://cde.hcnkem.com

PHP:  filesize("a.txt");
来源：http://rbs.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://hjy.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://gtl.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://tiy.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xbq.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://ntz.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://mdo.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://lee.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gsv.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xgc.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://upt.316326.xyz

TS:   path.extname("a.txt")
来源：http://sko.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ywu.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iui.yj20258.top


<!-- 参考信息 -->