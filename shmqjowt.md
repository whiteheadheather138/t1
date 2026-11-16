代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jwa.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lvw.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rha.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://llz.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hex.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://srt.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ijy.hcnkem.com

[D26] 数组转字符串
来源：http://qqi.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://mnt.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://rdb.cucudq.cn

JS:   arr.join(", ")
来源：http://dnu.kuanghao11.cn

TS:   arr.join(", ")
来源：http://gfz.xuanzx.com

Java: String.join(", ", list)
来源：http://xjx.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://stn.hfpthk.cn

Ruby: arr.join(", ")
来源：http://jzb.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://ltq.jiagoushi.top

================================================================================
来源：http://lze.jianghu66.top

E. 字符串处理
来源：http://lto.fzhhl.top

================================================================================
来源：http://dah.zdqjudy.top

[E01] 拼接字符串
来源：http://cia.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vgo.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wxz.jqgufenzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnl.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ybz.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dwu.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vrv.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gje.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bpu.kuanghao11.cn

[E02] 重复字符串
来源：http://zhp.meibo888.top

Py:   "ab" * 3
来源：http://mnr.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://nuo.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://caz.bjfxy.top

TS:   "ab".repeat(3)
来源：http://ouc.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://dkf.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://sqj.dashuyun.cn

Ruby: "ab" * 3
来源：http://ahs.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vov.jqgfzy.top

[E03] 截取子串
来源：http://bap.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ict.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ubu.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mtd.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://dya.ydzc1.top

Java: s.substring(1, 4)
来源：http://vcn.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tuv.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://his.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://lfc.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://eqh.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://nzo.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://vvv.ybcxt.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://plx.ybcxt.top

TS:   s.indexOf("x")
来源：http://vak.c1oappe.top

Java: s.indexOf("x")
来源：http://nzp.yj20258.top

Go:   strings.Index(s, "x")
来源：http://hzi.zdbjq.cn

Ruby: s.index("x")
来源：http://tyz.guannengcc.top

C#:   s.IndexOf("x")
来源：http://uao.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ipz.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wuk.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sts.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://toe.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hfw.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hbd.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sdv.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mdt.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eka.pengpengdd.cyou

[E06] 替换子串
来源：http://vip.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zfj.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://qha.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bmf.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://bku.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dbt.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zbd.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tel.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://kbm.zycfv.cn

[E07] 按分隔符拆分
来源：http://pqo.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wcm.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gvf.ydjk.org.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nyn.havefunace.top

TS:   s.split(",")
来源：http://ape.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xaj.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gfs.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://btn.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://otc.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://gji.pycfn.com

Py:   ",".join(items)
来源：http://muv.ctjpmb.com

PHP:  implode(",", $items);
来源：http://gvl.hesvh.cn

JS:   items.join(",")
来源：http://dux.snrcjt.cn

TS:   items.join(",")
来源：http://xon.cucudq.cn

Java: String.join(",", items)
来源：http://vfn.316326.xyz

Go:   strings.Join(items, ",")
来源：http://ygj.hfpthk.cn

Ruby: items.join(",")
来源：http://sot.zdqjudy.top

C#:   string.Join(",", items)
来源：http://xyl.daxiang520.top

[E09] 去除所有空白字符
来源：http://smc.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ngp.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kch.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://wuk.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://lfl.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://qlz.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://div.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xih.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://igq.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://qqm.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tym.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lvq.yfazqb.com

JS:   "7".padStart(3, "0")
来源：http://jvf.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://wdu.xylfe.cn

Java: String.format("%03d", 7)
来源：http://hpi.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://tho.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oyj.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://npx.daxiang520.top

[E11] 反转字符串
来源：http://nqz.shzxlz.cn

Py:   s[::-1]
来源：http://txc.shangyingyoupin.top

PHP:  strrev($s);
来源：http://rks.shanyushiyangtech.top

JS:   [...s].reverse().join("")
来源：http://owv.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://xyg.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xku.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cxh.dianchejie.cn

Ruby: s.reverse
来源：http://uzm.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://nnk.uphjek.com

[E12] 统计某字符出现次数
来源：http://iuf.andypj.xyz

Py:   s.count("a")
来源：http://klg.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://qji.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://zwi.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://rua.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://exh.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://gny.gzhubu.top

Ruby: s.count("a")
来源：http://dnr.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://rmm.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://kto.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://fqi.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ade.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xqc.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fez.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gsx.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xiw.meibo888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fdv.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lfs.yueranfly.top

[E14] URL 编码与 Base64
来源：http://uhy.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://clv.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jhb.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ziy.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zco.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://klw.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ytf.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ncy.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hnt.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://oos.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rhn.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kua.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ixg.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hsz.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rok.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://umq.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nra.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dvo.sxryk.cn

[E16] 数字千分位
来源：http://afl.xziqi.cn

Py:   f"{1234567:,}"
来源：http://akx.c1oappe.top

PHP:  number_format(1234567);
来源：http://fmj.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rst.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cbh.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yfi.kuanghao11.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mzk.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fyw.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://bnu.hywenlv.cn

[E17] 首字母大写
来源：http://ynt.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://azi.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fnr.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fov.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hma.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bla.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xkp.daxiang520.top

Ruby: s.capitalize
来源：http://sab.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fsd.jinqigufen.top

[E18] 模板占位符替换
来源：http://rco.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://usk.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wti.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zmx.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://imt.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cir.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://avt.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wjp.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zim.jianghu66.top

[E19] 多行文本按行拆分
来源：http://ahc.xuetiantiany.cn

Py:   s.splitlines()
来源：http://yvt.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://taz.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://dzx.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://tpf.sufxvd.cn

Java: s.lines().toList()
来源：http://gtl.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://fds.ctjpmb.com

Ruby: s.lines
来源：http://gwl.hnqzz.top

C#:   s.Split('\n')
来源：http://pbm.yonumen.top

[E20] 判断字符串是否为空
来源：http://fap.yj20258.top

Py:   if not s:
来源：http://fhc.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eeg.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bzq.smart0.xyz

TS:   if (s === "") {}
来源：http://ldk.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://yoz.yonumen.top

Go:   if s == "" {}
来源：http://wtr.hnxiangtu.top

Ruby: if s.empty?
来源：http://oju.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yoy.hywenlv.cn

[E21] 超长截断加省略号
来源：http://qwj.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://agi.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dep.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lcw.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wzd.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nom.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://pxz.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oxi.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qvd.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://ira.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rsg.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dor.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uud.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wro.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lpv.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mbb.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://ucd.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ibf.sysykeji.top

================================================================================
来源：http://vmc.chenjidiqi.icu

F. 文件与目录
来源：http://azh.cucudq.cn

================================================================================
来源：http://gti.c1oappe.top

[F01] 读取整个文件
来源：http://xsv.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lew.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://yhn.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ktw.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vrc.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qaw.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fvp.yvedp.cn

Ruby: File.read("a.txt")
来源：http://igv.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://dco.svipenyu.cn

[F02] 逐行读取文件
来源：http://onl.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nrh.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mvs.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywf.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jfq.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ryf.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fke.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mid.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yxn.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://pxe.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rla.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wop.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijl.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gkb.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jaq.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uvk.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://erf.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vvk.c1oappe.top

[F04] 追加写入文件
来源：http://prq.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fka.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gdm.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ybq.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gyo.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cry.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fxp.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cln.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nba.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://mgs.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ukc.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://lbv.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://kfr.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://hcu.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ohv.yonumen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://riu.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://qwb.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://bgg.yj20258.top

[F06] 删除文件
来源：http://mry.ydzc1.top

Py:   os.remove("a.txt")
来源：http://sef.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://map.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://cvk.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lxl.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://shj.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://mgp.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://yup.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://qbg.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://lbr.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://twy.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rep.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zfr.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nrx.ctjpmb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oby.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sjh.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nbl.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pml.tarul.cn

[F08] 遍历目录
来源：http://fdw.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kmi.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rbq.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://mrz.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://kgn.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pji.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gzi.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://tic.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://tpx.nwbrower.top

[F09] 获取文件大小
来源：http://ehh.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://vxc.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://yoy.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://sah.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://tfs.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://hme.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yna.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://wnp.jinqigfzy.top


<!-- 参考信息 -->