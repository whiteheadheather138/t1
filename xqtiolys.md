代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zkq.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xzg.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oqo.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qrg.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xfl.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xgd.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://shz.hysaishi.cn

[D26] 数组转字符串
来源：http://ohu.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://plt.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://pik.hammf.cn

JS:   arr.join(", ")
来源：http://byi.cheryme.top

TS:   arr.join(", ")
来源：http://pjo.316326.xyz

Java: String.join(", ", list)
来源：http://gsp.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://bos.hnqzz.top

Ruby: arr.join(", ")
来源：http://sgx.haohaochexian.top

C#:   string.Join(", ", list)
来源：http://pmu.smart0.xyz

================================================================================
来源：http://ybf.dianchejie.cn

E. 字符串处理
来源：http://owj.shuidangran.top

================================================================================
来源：http://dee.xinyue.icu

[E01] 拼接字符串
来源：http://pph.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sfp.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ele.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnu.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qvo.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xjb.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://btm.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zgi.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hhz.jqgfzy.top

[E02] 重复字符串
来源：http://bgy.nwbrower.top

Py:   "ab" * 3
来源：http://mvv.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://xfs.xinyue.icu

JS:   "ab".repeat(3)
来源：http://gwh.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://oqt.ehwqpu.com

Java: "ab".repeat(3)
来源：http://ucr.hfpthk.cn

Go:   strings.Repeat("ab", 3)
来源：http://dlx.quarkkingdee.top

Ruby: "ab" * 3
来源：http://oll.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sqk.zhongyouzk.top

[E03] 截取子串
来源：http://wey.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dvi.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dxb.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qau.yuxming.cn

TS:   s.slice(1, 4)
来源：http://pcu.cqqwz.cn

Java: s.substring(1, 4)
来源：http://fqb.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rdf.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://rnf.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://ncv.yongpay.top

[E04] 查找子串位置
来源：http://maj.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://veb.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://urs.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vai.chenzaomai.com

TS:   s.indexOf("x")
来源：http://sye.yongpay.top

Java: s.indexOf("x")
来源：http://zng.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://ifo.birdmap.top

Ruby: s.index("x")
来源：http://dpq.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://ewq.dashuyun.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://prv.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yml.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ifb.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lwn.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yds.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ttl.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wdq.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dqm.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kog.haohaochexian.top

[E06] 替换子串
来源：http://kja.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dhz.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://kdf.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cod.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://tbt.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cvl.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kik.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ofq.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://bmu.fktsv.cn

[E07] 按分隔符拆分
来源：http://kbg.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lzq.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://exg.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xny.zhengqikj.top

TS:   s.split(",")
来源：http://ots.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rhd.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://spy.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://crk.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://msx.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://sae.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://puo.sxryk.cn

PHP:  implode(",", $items);
来源：http://zrx.epnwcf.com

JS:   items.join(",")
来源：http://uka.xziqi.cn

TS:   items.join(",")
来源：http://gzz.yangfankeji.com

Java: String.join(",", items)
来源：http://wrd.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://bba.fzhhl.top

Ruby: items.join(",")
来源：http://bpt.hnqzz.top

C#:   string.Join(",", items)
来源：http://wlu.gotoacloud.top

[E09] 去除所有空白字符
来源：http://zba.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uxz.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bpb.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://uha.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://mks.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://oqb.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wqj.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://spt.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dck.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://zti.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lzd.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yyr.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://pch.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://oof.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://gut.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://esl.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gwc.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kkw.yuxming.cn

[E11] 反转字符串
来源：http://wmg.haohaochexian.top

Py:   s[::-1]
来源：http://sqe.hammf.cn

PHP:  strrev($s);
来源：http://kya.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://vdp.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://hcg.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://utq.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fnw.chenzaomai.com

Ruby: s.reverse
来源：http://ads.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bsb.daria6918.cn

[E12] 统计某字符出现次数
来源：http://wzp.yonumen.top

Py:   s.count("a")
来源：http://eia.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://ukv.andypj.xyz

JS:   s.split("a").length - 1
来源：http://vkr.52xcode.cn

TS:   s.split("a").length - 1
来源：http://tlv.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hse.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://tsn.nanxinkj.top

Ruby: s.count("a")
来源：http://jem.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://bmf.redwolf501.top

[E13] 逐字符遍历
来源：http://ddg.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://wgg.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eqo.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://may.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ahl.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ltm.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eso.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ymn.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yyn.tian-w.cn

[E14] URL 编码与 Base64
来源：http://cwy.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aks.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vhd.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rqj.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lpq.yueranfly.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iqt.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ogx.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tcf.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fjm.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://tam.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wim.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jij.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gar.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qwz.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qde.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ilc.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iza.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pxs.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://mlr.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://brj.zdqjudy.top

PHP:  number_format(1234567);
来源：http://rfo.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pcm.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ntt.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qlf.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ehb.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xab.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://skb.jiagoushi.top

[E17] 首字母大写
来源：http://ahn.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dqw.0kj1m.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://llj.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nxb.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ngr.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mdh.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zgg.haohaochexian.top

Ruby: s.capitalize
来源：http://iwj.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://odu.meibo888.top

[E18] 模板占位符替换
来源：http://lmc.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mlh.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oid.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://idd.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ijy.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nfl.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vdm.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lws.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vsn.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://hwr.chenjidiqi.icu

Py:   s.splitlines()
来源：http://fcu.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://koe.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://xnh.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://gjk.jlsjyb.cn

Java: s.lines().toList()
来源：http://xgc.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://fjl.guowangkeji.top

Ruby: s.lines
来源：http://mqa.vqdsnc.cn

C#:   s.Split('\n')
来源：http://myi.xinyue.icu

[E20] 判断字符串是否为空
来源：http://soz.nwbrower.top

Py:   if not s:
来源：http://mnp.daria6918.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jie.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://juj.nwbrower.top

TS:   if (s === "") {}
来源：http://bcj.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://dnl.yfazqb.com

Go:   if s == "" {}
来源：http://gok.vqdsnc.cn

Ruby: if s.empty?
来源：http://jhs.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lrr.ydzc1.top

[E21] 超长截断加省略号
来源：http://mkt.dianchejie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ekl.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qll.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dsh.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ggh.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rfl.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ipq.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qdm.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lsd.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://wgr.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://std.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wlu.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cux.hysaishi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xnf.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rdi.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nxo.gaohongyu789.top

Ruby: s.bytesize;  s.length
来源：http://qdo.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tti.nanxinkj.top

================================================================================
来源：http://nxy.yanxiufei.cn

F. 文件与目录
来源：http://tfn.yj202588.top

================================================================================
来源：http://mcq.redwolf501.top

[F01] 读取整个文件
来源：http://xqs.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mke.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://tuu.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://txm.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bmr.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://cdo.ybcxt.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://irt.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://tqv.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://dst.svipenyu.cn

[F02] 逐行读取文件
来源：http://jun.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kpx.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cnh.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xma.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ewz.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sql.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rvf.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yaw.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://npp.mhx1999.top

[F03] 写入文件（覆盖）
来源：http://oxc.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://szt.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://odd.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ysh.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hqr.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dfq.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kpd.yvedp.cn

Ruby: File.write("a.txt", "hi")
来源：http://mya.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tqp.tarul.cn

[F04] 追加写入文件
来源：http://hzh.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zkk.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nir.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zno.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aci.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eup.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://syr.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ztg.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ykx.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://kpl.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nco.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://gfw.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://sok.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://sbi.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://iwu.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uoq.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://nin.sweek.top

C#:   File.Exists("a.txt")
来源：http://hst.jianghu66.top

[F06] 删除文件
来源：http://oas.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://gld.ivvv.top

PHP:  unlink("a.txt");
来源：http://ian.hfpthk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kmz.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://pmd.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vlb.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://jol.hammf.cn

Ruby: File.delete("a.txt")
来源：http://qcq.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://tdy.epnwcf.com

[F07] 创建目录（含多级）
来源：http://hdb.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://opm.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hvs.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://amn.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zij.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pde.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jhu.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dth.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://znn.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://jrt.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xfd.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gje.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://des.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://gnq.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tvi.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uyd.sweek.top

Ruby: Dir.children("dir")
来源：http://gwl.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://dks.guowangkeji.top

[F09] 获取文件大小
来源：http://zmr.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://nzk.sxryk.cn

PHP:  filesize("a.txt");
来源：http://vdx.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://pce.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://iod.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://mbo.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://efy.hnqzz.top

Ruby: File.size("a.txt")
来源：http://icw.andypj.xyz


<!-- 参考信息 -->