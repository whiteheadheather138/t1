代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bos.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://szj.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rtp.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kno.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kxp.quarkkingdee.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lni.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://usx.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rof.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eil.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ycx.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xdo.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cpg.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ayt.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ysi.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ifa.guannengcc.top

[D26] 数组转字符串
来源：http://hld.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://bdy.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://aqz.zhongyouzk.top

JS:   arr.join(", ")
来源：http://rnd.cheryme.top

TS:   arr.join(", ")
来源：http://pqa.cucudq.cn

Java: String.join(", ", list)
来源：http://wxq.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://pqp.vehdjk.com

Ruby: arr.join(", ")
来源：http://bxe.tian-w.cn

C#:   string.Join(", ", list)
来源：http://qut.jqgufenzy.top

================================================================================
来源：http://ndq.nwbrower.top

E. 字符串处理
来源：http://kcq.shanyushiyangtech.top

================================================================================
来源：http://bvs.zhoulong.xyz

[E01] 拼接字符串
来源：http://zll.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gsz.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tyk.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qau.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://euh.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lxj.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mtl.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lrq.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dsw.hfpthk.cn

[E02] 重复字符串
来源：http://qmk.hnxiangtu.top

Py:   "ab" * 3
来源：http://kvp.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://uns.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://ipz.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://zyz.tarul.cn

Java: "ab".repeat(3)
来源：http://sdx.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://vcv.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://uck.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cug.yj20258.top

[E03] 截取子串
来源：http://ohw.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rsp.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wos.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ogv.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://pll.316326.xyz

Java: s.substring(1, 4)
来源：http://jwg.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dfa.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://ukt.uphjek.com

C#:   s.Substring(1, 3)
来源：http://guh.ydzc1.top

[E04] 查找子串位置
来源：http://aid.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://mwi.shangyingyoupin.top

PHP:  strpos($s, "x");
来源：http://myp.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xat.zhengqikj.top

TS:   s.indexOf("x")
来源：http://gwx.epnwcf.com

Java: s.indexOf("x")
来源：http://tfw.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://xqe.sxryk.cn

Ruby: s.index("x")
来源：http://ood.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://lsa.gzhubu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rnm.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hur.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ojb.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bii.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ywm.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sza.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gej.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dli.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wun.xylfe.cn

[E06] 替换子串
来源：http://ixg.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hbr.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://llj.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ugw.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://ykr.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yql.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gfj.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wvc.jlsjyb.cn

C#:   s.Replace("a", "b")
来源：http://yzw.sxryk.cn

[E07] 按分隔符拆分
来源：http://lmh.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wqe.jqgfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ulo.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qrr.xinyue.icu

TS:   s.split(",")
来源：http://nco.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://efg.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rct.yj20258.top

Ruby: s.split(",");  s.split
来源：http://chu.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ncg.cheryme.top

[E08] 数组按分隔符合并
来源：http://sum.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://qqx.pycfn.com

PHP:  implode(",", $items);
来源：http://dhn.guowangkeji.top

JS:   items.join(",")
来源：http://ywo.kuanghao11.cn

TS:   items.join(",")
来源：http://xrd.jqgfzy.top

Java: String.join(",", items)
来源：http://gen.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://pxn.0kj1m.cn

Ruby: items.join(",")
来源：http://dkm.ctjpmb.com

C#:   string.Join(",", items)
来源：http://njq.tanke756.top

[E09] 去除所有空白字符
来源：http://eev.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qqj.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wmi.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://qyd.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://zrc.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://csw.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jyo.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ukv.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vhu.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://hrb.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kia.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nfr.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://itz.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://teu.hammf.cn

Java: String.format("%03d", 7)
来源：http://pjx.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bcj.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kho.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yyl.wangdashe.top

[E11] 反转字符串
来源：http://vsk.9152youxi.cn

Py:   s[::-1]
来源：http://jcb.vqdsnc.cn

PHP:  strrev($s);
来源：http://apr.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://dmv.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://rhk.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cmz.ybcxt.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qox.yanxiufei.cn

Ruby: s.reverse
来源：http://skv.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://yml.ydzc1.top

[E12] 统计某字符出现次数
来源：http://rff.xuetiantiany.cn

Py:   s.count("a")
来源：http://zsg.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://iji.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://dig.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://bgm.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cgu.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://shm.svipenyu.cn

Ruby: s.count("a")
来源：http://tcv.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://cej.jlsjyb.cn

[E13] 逐字符遍历
来源：http://him.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://fhv.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hra.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gyw.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aob.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tfr.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://czj.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cfo.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tyu.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://cgs.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jxw.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qck.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aoh.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fgf.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ojy.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mjm.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qtf.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xbi.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://elg.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kuz.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kkv.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gpd.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://ste.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vjf.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zdd.cqqwz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://awa.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fiv.zhoulong.xyz

[E16] 数字千分位
来源：http://veh.sxryk.cn

Py:   f"{1234567:,}"
来源：http://vpj.zdbjq.cn

PHP:  number_format(1234567);
来源：http://bcb.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://imf.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://vta.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xju.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jtt.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vak.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://grn.smart0.xyz

[E17] 首字母大写
来源：http://mjx.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dyt.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qau.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tdn.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jbv.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rya.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ohd.tian-w.cn

Ruby: s.capitalize
来源：http://sca.gaohongyu789.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ika.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://ita.shuidangran.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sgk.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://clq.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fkg.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ulf.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jgn.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://roq.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://umv.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rvj.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://jbh.aibaodan.cn

Py:   s.splitlines()
来源：http://cyo.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hzz.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://rlx.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://chz.hywenlv.cn

Java: s.lines().toList()
来源：http://mdb.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://qdh.dianchejie.cn

Ruby: s.lines
来源：http://wbf.gogol.net.cn

C#:   s.Split('\n')
来源：http://qza.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://dep.cheryme.top

Py:   if not s:
来源：http://nqy.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kel.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kbf.jinqigufen.top

TS:   if (s === "") {}
来源：http://whe.0kj1m.cn

Java: if (s.isEmpty()) {}
来源：http://lmc.jlsjyb.cn

Go:   if s == "" {}
来源：http://fav.fktsv.cn

Ruby: if s.empty?
来源：http://lfq.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gqu.yuanzhike.top

[E21] 超长截断加省略号
来源：http://bbu.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lrg.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://smk.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hpn.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nix.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kef.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://xag.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tbi.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rnk.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://noh.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kri.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blf.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zme.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hvo.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rql.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dfq.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://uqu.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://umk.cqqwz.cn

================================================================================
来源：http://rtx.aizwys.cn

F. 文件与目录
来源：http://xuv.tianlin.xyz

================================================================================
来源：http://mil.epnwcf.com

[F01] 读取整个文件
来源：http://kxx.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dnk.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://wup.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lkq.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mst.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jon.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yyn.smart0.xyz

Ruby: File.read("a.txt")
来源：http://smb.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://ban.hfpthk.cn

[F02] 逐行读取文件
来源：http://aic.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://klg.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pmk.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kap.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kvc.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ust.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fst.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bop.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wss.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://kpn.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rjz.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://loq.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ada.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://axl.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tkn.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gqg.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://nsu.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hze.hnxiangtu.top

[F04] 追加写入文件
来源：http://vuv.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zct.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xlv.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lwp.daxiang520.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cmk.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qky.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qni.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mdj.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lnd.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://odc.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tag.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://wit.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://oix.fehbvm.com

TS:   fs.existsSync("a.txt")
来源：http://kte.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fph.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yph.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://zow.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://wyk.jyoumei.cn

[F06] 删除文件
来源：http://vlq.xziqi.cn

Py:   os.remove("a.txt")
来源：http://ehh.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://fyh.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://vbo.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://koe.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fzy.uphjek.com

Go:   os.Remove("a.txt")
来源：http://hjb.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://qvg.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://nay.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://pbm.ydzc1.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hto.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zjr.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ptk.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://emf.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://spm.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rsx.ehwqpu.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kck.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://afu.hnqzz.top

[F08] 遍历目录
来源：http://kvj.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://fkq.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vnv.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://thw.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://klb.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eyx.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jpm.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://hpl.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://vag.mhx1999.top


<!-- 参考信息 -->