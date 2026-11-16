代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ljq.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://awm.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://etx.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ezo.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vws.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xjg.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://orm.chenlongwang.top

[D26] 数组转字符串
来源：http://wzl.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://xic.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://vhh.yvedp.cn

JS:   arr.join(", ")
来源：http://yjg.tarul.cn

TS:   arr.join(", ")
来源：http://lol.chenlongwang.top

Java: String.join(", ", list)
来源：http://sma.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://yez.xziqi.cn

Ruby: arr.join(", ")
来源：http://zai.sysykeji.top

C#:   string.Join(", ", list)
来源：http://fqw.yvedp.cn

================================================================================
来源：http://cjl.shuidangran.top

E. 字符串处理
来源：http://ief.yj20258888.top

================================================================================
来源：http://kku.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://aew.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qqw.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qiz.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dlb.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ctm.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://whh.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://udd.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zei.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gne.yangfankeji.com

[E02] 重复字符串
来源：http://bow.quarkkingdee.top

Py:   "ab" * 3
来源：http://fss.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://oiw.tian-w.cn

JS:   "ab".repeat(3)
来源：http://asr.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://ccy.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://vwk.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://kbg.zhoulong.xyz

Ruby: "ab" * 3
来源：http://stp.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ddp.chenjidiqi.icu

[E03] 截取子串
来源：http://dzk.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://abw.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hek.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eez.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://tym.cheryme.top

Java: s.substring(1, 4)
来源：http://ibw.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qoo.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://buf.yj20258.top

C#:   s.Substring(1, 3)
来源：http://hvb.gzhubu.top

[E04] 查找子串位置
来源：http://uve.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://iqv.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://ioq.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wzr.hammf.cn

TS:   s.indexOf("x")
来源：http://vef.52xcode.cn

Java: s.indexOf("x")
来源：http://uhk.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://ria.nanxuanxn.top

Ruby: s.index("x")
来源：http://xiy.aizwys.cn

C#:   s.IndexOf("x")
来源：http://snp.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jrn.tian-w.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://atk.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nws.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bkm.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sis.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://erd.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://apx.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rti.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zqu.shanyushiyangkeji.top

[E06] 替换子串
来源：http://lyd.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uor.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://aao.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kxj.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://isb.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uwl.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mqw.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vjh.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://mfy.jiagoushi.top

[E07] 按分隔符拆分
来源：http://dtw.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fki.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://woy.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iuc.yj20258.top

TS:   s.split(",")
来源：http://iwp.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://ggw.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jqw.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://azn.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ijf.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://nzl.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://nxv.birdmap.top

PHP:  implode(",", $items);
来源：http://dbf.zycfv.cn

JS:   items.join(",")
来源：http://qpn.daria6918.cn

TS:   items.join(",")
来源：http://kuv.zhoulong.xyz

Java: String.join(",", items)
来源：http://zug.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://roe.hfpthk.cn

Ruby: items.join(",")
来源：http://vbw.0kj1m.cn

C#:   string.Join(",", items)
来源：http://gmz.yuxming.cn

[E09] 去除所有空白字符
来源：http://bxi.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tja.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://stt.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://sbz.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://cjy.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://pxp.zhiwuduotai.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://syl.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://yxr.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sux.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://ztu.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aoo.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rvh.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://ktd.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://zmm.mhx1999.top

Java: String.format("%03d", 7)
来源：http://frn.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gsu.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yql.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nap.jiagoushi.top

[E11] 反转字符串
来源：http://ptq.yuanzhike.top

Py:   s[::-1]
来源：http://sic.hywenlv.cn

PHP:  strrev($s);
来源：http://fxk.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://rjt.meibo888.top

TS:   [...s].reverse().join("")
来源：http://awm.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://him.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://wkf.jinghuilouyu.cn

Ruby: s.reverse
来源：http://xqt.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://krc.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://fwd.birdmap.top

Py:   s.count("a")
来源：http://gzt.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://gow.jianghu66.top

JS:   s.split("a").length - 1
来源：http://ztg.xinyue.icu

TS:   s.split("a").length - 1
来源：http://rdf.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ldf.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://xaz.fehbvm.com

Ruby: s.count("a")
来源：http://lqm.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://icw.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://wcv.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://urj.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tya.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://epk.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sxd.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bxs.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://umv.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oee.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sji.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://gzh.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ypk.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gvh.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://icr.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fgw.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wpr.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bpu.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aoq.haohaochexian.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bbf.9152youxi.cn

[E15] HTML 转义 / 反转义
来源：http://kkx.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qfl.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yto.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nms.redwolf501.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uzy.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kjg.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gmr.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wue.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xaj.xuetiantiany.cn

[E16] 数字千分位
来源：http://wia.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://jqz.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://ofu.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kfb.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vmt.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wsj.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bay.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cnf.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://zdd.birdmap.top

[E17] 首字母大写
来源：http://his.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pyn.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hog.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yvm.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://obh.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iec.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rkf.guowangkeji.top

Ruby: s.capitalize
来源：http://ess.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ows.cheryme.top

[E18] 模板占位符替换
来源：http://ypj.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sxy.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aew.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://aar.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://nbd.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cfl.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mea.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yjl.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rgq.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://syj.9152youxi.cn

Py:   s.splitlines()
来源：http://jbf.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nfx.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://qhz.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://suq.uphjek.com

Java: s.lines().toList()
来源：http://ckp.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://mfk.xuanzx.com

Ruby: s.lines
来源：http://pem.nanxuanxn.top

C#:   s.Split('\n')
来源：http://dgq.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://weg.jinqigfzy.top

Py:   if not s:
来源：http://bzn.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qjx.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ckn.gotoacloud.top

TS:   if (s === "") {}
来源：http://kcw.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://aca.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://nbd.haohaochexian.top

Ruby: if s.empty?
来源：http://kzq.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rym.jianghu66.top

[E21] 超长截断加省略号
来源：http://wbk.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cmk.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qpr.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ghl.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gfl.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dky.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://znw.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://toq.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://efz.yonumen.top

[E22] 字节长度与字符长度
来源：http://heq.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wus.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://moe.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wub.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zuk.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://whe.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qzk.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://hwb.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jnq.tianlin.xyz

================================================================================
来源：http://ezh.nanxinkj.top

F. 文件与目录
来源：http://owf.shanyushiyangkeji.top

================================================================================
来源：http://dmg.hywenlv.cn

[F01] 读取整个文件
来源：http://heb.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iwv.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://htn.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qbx.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://spk.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://egy.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ase.bbcook.cn

Ruby: File.read("a.txt")
来源：http://cyh.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://noh.52xcode.cn

[F02] 逐行读取文件
来源：http://brt.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oci.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rol.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yhv.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eer.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://idd.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://npc.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lkn.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tom.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://wzm.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wck.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dis.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jkr.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pmn.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jts.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fxc.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://brw.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pcr.gzhubu.top

[F04] 追加写入文件
来源：http://luf.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fwo.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ucp.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fwl.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jdd.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://maj.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ncu.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ynh.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jkp.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://cns.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uut.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://glx.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://pzb.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://jeg.yvedp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jcm.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tyf.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://ply.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://ewe.wangdashe.top

[F06] 删除文件
来源：http://uww.ydzc1.top

Py:   os.remove("a.txt")
来源：http://zyq.jianghu66.top

PHP:  unlink("a.txt");
来源：http://koh.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://wcn.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://mat.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qxq.meibo888.top

Go:   os.Remove("a.txt")
来源：http://mdz.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://yqo.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://tzv.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://kja.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://otz.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vfk.yongpay.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vuh.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qad.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hwu.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vmx.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kcm.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mke.dashuyun.cn

[F08] 遍历目录
来源：http://yss.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ilc.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jcm.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://kcx.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://aan.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dcn.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jbj.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://drs.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://hts.cheryme.top

[F09] 获取文件大小
来源：http://uaz.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://ohr.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://mrt.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://fsz.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://jxl.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://guh.jinqigufen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gar.yfazqb.com

Ruby: File.size("a.txt")
来源：http://kbu.pengpengdd.cyou


<!-- 参考信息 -->