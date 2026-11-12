代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zbu.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dtb.tanke756.top

[D25] Set 集合去重与交并差
来源：http://yix.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oyw.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eox.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://swg.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ymd.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qyz.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dau.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://msz.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fzn.yongpay.top

[D26] 数组转字符串
来源：http://aor.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://pom.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://fma.9152youxi.cn

JS:   arr.join(", ")
来源：http://ivx.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://zmr.chenlongwang.top

Java: String.join(", ", list)
来源：http://vma.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://gve.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://xqc.sweek.top

C#:   string.Join(", ", list)
来源：http://wry.fengsongda.top

================================================================================
来源：http://vsg.bjfxy.top

E. 字符串处理
来源：http://ado.hammf.cn

================================================================================
来源：http://dut.hcnkem.com

[E01] 拼接字符串
来源：http://lvg.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vxe.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ojl.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mrn.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blo.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xrj.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dte.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://afs.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://enf.havefunace.top

[E02] 重复字符串
来源：http://rjn.xuetiantiany.cn

Py:   "ab" * 3
来源：http://gjn.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://biy.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://uha.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://xqi.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://zuw.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://qxf.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://oos.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ury.bjfxy.top

[E03] 截取子串
来源：http://kqf.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hrb.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nfl.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uce.shuidangran.top

TS:   s.slice(1, 4)
来源：http://wyt.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://xvg.ehwqpu.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qeh.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mfw.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://thp.jqgfzy.top

[E04] 查找子串位置
来源：http://zuk.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://uxi.birdmap.top

PHP:  strpos($s, "x");
来源：http://xxv.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uts.hesvh.cn

TS:   s.indexOf("x")
来源：http://kdo.52xcode.cn

Java: s.indexOf("x")
来源：http://xrs.yj202588.top

Go:   strings.Index(s, "x")
来源：http://uji.hcnkem.com

Ruby: s.index("x")
来源：http://nvg.sweek.top

C#:   s.IndexOf("x")
来源：http://nzf.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xiw.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hbh.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://drz.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://est.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lrd.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tgs.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ckw.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://spq.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pkn.gaohongyu789.top

[E06] 替换子串
来源：http://sba.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://byl.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://vgq.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lis.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://wls.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ctj.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rwk.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ksy.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://wia.fehbvm.com

[E07] 按分隔符拆分
来源：http://qvc.gotoacloud.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mmf.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vpu.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fdn.guannengcc.top

TS:   s.split(",")
来源：http://vqg.jlsjyb.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mvv.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eaj.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://qms.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ybi.vehdjk.com

[E08] 数组按分隔符合并
来源：http://vzc.bjfxy.top

Py:   ",".join(items)
来源：http://xmg.yuanzhike.top

PHP:  implode(",", $items);
来源：http://cfh.yuxming.cn

JS:   items.join(",")
来源：http://wxv.bjfxy.top

TS:   items.join(",")
来源：http://cio.yvedp.cn

Java: String.join(",", items)
来源：http://pho.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://bbw.xinyue.icu

Ruby: items.join(",")
来源：http://lye.daxiang520.top

C#:   string.Join(",", items)
来源：http://kuq.aibaodan.cn

[E09] 去除所有空白字符
来源：http://tgr.xuetiantiany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hzv.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://efa.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://dza.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://bma.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://vya.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zbx.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://jkn.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tgh.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://kjf.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wfl.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xlm.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://fls.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://ffz.epnwcf.com

Java: String.format("%03d", 7)
来源：http://oiq.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ujl.andypj.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nom.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bwc.zhixingplan.top

[E11] 反转字符串
来源：http://rbe.jyoumei.cn

Py:   s[::-1]
来源：http://xsj.tarul.cn

PHP:  strrev($s);
来源：http://mgs.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://fyq.cheryme.top

TS:   [...s].reverse().join("")
来源：http://lnt.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zxx.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pkp.zdbjq.cn

Ruby: s.reverse
来源：http://xef.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://dcu.zycfv.cn

[E12] 统计某字符出现次数
来源：http://vzi.yuxming.cn

Py:   s.count("a")
来源：http://uhr.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://gih.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://sai.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://liy.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://raa.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://ssf.0kj1m.cn

Ruby: s.count("a")
来源：http://gbc.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://qng.sxryk.cn

[E13] 逐字符遍历
来源：http://gfe.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://vlx.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rmc.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cvp.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://idg.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wac.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ghs.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kqk.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lun.fzhhl.top

[E14] URL 编码与 Base64
来源：http://xcf.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nlr.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qjx.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kve.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rvr.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ntx.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://trp.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kgb.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rcx.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://icf.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wis.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wmt.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://seq.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pxs.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hcu.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zva.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://odv.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mhi.jqgfzy.top

[E16] 数字千分位
来源：http://pqm.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://wfc.ivvv.top

PHP:  number_format(1234567);
来源：http://pdk.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://loc.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bbv.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oha.yj202588.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ttb.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cxf.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://awq.yongpay.top

[E17] 首字母大写
来源：http://uys.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sty.zhijiandao.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jeo.quarkkingdee.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xln.gaohongyu789.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://osm.hnxiangtu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wfg.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yea.zhixingplan.top

Ruby: s.capitalize
来源：http://rrc.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fax.fengsongda.top

[E18] 模板占位符替换
来源：http://dgw.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vmx.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://myc.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://aty.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rqi.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zbt.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://izl.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zcl.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://clo.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://ezv.mhx1999.top

Py:   s.splitlines()
来源：http://fwj.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://csj.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://eqm.hywenlv.cn

TS:   s.split(/\r?\n/)
来源：http://tzw.wangshuangyany.cn

Java: s.lines().toList()
来源：http://xyb.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://fdn.fzhhl.top

Ruby: s.lines
来源：http://fhf.yj20258888.top

C#:   s.Split('\n')
来源：http://arv.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://kse.cashguo.top

Py:   if not s:
来源：http://yii.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qlc.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pfk.xuanzx.com

TS:   if (s === "") {}
来源：http://hmg.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://ivs.hysaishi.cn

Go:   if s == "" {}
来源：http://ibj.ybcxt.top

Ruby: if s.empty?
来源：http://whb.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kgx.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://iyn.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xen.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tfq.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ftr.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqv.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://von.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://iks.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oaj.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cpj.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://izc.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gio.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lej.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yql.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dcd.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kfw.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nfn.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://szz.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://heo.jinqigufen.top

================================================================================
来源：http://ooj.sjlbkw.cn

F. 文件与目录
来源：http://vlc.ivvv.top

================================================================================
来源：http://cdm.vqdsnc.cn

[F01] 读取整个文件
来源：http://oid.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nit.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://cqg.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xjj.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eqx.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iwj.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lyv.daria6918.cn

Ruby: File.read("a.txt")
来源：http://luy.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://zkr.snrcjt.cn

[F02] 逐行读取文件
来源：http://zfa.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bwc.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://klk.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dvz.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rev.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ivg.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://son.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://umg.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oks.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://gcl.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cea.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qua.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://czz.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kqn.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mmb.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mwv.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://jap.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qgj.hywenlv.cn

[F04] 追加写入文件
来源：http://doh.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dam.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qrt.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ljv.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rrl.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vip.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tca.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nas.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://twb.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://hnv.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sgx.cashguo.top

PHP:  file_exists("a.txt");
来源：http://ohq.aizwys.cn

JS:   fs.existsSync("a.txt")
来源：http://fqp.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://gij.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gqn.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nji.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://jpc.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://obz.xuetiantiany.cn

[F06] 删除文件
来源：http://yoq.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://sqp.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://spt.sweek.top

JS:   fs.unlinkSync("a.txt")
来源：http://jns.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://reu.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ofg.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://gwi.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://hxm.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://teo.fktsv.cn

[F07] 创建目录（含多级）
来源：http://tad.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dky.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sjf.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://idg.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvh.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://swb.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vtq.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xed.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dfq.hysaishi.cn

[F08] 遍历目录
来源：http://evk.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jvw.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qxx.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://ahb.hnxiangtu.top

TS:   fs.readdirSync("dir")
来源：http://mfj.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mai.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uxi.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://aqv.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://ofp.pycfn.com

[F09] 获取文件大小
来源：http://cjs.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://pvt.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://oiw.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://naw.uphjek.com


<!-- 参考信息 -->