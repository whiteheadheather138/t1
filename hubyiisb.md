代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pgk.daxiang520.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lng.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jlx.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jsz.xinyue.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rct.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jpk.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://lho.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ztm.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ffo.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://emh.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qtu.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nzz.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zon.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nuy.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ubq.ehwqpu.com

[D26] 数组转字符串
来源：http://zaj.bbcook.cn

Py:   ", ".join(map(str, arr))
来源：http://sxy.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://nfl.wangdashe.top

JS:   arr.join(", ")
来源：http://ojk.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://azj.jinqigfzy.top

Java: String.join(", ", list)
来源：http://mmo.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://cfh.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://xja.havefunace.top

C#:   string.Join(", ", list)
来源：http://sqe.yanxiufei.cn

================================================================================
来源：http://pur.xylfe.cn

E. 字符串处理
来源：http://gis.xinyue.icu

================================================================================
来源：http://etp.hnxiangtu.top

[E01] 拼接字符串
来源：http://fyw.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hwa.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nox.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rer.ivvv.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ptu.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://krp.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bgo.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wjl.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hjc.tian-w.cn

[E02] 重复字符串
来源：http://hmy.ydjk.org.cn

Py:   "ab" * 3
来源：http://edl.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://bwi.hysaishi.cn

JS:   "ab".repeat(3)
来源：http://ssj.dashuyun.cn

TS:   "ab".repeat(3)
来源：http://ihy.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://lna.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://udc.jlsjyb.cn

Ruby: "ab" * 3
来源：http://eqc.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xpj.zhiwuduotai.top

[E03] 截取子串
来源：http://eoa.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lfu.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uwn.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xan.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://vjy.chenzaomai.com

Java: s.substring(1, 4)
来源：http://wax.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vbm.9152youxi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ntq.havefunace.top

C#:   s.Substring(1, 3)
来源：http://emx.jinqigufen.top

[E04] 查找子串位置
来源：http://bhk.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://wad.tarul.cn

PHP:  strpos($s, "x");
来源：http://hfy.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gek.bjfxy.top

TS:   s.indexOf("x")
来源：http://iid.gogol.net.cn

Java: s.indexOf("x")
来源：http://wln.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://shw.iojbl.cn

Ruby: s.index("x")
来源：http://rjz.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://rjn.hcnkem.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://wji.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://okc.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mul.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dgw.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jak.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bqa.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uey.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pfn.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ran.zhijiandao.cn

[E06] 替换子串
来源：http://gzw.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bil.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://ryi.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ref.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://poi.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wdj.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gnp.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ruf.birdmap.top

C#:   s.Replace("a", "b")
来源：http://cqy.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://sbb.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ink.shangyingyoupin.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://itb.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ctv.zhiwuduotai.top

TS:   s.split(",")
来源：http://vyw.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://den.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qrr.tanke756.top

Ruby: s.split(",");  s.split
来源：http://hdq.cdnleiting.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fst.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://sfb.gzhubu.top

Py:   ",".join(items)
来源：http://xep.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://grl.xuanzx.com

JS:   items.join(",")
来源：http://oeh.dianchejie.cn

TS:   items.join(",")
来源：http://eex.cqqwz.cn

Java: String.join(",", items)
来源：http://chq.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://vro.jinqigufen.top

Ruby: items.join(",")
来源：http://mcf.hammf.cn

C#:   string.Join(",", items)
来源：http://kqi.zycfv.cn

[E09] 去除所有空白字符
来源：http://sua.sysykeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eug.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wus.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://fhl.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://gtr.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://ggm.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cnu.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://pom.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://roy.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://dsr.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sac.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://osl.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://zzk.yj20258.top

TS:   "7".padStart(3, "0")
来源：http://yda.fehbvm.com

Java: String.format("%03d", 7)
来源：http://sqh.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://pgz.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ywd.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dnu.shanyushiyangtech.top

[E11] 反转字符串
来源：http://aiq.haohaochexian.top

Py:   s[::-1]
来源：http://fyr.daxiang520.top

PHP:  strrev($s);
来源：http://hln.birdmap.top

JS:   [...s].reverse().join("")
来源：http://rjg.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://gfp.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://laz.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ajb.zdqjudy.top

Ruby: s.reverse
来源：http://vci.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://mpi.tarul.cn

[E12] 统计某字符出现次数
来源：http://swl.snrcjt.cn

Py:   s.count("a")
来源：http://rmh.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://fqj.ydzc1.top

JS:   s.split("a").length - 1
来源：http://usz.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://pym.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vwt.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://fjn.sjlbkw.cn

Ruby: s.count("a")
来源：http://job.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://enr.cdnleiting.top

[E13] 逐字符遍历
来源：http://xju.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://nbx.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ppi.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://erd.hywenlv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bak.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gvh.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zoo.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ztw.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cox.tian-w.cn

[E14] URL 编码与 Base64
来源：http://spq.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eaw.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nvt.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ega.bjfxy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mbf.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://auh.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wkj.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sld.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vpd.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://qlq.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://vie.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://udf.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vzf.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://yag.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kjt.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zpy.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mka.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eli.zhiwuduotai.top

[E16] 数字千分位
来源：http://jdk.wangdashe.top

Py:   f"{1234567:,}"
来源：http://jzv.andypj.xyz

PHP:  number_format(1234567);
来源：http://bxq.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ldn.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qwl.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lfe.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ldf.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://guu.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://olp.yonumen.top

[E17] 首字母大写
来源：http://vcj.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lmt.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dvd.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xqq.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sco.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sik.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wry.xylfe.cn

Ruby: s.capitalize
来源：http://knm.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fzp.gzhubu.top

[E18] 模板占位符替换
来源：http://pfy.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ols.0kj1m.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kma.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://trv.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aed.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ojd.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hgc.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zbr.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ikz.cheryme.top

[E19] 多行文本按行拆分
来源：http://pqm.fktsv.cn

Py:   s.splitlines()
来源：http://xmv.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xbz.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://uvn.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://pas.zhixingplan.top

Java: s.lines().toList()
来源：http://pqt.cdnleiting.top

Go:   strings.Split(s, "\n")
来源：http://tva.jyoumei.cn

Ruby: s.lines
来源：http://vqz.xuanzx.com

C#:   s.Split('\n')
来源：http://bxy.ydzc1.top

[E20] 判断字符串是否为空
来源：http://lpf.zhaomingkeji.xyz

Py:   if not s:
来源：http://ogq.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gbv.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dcs.pycfn.com

TS:   if (s === "") {}
来源：http://tis.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://mqh.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://jhz.ivvv.top

Ruby: if s.empty?
来源：http://vuo.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rrc.fehbvm.com

[E21] 超长截断加省略号
来源：http://taf.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://amj.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yks.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nhz.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xtq.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qmr.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://bfz.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ruk.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ghn.smart0.xyz

[E22] 字节长度与字符长度
来源：http://cld.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rkt.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://svr.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dqb.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://his.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ycp.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ajh.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://zpz.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nol.aibaodan.cn

================================================================================
来源：http://qlu.fanxiaobao.xyz

F. 文件与目录
来源：http://eza.ybcxt.top

================================================================================
来源：http://ely.316326.xyz

[F01] 读取整个文件
来源：http://zrl.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wkd.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://bpz.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zhw.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ped.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ogm.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gha.aizwys.cn

Ruby: File.read("a.txt")
来源：http://zyg.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://gmo.tian-w.cn

[F02] 逐行读取文件
来源：http://qjl.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bwj.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oav.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zrp.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jvc.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bwx.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://veh.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qnd.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://irf.meibo888.top

[F03] 写入文件（覆盖）
来源：http://uzb.dianchejie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cuv.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ilg.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fhc.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iah.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bvh.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ynr.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://ncw.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pno.xziqi.cn

[F04] 追加写入文件
来源：http://elj.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://upy.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cos.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qfu.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xbc.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hoi.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cxo.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zze.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lsf.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://xwc.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lgj.uphjek.com

PHP:  file_exists("a.txt");
来源：http://pqs.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://lqg.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://qlu.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jjm.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tom.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://jew.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://iyq.gogol.net.cn

[F06] 删除文件
来源：http://rfk.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://vcv.xinyue.icu

PHP:  unlink("a.txt");
来源：http://kdi.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://zyp.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://uya.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dnd.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://nfg.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://ynw.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://wvi.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://nro.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hex.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qcf.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dqw.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uzz.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://glq.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iny.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jsw.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xha.sufxvd.cn

[F08] 遍历目录
来源：http://fcn.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uuj.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vcw.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://nqv.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://vou.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hqz.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://thd.gzhubu.top

Ruby: Dir.children("dir")
来源：http://vyl.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://kcr.wangdashe.top


<!-- 参考信息 -->