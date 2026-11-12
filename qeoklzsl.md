代发 wailian999

Java: String.join(", ", list)
来源：http://aqm.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://lzs.jqgfzy.top

Ruby: arr.join(", ")
来源：http://xze.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://hxl.hesvh.cn

================================================================================
来源：http://aob.smart0.xyz

E. 字符串处理
来源：http://edg.fzhhl.top

================================================================================
来源：http://kir.chenlongwang.top

[E01] 拼接字符串
来源：http://ide.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uvx.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iov.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ary.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zkr.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gxv.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nav.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fjh.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ggl.52xcode.cn

[E02] 重复字符串
来源：http://egc.nanxuanxn.top

Py:   "ab" * 3
来源：http://jfe.jinqigfzy.top

PHP:  str_repeat("ab", 3);
来源：http://dxx.yj20258888.top

JS:   "ab".repeat(3)
来源：http://wvk.nwbrower.top

TS:   "ab".repeat(3)
来源：http://qeb.hcnkem.com

Java: "ab".repeat(3)
来源：http://fiq.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://gmw.tanke756.top

Ruby: "ab" * 3
来源：http://mky.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uyc.nwbrower.top

[E03] 截取子串
来源：http://dfr.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pkq.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qth.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fzg.pycfn.com

TS:   s.slice(1, 4)
来源：http://ozz.gaohongyu789.top

Java: s.substring(1, 4)
来源：http://ebg.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://znk.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://nkr.pycfn.com

C#:   s.Substring(1, 3)
来源：http://ftw.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://hnd.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://pob.zhixingplan.top

PHP:  strpos($s, "x");
来源：http://mzo.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kml.meibo888.top

TS:   s.indexOf("x")
来源：http://zer.tian-w.cn

Java: s.indexOf("x")
来源：http://luj.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://msw.gaohongyu789.top

Ruby: s.index("x")
来源：http://ogp.xziqi.cn

C#:   s.IndexOf("x")
来源：http://zza.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iit.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xcc.tarul.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rpv.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://drc.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://dpz.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qbm.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ync.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vpq.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iyj.smart0.xyz

[E06] 替换子串
来源：http://vjq.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xii.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://jko.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wze.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://vyu.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eli.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zzw.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ozs.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://ggq.shuidangran.top

[E07] 按分隔符拆分
来源：http://yuw.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pbw.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yir.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ugm.shangyingyoupin.top

TS:   s.split(",")
来源：http://gso.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://nkx.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ggc.yonumen.top

Ruby: s.split(",");  s.split
来源：http://zgs.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zcs.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://hcr.guowangkeji.top

Py:   ",".join(items)
来源：http://ijb.hammf.cn

PHP:  implode(",", $items);
来源：http://tme.hywenlv.cn

JS:   items.join(",")
来源：http://owp.cheryme.top

TS:   items.join(",")
来源：http://ggw.yj20258888.top

Java: String.join(",", items)
来源：http://xdk.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://lgs.jinqigufen.top

Ruby: items.join(",")
来源：http://yij.sweek.top

C#:   string.Join(",", items)
来源：http://pkz.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://hoc.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fbb.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kso.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://fig.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://gig.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://qmv.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ciq.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://sya.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cmg.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://wdj.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mup.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zdw.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://rdf.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://rnu.uphjek.com

Java: String.format("%03d", 7)
来源：http://lnh.fzhhl.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lsp.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pao.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mjy.jqgufenzy.top

[E11] 反转字符串
来源：http://jfd.hammf.cn

Py:   s[::-1]
来源：http://slr.yanxiufei.cn

PHP:  strrev($s);
来源：http://knn.tanke756.top

JS:   [...s].reverse().join("")
来源：http://oym.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://hup.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://izy.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://oet.jqgufenzy.top

Ruby: s.reverse
来源：http://cod.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ggs.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://wsc.jianghu66.top

Py:   s.count("a")
来源：http://nir.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://ixs.sweek.top

JS:   s.split("a").length - 1
来源：http://jnr.yongpay.top

TS:   s.split("a").length - 1
来源：http://caz.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gjz.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://uea.jinqigufen.top

Ruby: s.count("a")
来源：http://fds.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://trj.daxiang520.top

[E13] 逐字符遍历
来源：http://hav.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://wnl.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uis.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mfv.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://daz.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bmb.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gmm.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://byw.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://thm.cashguo.top

[E14] URL 编码与 Base64
来源：http://ccy.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ykk.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tqm.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kvf.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://orc.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lfy.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tzp.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ome.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hdy.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://juv.dianchejie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wgl.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hzm.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rlp.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://rtj.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ipi.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qef.jinqigfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zdf.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ril.yueranfly.top

[E16] 数字千分位
来源：http://zsp.birdmap.top

Py:   f"{1234567:,}"
来源：http://xzf.nwbrower.top

PHP:  number_format(1234567);
来源：http://lzl.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mae.jinyuanbaomall.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://klg.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://krz.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jhy.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xgz.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://vkm.yj20258.top

[E17] 首字母大写
来源：http://jdf.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://irf.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lum.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hao.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jxn.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bdg.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xvh.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://zhc.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://epp.yueranfly.top

[E18] 模板占位符替换
来源：http://xup.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qin.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rgq.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xnn.svipenyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://znh.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jmr.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yzd.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uex.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jhn.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://wgh.hnxiangtu.top

Py:   s.splitlines()
来源：http://oec.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gwx.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://oya.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://bvd.haohaochexian.top

Java: s.lines().toList()
来源：http://uui.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://djk.hcnkem.com

Ruby: s.lines
来源：http://ale.hnqzz.top

C#:   s.Split('\n')
来源：http://ggg.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://elu.gogol.net.cn

Py:   if not s:
来源：http://ryd.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hsd.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mpb.hysaishi.cn

TS:   if (s === "") {}
来源：http://foc.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://ecj.yanxiufei.cn

Go:   if s == "" {}
来源：http://vzf.zycfv.cn

Ruby: if s.empty?
来源：http://rdk.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hdj.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://cjb.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cak.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qvy.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://crl.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sij.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gfz.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://jmt.jyoumei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tcl.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://muc.yj20258.top

[E22] 字节长度与字符长度
来源：http://ysl.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jss.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mds.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mju.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ydq.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yuf.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zup.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://acl.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://auo.fzhhl.top

================================================================================
来源：http://nbq.guowangkeji.top

F. 文件与目录
来源：http://beq.gaohongyu789.top

================================================================================
来源：http://hbx.ydjk.org.cn

[F01] 读取整个文件
来源：http://iro.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lgz.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://fuc.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cau.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mww.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://wzm.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jqn.snrcjt.cn

Ruby: File.read("a.txt")
来源：http://xrr.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://ywj.nanxuanxn.top

[F02] 逐行读取文件
来源：http://fnj.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ckl.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wxi.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qzz.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ccy.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uex.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rjf.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ice.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eeh.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://ljb.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zpj.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://eyp.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kts.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uom.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wzs.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dus.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://mdw.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nju.guowangkeji.top

[F04] 追加写入文件
来源：http://vyk.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tkn.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dno.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cgc.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pxr.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mir.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iba.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uxf.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://roe.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://sdu.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vbv.uphjek.com

PHP:  file_exists("a.txt");
来源：http://ybs.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://ijf.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://sik.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jdc.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vcl.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://oka.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://iho.xinyue.icu

[F06] 删除文件
来源：http://yfr.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://pyq.ivvv.top

PHP:  unlink("a.txt");
来源：http://dfh.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yje.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://knv.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://anq.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://opl.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://lkq.yonumen.top

C#:   File.Delete("a.txt");
来源：http://zkt.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://ffn.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tyq.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jgl.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dxs.guannengcc.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://erz.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hes.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lzb.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ybg.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ezu.sweek.top

[F08] 遍历目录
来源：http://vsh.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gsj.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://enn.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://oib.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://syj.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fhe.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wch.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://uhk.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://frv.daxiang520.top

[F09] 获取文件大小
来源：http://msd.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://wtg.sxryk.cn

PHP:  filesize("a.txt");
来源：http://hhe.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://vyr.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://zxu.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://dyi.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://too.zycfv.cn

Ruby: File.size("a.txt")
来源：http://cjt.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://gne.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://ltm.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://duf.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jol.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://abl.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://bzg.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zgw.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fjy.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dau.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://svk.smart0.xyz

[F11] 复制与移动文件
来源：http://pbm.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hlf.zhaomingkeji.xyz


<!-- 参考信息 -->