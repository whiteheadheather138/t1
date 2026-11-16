代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gpj.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pon.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rap.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://ews.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://bap.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://aqz.jianghu66.top

JS:   arr.join(", ")
来源：http://zhm.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://bde.yj20258888.top

Java: String.join(", ", list)
来源：http://hkt.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://bef.iojbl.cn

Ruby: arr.join(", ")
来源：http://dus.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://hkh.zycfv.cn

================================================================================
来源：http://snx.wangshuangyany.cn

E. 字符串处理
来源：http://vvg.jinyuanbaomall.cn

================================================================================
来源：http://jih.xinyue.icu

[E01] 拼接字符串
来源：http://ifn.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kan.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://est.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mdq.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tlx.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zni.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://leo.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gpt.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://len.zhengqikj.top

[E02] 重复字符串
来源：http://rui.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://ykb.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://nin.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://fip.wangdashe.top

TS:   "ab".repeat(3)
来源：http://rtt.jianghu66.top

Java: "ab".repeat(3)
来源：http://wqc.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://mkt.snrcjt.cn

Ruby: "ab" * 3
来源：http://nmg.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ksu.vqdsnc.cn

[E03] 截取子串
来源：http://has.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hgy.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rsp.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gpl.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://owj.ppjwa.cn

Java: s.substring(1, 4)
来源：http://jgf.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uhs.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mxj.hammf.cn

C#:   s.Substring(1, 3)
来源：http://tdw.sjlbkw.cn

[E04] 查找子串位置
来源：http://def.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://emk.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://htr.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jbb.cdnleiting.top

TS:   s.indexOf("x")
来源：http://obd.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://cff.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://nvt.hammf.cn

Ruby: s.index("x")
来源：http://hfs.xylfe.cn

C#:   s.IndexOf("x")
来源：http://ugd.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dut.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mta.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wsx.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mhd.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nnf.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jcq.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gzh.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xup.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://koh.meibo888.top

[E06] 替换子串
来源：http://pcl.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nlr.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://wdz.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ppi.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://vji.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fjx.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qot.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ffk.cqqwz.cn

C#:   s.Replace("a", "b")
来源：http://lin.dashuyun.cn

[E07] 按分隔符拆分
来源：http://lvq.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qcm.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xtd.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ism.nwbrower.top

TS:   s.split(",")
来源：http://sfw.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://bnx.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://buj.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://asb.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bqg.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://vri.ehwqpu.com

Py:   ",".join(items)
来源：http://tls.yongpay.top

PHP:  implode(",", $items);
来源：http://ycr.guowangkeji.top

JS:   items.join(",")
来源：http://gxe.haohaochexian.top

TS:   items.join(",")
来源：http://bst.gogol.net.cn

Java: String.join(",", items)
来源：http://emk.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://grg.jqgufenzy.top

Ruby: items.join(",")
来源：http://aro.sufxvd.cn

C#:   string.Join(",", items)
来源：http://zxm.zdbjq.cn

[E09] 去除所有空白字符
来源：http://bav.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vri.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://brb.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://jrk.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://sbm.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ufv.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rlq.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://pje.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wbl.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://ikb.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://owu.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gok.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://hyr.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://oxw.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://uqi.cdnleiting.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wcg.andypj.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://enp.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sdc.smart0.xyz

[E11] 反转字符串
来源：http://nwz.mhx1999.top

Py:   s[::-1]
来源：http://tvf.xylfe.cn

PHP:  strrev($s);
来源：http://zje.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://unl.meibo888.top

TS:   [...s].reverse().join("")
来源：http://owo.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ljq.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oft.gaohongyu789.top

Ruby: s.reverse
来源：http://rss.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://dwi.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://yge.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://dzn.yonumen.top

PHP:  substr_count($s, "a");
来源：http://kui.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://ibu.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://cpi.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yfh.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://ryf.wangshuangyany.cn

Ruby: s.count("a")
来源：http://abf.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://csw.yj20258888.top

[E13] 逐字符遍历
来源：http://abm.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://cbt.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rag.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ylr.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kua.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yzg.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rqr.cdnleiting.top

Ruby: s.each_char { |ch| puts ch }
来源：http://igh.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wui.tian-w.cn

[E14] URL 编码与 Base64
来源：http://xsw.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uqd.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://knk.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qed.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iiq.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ylc.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://okb.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://shg.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yzm.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://ufi.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tsz.xylfe.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jsc.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jdt.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://jbp.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iaf.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tdm.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://afj.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mnl.jinghuilouyu.cn

[E16] 数字千分位
来源：http://wrf.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://qxe.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://jnl.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yzb.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eqv.vehdjk.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tfj.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sdd.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fet.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://xsy.0kj1m.cn

[E17] 首字母大写
来源：http://mnw.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cco.ivvv.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vwd.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kyv.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fqf.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xak.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://its.yonumen.top

Ruby: s.capitalize
来源：http://wgd.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://juw.zdqjudy.top

[E18] 模板占位符替换
来源：http://ozd.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tlf.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://koy.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://rlx.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mbd.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tyq.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gue.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yxe.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tkf.daxiang520.top

[E19] 多行文本按行拆分
来源：http://eon.yueranfly.top

Py:   s.splitlines()
来源：http://qdj.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://opm.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://rhl.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://pfn.zhijiandao.cn

Java: s.lines().toList()
来源：http://ija.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://dsv.hesvh.cn

Ruby: s.lines
来源：http://nft.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://rqg.fengsongda.top

[E20] 判断字符串是否为空
来源：http://ixh.jinqigfzy.top

Py:   if not s:
来源：http://kaf.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cff.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mia.yfazqb.com

TS:   if (s === "") {}
来源：http://zft.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://fgv.quarkkingdee.top

Go:   if s == "" {}
来源：http://wac.xuanzx.com

Ruby: if s.empty?
来源：http://frz.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://buw.hysaishi.cn

[E21] 超长截断加省略号
来源：http://yeg.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rtt.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bki.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ggc.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gcj.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cjl.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://vfv.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uxj.chenzaomai.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sep.xinyue.icu

[E22] 字节长度与字符长度
来源：http://itw.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eww.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wye.xziqi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ray.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqz.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kkt.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sxr.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://lcv.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://klu.zdbjq.cn

================================================================================
来源：http://ttc.9152youxi.cn

F. 文件与目录
来源：http://xeu.316326.xyz

================================================================================
来源：http://vyu.smart0.xyz

[F01] 读取整个文件
来源：http://vcl.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dxp.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://vpl.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qhf.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tnu.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lky.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://man.shuidangran.top

Ruby: File.read("a.txt")
来源：http://dwm.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://onl.shuidangran.top

[F02] 逐行读取文件
来源：http://kxs.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cdx.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dmj.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yol.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://drg.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zqa.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vgr.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lok.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://vxq.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gis.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://snu.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zqt.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zvq.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hzv.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ygs.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://gdn.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dnp.gotoacloud.top

[F04] 追加写入文件
来源：http://pih.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jhv.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rwq.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wwf.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://chm.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bqd.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://als.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uky.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wbv.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://ccx.jinyuanbaomall.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gje.xuanzx.com

PHP:  file_exists("a.txt");
来源：http://yed.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://gor.fehbvm.com

TS:   fs.existsSync("a.txt")
来源：http://rzv.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pwg.aizwys.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://epr.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://vfu.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://tmb.dashuyun.cn

[F06] 删除文件
来源：http://thu.sysykeji.top

Py:   os.remove("a.txt")
来源：http://vsw.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://ruu.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://uoi.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://dsh.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rdt.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://qmr.jianghu66.top

Ruby: File.delete("a.txt")
来源：http://iky.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://yvy.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://prk.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jir.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nlz.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iko.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xza.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yda.andypj.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bjh.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://awd.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wvv.jlsjyb.cn

[F08] 遍历目录
来源：http://mvz.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mxx.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lor.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://pmf.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://xbn.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xij.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://alm.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://pzp.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://jnm.aizwys.cn

[F09] 获取文件大小
来源：http://abu.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://yeu.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://kki.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://dmk.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://pcf.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://hwb.xziqi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bxc.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://dyc.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://wdi.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://yhg.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cmh.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mws.ivvv.top


<!-- 参考信息 -->