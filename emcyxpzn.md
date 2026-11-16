代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ycq.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://knh.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://snp.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nri.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://foy.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bof.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://znd.yangfankeji.com

[D26] 数组转字符串
来源：http://uyc.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://umh.ivvv.top

PHP:  implode(", ", $arr);
来源：http://qqc.yvedp.cn

JS:   arr.join(", ")
来源：http://sam.birdmap.top

TS:   arr.join(", ")
来源：http://khj.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://rhk.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://ddt.chenzaomai.com

Ruby: arr.join(", ")
来源：http://rof.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://omg.daria6918.cn

================================================================================
来源：http://tdo.redwolf501.top

E. 字符串处理
来源：http://zct.svipenyu.cn

================================================================================
来源：http://fyl.jqgufenzy.top

[E01] 拼接字符串
来源：http://rga.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tzt.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://erm.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqn.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vfk.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lfr.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wfo.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kto.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gcw.yangfankeji.com

[E02] 重复字符串
来源：http://lti.cheryme.top

Py:   "ab" * 3
来源：http://hxt.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://hvr.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://zvy.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://jrx.yangfankeji.com

Java: "ab".repeat(3)
来源：http://uqg.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://xsv.fehbvm.com

Ruby: "ab" * 3
来源：http://ueh.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jsh.gotoacloud.top

[E03] 截取子串
来源：http://lxj.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dsw.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ylf.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wrx.zdqjudy.top

TS:   s.slice(1, 4)
来源：http://whb.cheryme.top

Java: s.substring(1, 4)
来源：http://spe.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://liw.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://mkx.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://zkg.0kj1m.cn

[E04] 查找子串位置
来源：http://zzy.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://ymy.uphjek.com

PHP:  strpos($s, "x");
来源：http://ust.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yyn.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://tyk.c1oappe.top

Java: s.indexOf("x")
来源：http://vns.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://vdi.quarkkingdee.top

Ruby: s.index("x")
来源：http://zji.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://tjf.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://szq.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jry.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hic.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lcn.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kfg.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zia.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dgw.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sxu.meibo888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ehf.chenjidiqi.icu

[E06] 替换子串
来源：http://fem.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qss.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://dnn.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eqd.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://qib.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gby.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ygx.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://del.tanke756.top

C#:   s.Replace("a", "b")
来源：http://frk.daxiang520.top

[E07] 按分隔符拆分
来源：http://otz.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vrz.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lgh.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://vvp.zhixingplan.top

TS:   s.split(",")
来源：http://gyq.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://qiw.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sra.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://yxg.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mmd.aizwys.cn

[E08] 数组按分隔符合并
来源：http://asx.yfazqb.com

Py:   ",".join(items)
来源：http://wap.9152youxi.cn

PHP:  implode(",", $items);
来源：http://idv.epnwcf.com

JS:   items.join(",")
来源：http://rjt.ivvv.top

TS:   items.join(",")
来源：http://sux.havefunace.top

Java: String.join(",", items)
来源：http://vta.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://adg.dashuyun.cn

Ruby: items.join(",")
来源：http://ltj.daria6918.cn

C#:   string.Join(",", items)
来源：http://bma.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://zfk.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iaa.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vvg.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://lsj.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://tmr.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://iut.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zct.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mpe.hfpthk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zwl.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://ghv.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pif.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://obe.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://dfa.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://rdv.fehbvm.com

Java: String.format("%03d", 7)
来源：http://pok.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://gog.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://foe.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cle.bjfxy.top

[E11] 反转字符串
来源：http://mux.fengsongda.top

Py:   s[::-1]
来源：http://tdb.316326.xyz

PHP:  strrev($s);
来源：http://bsv.meibo888.top

JS:   [...s].reverse().join("")
来源：http://quz.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://slj.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://txp.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vro.dashuyun.cn

Ruby: s.reverse
来源：http://lng.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://fwd.yj202588.top

[E12] 统计某字符出现次数
来源：http://vzo.wangshuangyany.cn

Py:   s.count("a")
来源：http://axg.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://ujm.cashguo.top

JS:   s.split("a").length - 1
来源：http://axa.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://shx.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ivw.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://ejv.fengsongda.top

Ruby: s.count("a")
来源：http://xxu.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://otr.redwolf501.top

[E13] 逐字符遍历
来源：http://szd.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://mxa.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uqo.kuanghao11.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gkg.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tca.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lzs.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xvo.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ulj.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cry.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://zhd.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oed.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://cvx.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dim.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hel.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qlv.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kej.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lkb.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bdx.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://cxv.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qhr.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uvc.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://slx.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xqu.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://koz.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rct.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uhh.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hwq.sjlbkw.cn

[E16] 数字千分位
来源：http://une.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://esj.yonumen.top

PHP:  number_format(1234567);
来源：http://wbp.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zes.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wqs.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gjj.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qid.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zlx.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://amz.chenzaomai.com

[E17] 首字母大写
来源：http://ikf.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qsx.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mwp.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rpg.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kis.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qol.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gsh.ybcxt.top

Ruby: s.capitalize
来源：http://yqb.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mju.yuanzhike.top

[E18] 模板占位符替换
来源：http://mql.ywan-chungtsiang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fss.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nil.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nya.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xdh.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wqa.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dyg.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hgj.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uxi.hnqzz.top

[E19] 多行文本按行拆分
来源：http://oie.zdbjq.cn

Py:   s.splitlines()
来源：http://nyl.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tmn.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://nvy.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://kqb.yanxiufei.cn

Java: s.lines().toList()
来源：http://vjk.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://mea.gogol.net.cn

Ruby: s.lines
来源：http://jux.daria6918.cn

C#:   s.Split('\n')
来源：http://alb.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://zfg.fktsv.cn

Py:   if not s:
来源：http://hii.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vzh.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://crk.jianghu66.top

TS:   if (s === "") {}
来源：http://wsm.sxryk.cn

Java: if (s.isEmpty()) {}
来源：http://iob.uphjek.com

Go:   if s == "" {}
来源：http://bnz.zycfv.cn

Ruby: if s.empty?
来源：http://wfd.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bpw.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://jwo.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qiy.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://klu.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hky.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vpt.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qiz.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://zqk.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://doy.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ize.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://rsi.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qsq.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pjn.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nlr.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://skl.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rmf.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iha.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://rum.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hhj.gzhubu.top

================================================================================
来源：http://nmb.hesvh.cn

F. 文件与目录
来源：http://ihg.ydzc1.top

================================================================================
来源：http://qkk.jianghu66.top

[F01] 读取整个文件
来源：http://jud.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ejv.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://xid.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ygs.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cns.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ljs.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nvk.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://lui.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://wyz.ivvv.top

[F02] 逐行读取文件
来源：http://czc.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jhd.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ldy.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ajp.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cqr.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ytr.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ftq.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lgh.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yco.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://fhu.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sue.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jzd.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xae.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://owy.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pet.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aqx.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://fpb.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://txg.ppjwa.cn

[F04] 追加写入文件
来源：http://rvn.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gpm.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fol.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://asz.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qas.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bwv.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hhn.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iwf.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yhd.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://ued.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gmc.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://ruo.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://aou.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://est.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://bpv.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vet.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://syg.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://yqd.zhaomingkeji.xyz

[F06] 删除文件
来源：http://ocw.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://hew.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://tqx.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://naj.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://enl.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ejp.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://tpt.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://jyo.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://xdn.xziqi.cn

[F07] 创建目录（含多级）
来源：http://dvu.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zqx.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fzb.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mkx.epnwcf.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzn.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vhk.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lwa.sysykeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dtf.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mtj.yfazqb.com

[F08] 遍历目录
来源：http://fjm.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oho.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lat.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://rri.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://twv.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wfs.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vae.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://gxo.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://atj.gotoacloud.top

[F09] 获取文件大小
来源：http://kzv.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://bri.cashguo.top

PHP:  filesize("a.txt");
来源：http://upx.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://ivu.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://uuy.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://ssu.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jug.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://ckt.yanxiufei.cn


<!-- 参考信息 -->