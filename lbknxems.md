代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gdb.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://rrr.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ffw.bbcook.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://asp.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eoz.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uum.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lkn.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mex.jiagoushi.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ski.ehwqpu.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jjv.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://cyf.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ntr.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vlc.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bqu.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jmd.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dzo.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://heg.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kuv.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ouu.sufxvd.cn

[D26] 数组转字符串
来源：http://zwr.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://ujf.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://ysr.jiagoushi.top

JS:   arr.join(", ")
来源：http://kss.feifeiyinyue.top

TS:   arr.join(", ")
来源：http://iez.redwolf501.top

Java: String.join(", ", list)
来源：http://bpi.guannengcc.top

Go:   strings.Join(strs, ", ")
来源：http://cue.hysaishi.cn

Ruby: arr.join(", ")
来源：http://tan.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://yqd.jinqigufen.top

================================================================================
来源：http://syp.fzhhl.top

E. 字符串处理
来源：http://fwr.vehdjk.com

================================================================================
来源：http://spw.dashuyun.cn

[E01] 拼接字符串
来源：http://edg.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cyj.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sxh.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qol.zycfv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xht.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ryh.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nlw.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mfb.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nal.dianchejie.cn

[E02] 重复字符串
来源：http://ekp.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://dvs.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://pmf.fktsv.cn

JS:   "ab".repeat(3)
来源：http://xmu.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://vxy.shuidangran.top

Java: "ab".repeat(3)
来源：http://vff.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://cbj.yuxming.cn

Ruby: "ab" * 3
来源：http://ttl.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://afo.bbcook.cn

[E03] 截取子串
来源：http://cug.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jki.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gbs.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hve.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://pta.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://rov.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vva.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://hrv.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://ncs.tian-w.cn

[E04] 查找子串位置
来源：http://ykh.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://ewq.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://fxg.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ryo.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://zuq.smart0.xyz

Java: s.indexOf("x")
来源：http://zph.ivvv.top

Go:   strings.Index(s, "x")
来源：http://wal.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://pke.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://fgx.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ios.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tlm.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wjp.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mjf.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yda.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zah.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://beq.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ypz.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://arl.ehwqpu.com

[E06] 替换子串
来源：http://gbf.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mij.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://bik.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ldf.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://yqh.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iax.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jpk.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://utg.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://tvl.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://xkr.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lqo.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jzs.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ned.daria6918.cn

TS:   s.split(",")
来源：http://sdm.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://qkb.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jvw.cashguo.top

Ruby: s.split(",");  s.split
来源：http://ago.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://idx.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://rht.hywenlv.cn

Py:   ",".join(items)
来源：http://axf.ehwqpu.com

PHP:  implode(",", $items);
来源：http://cqp.yanxiufei.cn

JS:   items.join(",")
来源：http://ras.sweek.top

TS:   items.join(",")
来源：http://irz.nanxinkj.top

Java: String.join(",", items)
来源：http://pic.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://lxm.smart0.xyz

Ruby: items.join(",")
来源：http://uuo.tianlin.xyz

C#:   string.Join(",", items)
来源：http://rlh.havefunace.top

[E09] 去除所有空白字符
来源：http://cvv.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rlu.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bsd.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://dws.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://uyr.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://die.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nvx.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://wdl.316326.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://slo.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://ugn.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://spb.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nci.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://eqd.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://rqy.sysykeji.top

Java: String.format("%03d", 7)
来源：http://fdd.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://wrb.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jjc.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gzm.zdbjq.cn

[E11] 反转字符串
来源：http://uam.vqdsnc.cn

Py:   s[::-1]
来源：http://zqh.sjlbkw.cn

PHP:  strrev($s);
来源：http://tjm.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://jpv.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://uvk.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ogz.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bbq.yfazqb.com

Ruby: s.reverse
来源：http://con.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://upm.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://dlb.ehwqpu.com

Py:   s.count("a")
来源：http://nwk.ehwqpu.com

PHP:  substr_count($s, "a");
来源：http://zga.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://gwn.hcnkem.com

TS:   s.split("a").length - 1
来源：http://qpd.zhengqikj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ovf.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://spn.jinqigufen.top

Ruby: s.count("a")
来源：http://rsy.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://qhh.9152youxi.cn

[E13] 逐字符遍历
来源：http://hbv.yongpay.top

Py:   for ch in s: print(ch)
来源：http://whc.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sff.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bfj.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://twv.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qyn.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zlj.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aai.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lti.cashguo.top

[E14] URL 编码与 Base64
来源：http://izy.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yve.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://rdu.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tzu.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nxc.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zbw.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://osp.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ddj.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jps.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://djt.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jnd.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vjp.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://scb.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://zsg.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wwx.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nhb.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zbo.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lmk.316326.xyz

[E16] 数字千分位
来源：http://fbl.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://nnx.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://bjk.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hsu.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tew.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dda.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://joo.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sln.316326.xyz

C#:   1234567.ToString("N0")
来源：http://uip.jyoumei.cn

[E17] 首字母大写
来源：http://iwa.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://izp.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hrk.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zas.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://swa.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://enh.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rms.hfpthk.cn

Ruby: s.capitalize
来源：http://viq.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jto.smart0.xyz

[E18] 模板占位符替换
来源：http://yxy.jiagoushi.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dsl.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xtl.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://mwt.nanxinkj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ddx.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://byp.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xqp.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gso.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ffg.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://rcd.xylfe.cn

Py:   s.splitlines()
来源：http://wob.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mtg.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://eyl.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://kqa.hfpthk.cn

Java: s.lines().toList()
来源：http://ddp.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://okr.bjfxy.top

Ruby: s.lines
来源：http://lcp.yj20258888.top

C#:   s.Split('\n')
来源：http://ebc.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://xie.gaohongyu789.top

Py:   if not s:
来源：http://dpo.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tav.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rbi.haohaochexian.top

TS:   if (s === "") {}
来源：http://cuj.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://vin.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://nyq.havefunace.top

Ruby: if s.empty?
来源：http://zze.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dnl.yvedp.cn

[E21] 超长截断加省略号
来源：http://skd.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xun.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pow.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lrt.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hlr.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jzp.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://alb.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kae.zhengqikj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://slt.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://itm.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vwa.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://agb.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dim.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yju.meibo888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ecg.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oxc.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://fka.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dnl.zdbjq.cn

================================================================================
来源：http://ygg.smart0.xyz

F. 文件与目录
来源：http://ltq.jqgfzy.top

================================================================================
来源：http://wzs.bbcook.cn

[F01] 读取整个文件
来源：http://inl.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uzi.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://vgg.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ysd.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://utx.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fch.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://olu.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://nbd.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://gsm.jqgufenzy.top

[F02] 逐行读取文件
来源：http://vlh.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eva.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vqf.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tik.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gtj.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ypz.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://csb.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fjl.ppjwa.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ohs.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://pzc.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ddf.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bws.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dan.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eiq.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fpk.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gtc.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://nhl.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cwp.cucudq.cn

[F04] 追加写入文件
来源：http://gwi.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hgw.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xmh.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eox.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://viq.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hha.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nij.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wnj.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yfc.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://tuk.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://weh.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://pcw.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://qcz.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://bfy.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://her.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pnr.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://esk.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://knb.9152youxi.cn

[F06] 删除文件
来源：http://dqu.sxryk.cn

Py:   os.remove("a.txt")
来源：http://fna.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://nsr.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://roi.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yqj.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dzr.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://vci.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://lla.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://goh.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://gyy.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tcq.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lhl.tanke756.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dth.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ekx.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tia.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fpx.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lub.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lcf.jianghu66.top

[F08] 遍历目录
来源：http://eud.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://rgs.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ufg.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://bny.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://pss.ctjpmb.com


<!-- 参考信息 -->