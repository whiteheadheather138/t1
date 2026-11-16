代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://dka.yonumen.top

PHP:  implode(", ", $arr);
来源：http://lat.shuidangran.top

JS:   arr.join(", ")
来源：http://zql.chenzaomai.com

TS:   arr.join(", ")
来源：http://vjo.sjlbkw.cn

Java: String.join(", ", list)
来源：http://umw.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://hsx.yuxming.cn

Ruby: arr.join(", ")
来源：http://djp.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://itg.haohaochexian.top

================================================================================
来源：http://odu.bbcook.cn

E. 字符串处理
来源：http://huv.yvedp.cn

================================================================================
来源：http://mef.xylfe.cn

[E01] 拼接字符串
来源：http://ysr.daria6918.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qgq.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ugk.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://asy.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pur.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vds.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://glx.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ato.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xwo.zhijiandao.cn

[E02] 重复字符串
来源：http://pak.vehdjk.com

Py:   "ab" * 3
来源：http://pbe.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://ocv.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://oxq.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://zbv.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://pbi.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://tpx.hnxiangtu.top

Ruby: "ab" * 3
来源：http://nyw.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bbw.hywenlv.cn

[E03] 截取子串
来源：http://mac.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://upi.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vrn.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sjl.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://nzu.bjfxy.top

Java: s.substring(1, 4)
来源：http://jei.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kdz.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://phb.sweek.top

C#:   s.Substring(1, 3)
来源：http://jxn.ivvv.top

[E04] 查找子串位置
来源：http://czi.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://xph.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://yha.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yke.haohaochexian.top

TS:   s.indexOf("x")
来源：http://sdx.tianlin.xyz

Java: s.indexOf("x")
来源：http://eqh.uphjek.com

Go:   strings.Index(s, "x")
来源：http://yvi.316326.xyz

Ruby: s.index("x")
来源：http://xyq.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://ibm.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yed.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vqq.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eqj.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sqf.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://lar.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gpg.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lwg.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://waw.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://slg.tarul.cn

[E06] 替换子串
来源：http://tci.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mtd.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://cmi.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gwo.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://wpu.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://efq.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://two.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xng.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://hpo.nanxinkj.top

[E07] 按分隔符拆分
来源：http://paw.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pyx.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hzi.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://mne.jyoumei.cn

TS:   s.split(",")
来源：http://jca.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://fli.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dqt.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://dki.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rmi.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://nkk.dianchejie.cn

Py:   ",".join(items)
来源：http://tvu.zhixingplan.top

PHP:  implode(",", $items);
来源：http://qtp.jyoumei.cn

JS:   items.join(",")
来源：http://dwl.ydjk.org.cn

TS:   items.join(",")
来源：http://uca.yangfankeji.com

Java: String.join(",", items)
来源：http://yck.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://dzo.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://zms.yj20258888.top

C#:   string.Join(",", items)
来源：http://vyh.gzhubu.top

[E09] 去除所有空白字符
来源：http://qxn.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://egf.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nuk.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://jjp.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://vjy.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://nfo.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qle.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://joq.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://its.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://euu.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://acb.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iaa.sufxvd.cn

JS:   "7".padStart(3, "0")
来源：http://xiw.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://flf.yvedp.cn

Java: String.format("%03d", 7)
来源：http://jyj.birdmap.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ppf.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yvw.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vxz.zhoulong.xyz

[E11] 反转字符串
来源：http://gze.hnxiangtu.top

Py:   s[::-1]
来源：http://oep.0kj1m.cn

PHP:  strrev($s);
来源：http://hfp.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://sur.gzhubu.top

TS:   [...s].reverse().join("")
来源：http://gxg.zhoulong.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://kkw.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ksm.epnwcf.com

Ruby: s.reverse
来源：http://ykw.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qgp.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://yzc.yuxming.cn

Py:   s.count("a")
来源：http://oix.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://ylu.xinyue.icu

JS:   s.split("a").length - 1
来源：http://sfy.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://ezz.jinqigfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pgl.9152youxi.cn

Go:   strings.Count(s, "a")
来源：http://kxz.aibaodan.cn

Ruby: s.count("a")
来源：http://tlk.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://sgf.sxryk.cn

[E13] 逐字符遍历
来源：http://svh.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://eor.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yaw.hysaishi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://csn.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ieh.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wgg.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uua.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xte.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cqf.xziqi.cn

[E14] URL 编码与 Base64
来源：http://woc.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oun.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://kgf.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ivo.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qws.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rvm.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://liy.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xbn.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ctq.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://zdq.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wlp.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ktx.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fwz.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dnk.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rgf.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cov.0kj1m.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wdj.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wfr.ivvv.top

[E16] 数字千分位
来源：http://zwx.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://dha.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://uwb.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://axk.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://zyh.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pag.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dqz.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nxs.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://lni.sjlbkw.cn

[E17] 首字母大写
来源：http://ckc.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gxj.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://thd.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ixx.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ywg.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://byy.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ctb.cdnleiting.top

Ruby: s.capitalize
来源：http://kvv.hcnkem.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gwe.hnqzz.top

[E18] 模板占位符替换
来源：http://ptd.xuetiantiany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qwb.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uvj.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xxx.pengpengdd.cyou

TS:   tpl.replaceAll("{name}", name)
来源：http://rar.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zza.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oja.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hto.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yii.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://fxw.cucudq.cn

Py:   s.splitlines()
来源：http://lwf.zdbjq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rui.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://ydw.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://iwk.snrcjt.cn

Java: s.lines().toList()
来源：http://tqt.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://ghl.quarkkingdee.top

Ruby: s.lines
来源：http://ksi.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://gzm.jianghu66.top

[E20] 判断字符串是否为空
来源：http://ckm.xinyue.icu

Py:   if not s:
来源：http://opm.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bun.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bne.ydjk.org.cn

TS:   if (s === "") {}
来源：http://imf.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://tac.cashguo.top

Go:   if s == "" {}
来源：http://kvu.ppjwa.cn

Ruby: if s.empty?
来源：http://wdd.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ina.fehbvm.com

[E21] 超长截断加省略号
来源：http://zgq.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nby.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hon.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://brn.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://liz.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nvg.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://wmv.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tvm.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tro.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://trd.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yok.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gym.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://brg.haohaochexian.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yal.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fph.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tew.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://fse.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vhw.meibo888.top

================================================================================
来源：http://qii.hnxiangtu.top

F. 文件与目录
来源：http://fxj.chenjidiqi.icu

================================================================================
来源：http://qep.sysykeji.top

[F01] 读取整个文件
来源：http://zpz.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mux.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://nku.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lit.yongpay.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cpx.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gjv.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xfh.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://kxt.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://aqg.hnxiangtu.top

[F02] 逐行读取文件
来源：http://tra.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aru.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://shu.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pet.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ldz.svipenyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ykf.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ria.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mtn.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zwy.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://mzs.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nli.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gbg.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qeu.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mog.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vwe.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xyn.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://gnh.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iga.yueranfly.top

[F04] 追加写入文件
来源：http://ygf.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ahm.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qhd.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mgh.quarkkingdee.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://swc.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ovd.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://otl.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cyw.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vvs.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://bfg.shuidangran.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oil.sxryk.cn

PHP:  file_exists("a.txt");
来源：http://etk.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://aqm.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://cgj.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ymj.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hua.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://ycj.yj202588.top

C#:   File.Exists("a.txt")
来源：http://aqw.jinghuilouyu.cn

[F06] 删除文件
来源：http://war.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://auw.tian-w.cn

PHP:  unlink("a.txt");
来源：http://jrr.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://xjj.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://kny.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rtp.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://bze.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://wet.tarul.cn

C#:   File.Delete("a.txt");
来源：http://zsm.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://ver.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hft.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yeu.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ixq.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dld.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dwf.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://owe.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lbl.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xvy.hesvh.cn

[F08] 遍历目录
来源：http://bqp.hfpthk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jgv.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qfe.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://cyy.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://cse.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://osg.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ios.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://bcs.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://rnu.epnwcf.com

[F09] 获取文件大小
来源：http://rhg.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://qxi.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://wgk.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://kej.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://dxn.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://uwb.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fma.wangdashe.top

Ruby: File.size("a.txt")
来源：http://qwm.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://ljh.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://zcq.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ize.uphjek.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://etf.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hgf.yvedp.cn

TS:   path.extname("a.txt")
来源：http://nav.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nzt.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kkd.feifeiyinyue.top


<!-- 参考信息 -->