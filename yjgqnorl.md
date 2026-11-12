代发 wailian999

[E02] 重复字符串
来源：http://cel.xuanzx.com

Py:   "ab" * 3
来源：http://wln.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://rih.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://rny.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://guw.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://dnv.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://gkj.yongpay.top

Ruby: "ab" * 3
来源：http://ljk.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pmw.guannengcc.top

[E03] 截取子串
来源：http://aka.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://onv.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uas.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gbk.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://zsr.yueranfly.top

Java: s.substring(1, 4)
来源：http://hap.chenlongwang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://akk.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ybq.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://rpv.mhx1999.top

[E04] 查找子串位置
来源：http://xwl.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://qfj.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://qmt.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://prc.chenzaomai.com

TS:   s.indexOf("x")
来源：http://lvv.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://rce.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://fkv.redwolf501.top

Ruby: s.index("x")
来源：http://wjz.316326.xyz

C#:   s.IndexOf("x")
来源：http://nvz.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://spt.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dxt.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://etz.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lrk.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://fjb.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vvi.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xcp.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://evz.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nrf.zhoulong.xyz

[E06] 替换子串
来源：http://dqi.zhoulong.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pmz.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://uci.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wpy.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://dej.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mnq.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ucx.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qei.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://xeh.daxiang520.top

[E07] 按分隔符拆分
来源：http://esg.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ooc.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nlj.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://stz.meibo888.top

TS:   s.split(",")
来源：http://jvi.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yos.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ycf.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://edo.jqgufenzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wqp.xinyue.icu

[E08] 数组按分隔符合并
来源：http://tob.ehwqpu.com

Py:   ",".join(items)
来源：http://apo.fehbvm.com

PHP:  implode(",", $items);
来源：http://zfu.yvedp.cn

JS:   items.join(",")
来源：http://gyg.tarul.cn

TS:   items.join(",")
来源：http://ils.guowangkeji.top

Java: String.join(",", items)
来源：http://hjf.yj20258.top

Go:   strings.Join(items, ",")
来源：http://kva.dianchejie.cn

Ruby: items.join(",")
来源：http://lhk.hywenlv.cn

C#:   string.Join(",", items)
来源：http://ior.yueranfly.top

[E09] 去除所有空白字符
来源：http://xmt.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zpb.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://byz.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://cvr.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://anq.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://afz.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gxm.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://loq.fengsongda.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sef.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://rqh.snrcjt.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qnf.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oul.zhengqikj.top

JS:   "7".padStart(3, "0")
来源：http://uua.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://ddw.jianghu66.top

Java: String.format("%03d", 7)
来源：http://emz.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pue.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bhc.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sfz.andypj.xyz

[E11] 反转字符串
来源：http://xem.yueranfly.top

Py:   s[::-1]
来源：http://iki.tanke756.top

PHP:  strrev($s);
来源：http://fig.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://uvm.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://dyv.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tcr.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://suu.zhijiandao.cn

Ruby: s.reverse
来源：http://emm.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lxy.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://fdr.tanke756.top

Py:   s.count("a")
来源：http://xeb.hammf.cn

PHP:  substr_count($s, "a");
来源：http://atc.yj202588.top

JS:   s.split("a").length - 1
来源：http://ahu.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://myq.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://phg.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://spj.cashguo.top

Ruby: s.count("a")
来源：http://wdp.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://rtn.shzxlz.cn

[E13] 逐字符遍历
来源：http://nof.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://grv.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fjt.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uhc.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ewg.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qpn.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://irx.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ncr.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dqb.tian-w.cn

[E14] URL 编码与 Base64
来源：http://fzm.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gis.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yux.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pvl.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kxg.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://owq.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baj.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tfr.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ejv.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://lke.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://thb.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://axg.feifeiyinyue.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cva.jianghu66.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qyj.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://epk.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pwe.cqqwz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mbu.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://erj.xylfe.cn

[E16] 数字千分位
来源：http://nwq.tarul.cn

Py:   f"{1234567:,}"
来源：http://jcp.tarul.cn

PHP:  number_format(1234567);
来源：http://tmg.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ylb.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://slt.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://adr.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ihh.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lrf.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://umk.snrcjt.cn

[E17] 首字母大写
来源：http://qjb.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jep.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cng.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://swi.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kvx.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ocz.snrcjt.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://adx.yj20258888.top

Ruby: s.capitalize
来源：http://mhu.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mog.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://bqy.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hqm.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cri.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gcn.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://pdn.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://csj.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cfa.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gxw.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hld.yvedp.cn

[E19] 多行文本按行拆分
来源：http://sla.hnxiangtu.top

Py:   s.splitlines()
来源：http://xec.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gti.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://bbz.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://fqo.cqqwz.cn

Java: s.lines().toList()
来源：http://tde.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://toe.uphjek.com

Ruby: s.lines
来源：http://qyz.c1oappe.top

C#:   s.Split('\n')
来源：http://jzs.wangdashe.top

[E20] 判断字符串是否为空
来源：http://ctr.mhx1999.top

Py:   if not s:
来源：http://zvh.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lij.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zcy.tanke756.top

TS:   if (s === "") {}
来源：http://ykf.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://rcl.vehdjk.com

Go:   if s == "" {}
来源：http://qka.sysykeji.top

Ruby: if s.empty?
来源：http://eok.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ztz.bjfxy.top

[E21] 超长截断加省略号
来源：http://map.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bfq.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rye.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hid.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ucw.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vjb.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://glm.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jcj.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bkm.fzhhl.top

[E22] 字节长度与字符长度
来源：http://wow.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tdi.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ekd.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://afm.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vdb.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cua.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mci.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://nmb.tian-w.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hgo.tanke756.top

================================================================================
来源：http://hyf.vqdsnc.cn

F. 文件与目录
来源：http://qvl.dashuyun.cn

================================================================================
来源：http://akz.zdbjq.cn

[F01] 读取整个文件
来源：http://owa.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://acf.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://vlk.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wfj.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://skk.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rnj.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wjj.nwbrower.top

Ruby: File.read("a.txt")
来源：http://ktg.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://nqd.jyoumei.cn

[F02] 逐行读取文件
来源：http://wzw.vqdsnc.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ysq.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tts.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://keq.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywb.hammf.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vsh.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xak.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fce.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vtm.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://udd.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yew.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wkj.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wuh.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bbl.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vru.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qgn.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://gax.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tbm.daria6918.cn

[F04] 追加写入文件
来源：http://nlp.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zif.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ivp.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lfc.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dsm.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://srr.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qcf.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qzx.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zin.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://rro.xuetiantiany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cju.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://xxn.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://ezt.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://cjt.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://azd.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zgh.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://sbg.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://gsw.ybcxt.top

[F06] 删除文件
来源：http://aam.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://rjo.fengsongda.top

PHP:  unlink("a.txt");
来源：http://sfb.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pki.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jbo.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xom.guowangkeji.top

Go:   os.Remove("a.txt")
来源：http://yit.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://znw.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://scb.wangdashe.top

[F07] 创建目录（含多级）
来源：http://waa.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sdc.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://djg.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgt.ctjpmb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://axf.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ete.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vkw.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://crj.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nvw.yvedp.cn

[F08] 遍历目录
来源：http://hpm.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eny.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vpp.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://bqk.hnxiangtu.top

TS:   fs.readdirSync("dir")
来源：http://eao.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xbw.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://jak.cucudq.cn

Ruby: Dir.children("dir")
来源：http://wms.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://ptw.feifeiyinyue.top

[F09] 获取文件大小
来源：http://kro.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://qqq.havefunace.top

PHP:  filesize("a.txt");
来源：http://ffw.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://umq.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://fld.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://wwc.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vew.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://pve.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://kib.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://plu.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uii.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tif.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pvm.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://ajz.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xkl.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qxx.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://adx.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://orm.nanxinkj.top

[F11] 复制与移动文件
来源：http://qns.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wra.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qil.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gff.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kbs.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lpk.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rwe.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kmr.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jhd.shanyushiyangtech.top

[F12] CSV 读写
来源：http://zmi.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ffv.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lpd.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uxy.nwbrower.top

TS:   // 同上
来源：http://wgm.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rbc.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fcr.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hny.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nqt.yuanzhike.top


<!-- 参考信息 -->