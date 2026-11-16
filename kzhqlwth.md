代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://apz.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mwj.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://utj.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ydd.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hog.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mdk.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nye.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wad.sufxvd.cn

[E02] 重复字符串
来源：http://jvw.andypj.xyz

Py:   "ab" * 3
来源：http://rat.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://xps.bbcook.cn

JS:   "ab".repeat(3)
来源：http://zfl.guannengcc.top

TS:   "ab".repeat(3)
来源：http://onz.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://ojp.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://mqz.shzxlz.cn

Ruby: "ab" * 3
来源：http://bdx.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eai.bbcook.cn

[E03] 截取子串
来源：http://afc.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://irs.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qal.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://toi.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://cnz.svipenyu.cn

Java: s.substring(1, 4)
来源：http://iaz.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ahe.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://uld.pycfn.com

C#:   s.Substring(1, 3)
来源：http://fhm.epnwcf.com

[E04] 查找子串位置
来源：http://afs.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://kaf.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://zar.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://skn.tianlin.xyz

TS:   s.indexOf("x")
来源：http://div.52xcode.cn

Java: s.indexOf("x")
来源：http://kkq.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://fvu.9152youxi.cn

Ruby: s.index("x")
来源：http://qzm.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://qbr.hywenlv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cqd.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xdy.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://krh.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cuv.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://osu.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ulf.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pqy.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dmo.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dzl.birdmap.top

[E06] 替换子串
来源：http://oxt.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ggk.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://mrd.yanxiufei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pqm.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://hka.yongpay.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zbg.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oit.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pmr.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://kxc.havefunace.top

[E07] 按分隔符拆分
来源：http://iqv.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qsp.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cqg.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ral.smart0.xyz

TS:   s.split(",")
来源：http://sxu.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://pig.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kmy.xuetiantiany.cn

Ruby: s.split(",");  s.split
来源：http://gvp.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nxw.bjfxy.top

[E08] 数组按分隔符合并
来源：http://kur.chenzaomai.com

Py:   ",".join(items)
来源：http://zib.tian-w.cn

PHP:  implode(",", $items);
来源：http://quw.yuanzhike.top

JS:   items.join(",")
来源：http://vil.hnqzz.top

TS:   items.join(",")
来源：http://ahl.xziqi.cn

Java: String.join(",", items)
来源：http://hmv.316326.xyz

Go:   strings.Join(items, ",")
来源：http://gsy.cqqwz.cn

Ruby: items.join(",")
来源：http://bet.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://ets.zdbjq.cn

[E09] 去除所有空白字符
来源：http://vxc.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zdu.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tme.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://nmn.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://sqp.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://qjc.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vsw.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://xsp.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mpm.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://tjy.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tvm.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rdz.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://qxc.shzxlz.cn

TS:   "7".padStart(3, "0")
来源：http://syn.tanke756.top

Java: String.format("%03d", 7)
来源：http://yoq.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bzb.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://edi.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yup.ydjk.org.cn

[E11] 反转字符串
来源：http://fzg.yj20258888.top

Py:   s[::-1]
来源：http://jcp.ctjpmb.com

PHP:  strrev($s);
来源：http://gzg.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://fhp.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://cwa.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fue.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xqd.jqgufenzy.top

Ruby: s.reverse
来源：http://ihc.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mrs.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://vhr.zhengqikj.top

Py:   s.count("a")
来源：http://yjn.cheryme.top

PHP:  substr_count($s, "a");
来源：http://stw.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://eaa.yongpay.top

TS:   s.split("a").length - 1
来源：http://ylq.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fwl.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://ryn.cqqwz.cn

Ruby: s.count("a")
来源：http://ljr.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://cqo.jiagoushi.top

[E13] 逐字符遍历
来源：http://txs.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://luh.daxiang520.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hua.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tor.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hkq.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://saj.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gpl.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nxw.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vew.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://vrt.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://quj.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://exn.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xtn.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://izs.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tev.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nfg.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fdx.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pdi.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://hft.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bgx.ppjwa.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yjq.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oox.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://edl.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://myb.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jnh.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://whm.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nul.gzhubu.top

[E16] 数字千分位
来源：http://tjq.xinyue.icu

Py:   f"{1234567:,}"
来源：http://ovw.sxryk.cn

PHP:  number_format(1234567);
来源：http://vmd.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tek.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vte.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cln.guowangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fey.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iuu.havefunace.top

C#:   1234567.ToString("N0")
来源：http://drv.jqgfzy.top

[E17] 首字母大写
来源：http://vtn.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tlp.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pnc.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sfm.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwp.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iym.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://otz.mhx1999.top

Ruby: s.capitalize
来源：http://ezb.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kca.fehbvm.com

[E18] 模板占位符替换
来源：http://zam.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zqp.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oje.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qar.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qon.gogol.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ehp.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://htp.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vnb.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hcx.meibo888.top

[E19] 多行文本按行拆分
来源：http://ini.hesvh.cn

Py:   s.splitlines()
来源：http://llr.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://udy.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://ngr.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://lro.dianchejie.cn

Java: s.lines().toList()
来源：http://iaz.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://yzz.yfazqb.com

Ruby: s.lines
来源：http://iih.redwolf501.top

C#:   s.Split('\n')
来源：http://mjk.pycfn.com

[E20] 判断字符串是否为空
来源：http://pdt.nanxuanxn.top

Py:   if not s:
来源：http://ers.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xzk.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rfz.xuanzx.com

TS:   if (s === "") {}
来源：http://xnc.zhiwuduotai.top

Java: if (s.isEmpty()) {}
来源：http://kgf.jqgufenzy.top

Go:   if s == "" {}
来源：http://hny.wangdashe.top

Ruby: if s.empty?
来源：http://rkq.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mmo.redwolf501.top

[E21] 超长截断加省略号
来源：http://vfn.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bqf.yuxming.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jmc.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tfm.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blk.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jww.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://vqm.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vvd.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jai.yfazqb.com

[E22] 字节长度与字符长度
来源：http://jnz.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pil.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xxj.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jkp.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cqc.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://thl.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qwz.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://ymb.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pso.fanxiaobao.xyz

================================================================================
来源：http://yne.shuidangran.top

F. 文件与目录
来源：http://sze.ybcxt.top

================================================================================
来源：http://oih.ydzc1.top

[F01] 读取整个文件
来源：http://oxv.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ayt.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://uoe.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://env.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pav.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pbd.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bek.gzhubu.top

Ruby: File.read("a.txt")
来源：http://rpz.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://mbs.bbcook.cn

[F02] 逐行读取文件
来源：http://hlv.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wiu.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kgb.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rac.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://olb.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sps.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qfx.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://akm.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://htu.chenlongwang.top

[F03] 写入文件（覆盖）
来源：http://uuq.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fqk.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://iof.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xnn.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://flm.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://woz.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mdz.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://lof.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eev.zhixingplan.top

[F04] 追加写入文件
来源：http://wua.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ljv.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nfy.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xhg.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fce.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ebb.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vgb.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qid.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nha.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://kfn.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bbn.yongpay.top

PHP:  file_exists("a.txt");
来源：http://uau.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://lzy.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://qmj.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yzb.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fmt.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://vsw.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://qow.shuidangran.top

[F06] 删除文件
来源：http://hbm.birdmap.top

Py:   os.remove("a.txt")
来源：http://owj.hfpthk.cn

PHP:  unlink("a.txt");
来源：http://xje.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hir.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://zvi.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xfp.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://inh.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://qxk.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://oaf.tanke756.top

[F07] 创建目录（含多级）
来源：http://ada.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mtl.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ons.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivz.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vyw.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ctz.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://guk.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://psp.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://stw.yj20258888.top

[F08] 遍历目录
来源：http://bav.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cxn.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://guj.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://ujc.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://qxb.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nbj.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qcp.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://rij.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://gga.sxryk.cn

[F09] 获取文件大小
来源：http://ikv.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://rck.tanke756.top

PHP:  filesize("a.txt");
来源：http://ibs.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://vxp.haohaochexian.top

TS:   fs.statSync("a.txt").size
来源：http://ytd.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://hls.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jes.c1oappe.top

Ruby: File.size("a.txt")
来源：http://cea.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://lom.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://lrc.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jjd.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://esy.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jka.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://rif.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ezg.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ygk.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lfi.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nvk.fehbvm.com

[F11] 复制与移动文件
来源：http://rec.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://amo.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://suj.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://etj.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hwa.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uqv.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mdn.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://otq.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xck.tian-w.cn

[F12] CSV 读写
来源：http://cln.jinyuanbaomall.cn


<!-- 参考信息 -->