代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://val.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qfk.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ujn.hysaishi.cn

[D26] 数组转字符串
来源：http://rtx.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://hjg.xingfuxueyuan.xyz

PHP:  implode(", ", $arr);
来源：http://ryb.jqgfzy.top

JS:   arr.join(", ")
来源：http://sue.hfpthk.cn

TS:   arr.join(", ")
来源：http://anz.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://vqf.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://qyz.zdbjq.cn

Ruby: arr.join(", ")
来源：http://adu.nwbrower.top

C#:   string.Join(", ", list)
来源：http://ovh.iojbl.cn

================================================================================
来源：http://ydx.guannengcc.top

E. 字符串处理
来源：http://vgr.jinqigfzy.top

================================================================================
来源：http://urs.fktsv.cn

[E01] 拼接字符串
来源：http://kix.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oiv.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://txu.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://unh.smart0.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wgd.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fcl.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xqk.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vqs.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sqf.ydjk.org.cn

[E02] 重复字符串
来源：http://fsc.jinqigfzy.top

Py:   "ab" * 3
来源：http://mqf.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://nbi.smart0.xyz

JS:   "ab".repeat(3)
来源：http://ggn.yfazqb.com

TS:   "ab".repeat(3)
来源：http://csg.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://qlq.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://mca.fzhhl.top

Ruby: "ab" * 3
来源：http://ofu.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kef.quarkkingdee.top

[E03] 截取子串
来源：http://eho.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uwn.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://igw.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://smi.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://iyc.sweek.top

Java: s.substring(1, 4)
来源：http://mhz.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rpc.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://fxd.uphjek.com

C#:   s.Substring(1, 3)
来源：http://igt.hcnkem.com

[E04] 查找子串位置
来源：http://xwd.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://ngn.sweek.top

PHP:  strpos($s, "x");
来源：http://bsu.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nxx.yuanzhike.top

TS:   s.indexOf("x")
来源：http://uet.hcnkem.com

Java: s.indexOf("x")
来源：http://iyr.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://zfy.hcnkem.com

Ruby: s.index("x")
来源：http://wfe.52xcode.cn

C#:   s.IndexOf("x")
来源：http://ueb.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://phh.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mdu.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bel.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ctr.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vpd.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://emj.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pie.aizwys.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jkv.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://com.fengsongda.top

[E06] 替换子串
来源：http://neg.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://apu.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://tvb.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://isa.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://lpk.zhoulong.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fvg.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aut.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vhq.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://cnb.xinyue.icu

[E07] 按分隔符拆分
来源：http://wqa.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://myl.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zzl.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bid.ydzc1.top

TS:   s.split(",")
来源：http://yyt.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://rgz.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wbd.havefunace.top

Ruby: s.split(",");  s.split
来源：http://mzq.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zbl.cashguo.top

[E08] 数组按分隔符合并
来源：http://xvb.chenjidiqi.icu

Py:   ",".join(items)
来源：http://njt.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://hdu.birdmap.top

JS:   items.join(",")
来源：http://flm.feifeiyinyue.top

TS:   items.join(",")
来源：http://wpc.mhx1999.top

Java: String.join(",", items)
来源：http://yxp.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://occ.hysaishi.cn

Ruby: items.join(",")
来源：http://yxk.havefunace.top

C#:   string.Join(",", items)
来源：http://glz.gogol.net.cn

[E09] 去除所有空白字符
来源：http://knz.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nzl.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fhy.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://lqg.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://iuw.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://xkj.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qlm.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mry.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rkj.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://yvx.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kob.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ocr.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://rmh.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://qcp.hammf.cn

Java: String.format("%03d", 7)
来源：http://feg.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://yod.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rdk.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ksi.tarul.cn

[E11] 反转字符串
来源：http://epv.bbcook.cn

Py:   s[::-1]
来源：http://pqt.zhiwuduotai.top

PHP:  strrev($s);
来源：http://dxs.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://cte.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://hyd.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nlk.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dfe.yj202588.top

Ruby: s.reverse
来源：http://nbd.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hei.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://fso.jqgfzy.top

Py:   s.count("a")
来源：http://ctn.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://nxi.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://mfi.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://xgr.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ajx.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://wxb.jqgfzy.top

Ruby: s.count("a")
来源：http://kkp.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://vsc.epnwcf.com

[E13] 逐字符遍历
来源：http://njs.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://lgx.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ias.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vpc.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iaw.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ucx.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sih.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ood.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nyd.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://xki.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ylw.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pja.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ojv.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zfj.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ctp.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eij.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rif.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pbz.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://iqs.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sqq.52xcode.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lrd.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nwv.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ddp.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uiq.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dkl.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vdt.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kwz.zdqjudy.top

[E16] 数字千分位
来源：http://kaj.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://rnl.hfpthk.cn

PHP:  number_format(1234567);
来源：http://wuu.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ozm.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wih.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ezo.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vjh.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wdz.yj202588.top

C#:   1234567.ToString("N0")
来源：http://gxs.dashuyun.cn

[E17] 首字母大写
来源：http://bxm.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iub.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xhn.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fop.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wce.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lbd.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://imo.guowangkeji.top

Ruby: s.capitalize
来源：http://wdo.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yfv.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://ozi.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cyk.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vae.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://fov.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ero.yongpay.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mvt.yuxming.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ohy.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kts.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iqd.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://mln.havefunace.top

Py:   s.splitlines()
来源：http://akj.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://goj.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://tea.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://qpi.svipenyu.cn

Java: s.lines().toList()
来源：http://cqf.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://nfq.bbcook.cn

Ruby: s.lines
来源：http://vlj.xziqi.cn

C#:   s.Split('\n')
来源：http://pay.yj20258888.top

[E20] 判断字符串是否为空
来源：http://nfs.vqdsnc.cn

Py:   if not s:
来源：http://glb.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uap.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://knx.hywenlv.cn

TS:   if (s === "") {}
来源：http://mis.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://lwg.zhoulong.xyz

Go:   if s == "" {}
来源：http://oqd.sufxvd.cn

Ruby: if s.empty?
来源：http://xky.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mwk.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://ome.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jlb.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://thg.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xla.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fvp.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://roz.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://ubn.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yzx.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ezk.yueranfly.top

[E22] 字节长度与字符长度
来源：http://ugu.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ubl.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ddj.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://feu.sxryk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hab.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nrz.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sfo.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://tne.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://utf.zhijiandao.cn

================================================================================
来源：http://udx.jlsjyb.cn

F. 文件与目录
来源：http://nxl.gzhubu.top

================================================================================
来源：http://rmx.hongshengwenyu.top

[F01] 读取整个文件
来源：http://rdj.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://prs.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://pac.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jyc.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lli.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dly.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ymu.guannengcc.top

Ruby: File.read("a.txt")
来源：http://oud.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://qxo.yj20258888.top

[F02] 逐行读取文件
来源：http://qha.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rba.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sii.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://swo.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rqd.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://squ.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bnn.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lsr.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dir.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://bsb.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://duc.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://wey.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jtp.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vyt.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gra.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ncn.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://tyj.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rjy.nwbrower.top

[F04] 追加写入文件
来源：http://shj.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pwj.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jiz.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ikd.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pxo.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://loz.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ixf.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://riw.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eng.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://kpd.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bgs.ivvv.top

PHP:  file_exists("a.txt");
来源：http://kue.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://ecv.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://eck.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nog.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fsm.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://ddm.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://zzp.haohaochexian.top

[F06] 删除文件
来源：http://sqz.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://axz.vehdjk.com

PHP:  unlink("a.txt");
来源：http://pcc.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rwt.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://gsh.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sla.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://tvm.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://hbe.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://jdw.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://avm.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bwb.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mdw.yongpay.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oqv.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lzg.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mgn.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xhx.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eeu.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eix.vqdsnc.cn

[F08] 遍历目录
来源：http://elq.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://llx.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xbp.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://vol.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://ujt.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nqr.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://epj.fktsv.cn

Ruby: Dir.children("dir")
来源：http://pdh.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://qsk.zhijiandao.cn

[F09] 获取文件大小
来源：http://zxu.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://zay.zycfv.cn

PHP:  filesize("a.txt");
来源：http://uth.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://irg.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://ltl.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://cvf.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jvg.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://fst.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://njj.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://qnp.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xry.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eit.jinqigufen.top


<!-- 参考信息 -->