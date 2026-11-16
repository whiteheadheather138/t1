代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yvq.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ata.vehdjk.com

Go:   // 手写循环
来源：http://bxg.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oam.pengpengdd.cyou

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ubw.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://xxf.havefunace.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://afl.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sqh.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hnl.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ryi.xziqi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nfn.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pkv.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ojx.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gnm.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://vzw.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tvt.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yho.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bvt.aizwys.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xzs.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fks.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zcr.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lzt.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sgw.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://jvn.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://kur.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://lgi.guowangkeji.top

JS:   arr.join(", ")
来源：http://hho.yangfankeji.com

TS:   arr.join(", ")
来源：http://iaa.52xcode.cn

Java: String.join(", ", list)
来源：http://mlf.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://gut.yfazqb.com

Ruby: arr.join(", ")
来源：http://xbk.hesvh.cn

C#:   string.Join(", ", list)
来源：http://qwe.cashguo.top

================================================================================
来源：http://dbj.cucudq.cn

E. 字符串处理
来源：http://cqx.ydzc1.top

================================================================================
来源：http://mzb.zhijiandao.cn

[E01] 拼接字符串
来源：http://gpu.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bza.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jkf.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jyh.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://apg.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nua.yanxiufei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qhc.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pgi.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eph.guowangkeji.top

[E02] 重复字符串
来源：http://uab.ivvv.top

Py:   "ab" * 3
来源：http://gjm.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://pyo.daria6918.cn

JS:   "ab".repeat(3)
来源：http://ozs.yongpay.top

TS:   "ab".repeat(3)
来源：http://agl.vehdjk.com

Java: "ab".repeat(3)
来源：http://dfi.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://dtx.ctjpmb.com

Ruby: "ab" * 3
来源：http://zae.kuanghao11.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ssc.jyoumei.cn

[E03] 截取子串
来源：http://aad.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wvq.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ilr.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bxo.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://dfr.pycfn.com

Java: s.substring(1, 4)
来源：http://ypq.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dis.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://arw.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://fgw.fktsv.cn

[E04] 查找子串位置
来源：http://lcc.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://qgk.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://jfz.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ypk.havefunace.top

TS:   s.indexOf("x")
来源：http://vod.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://gwi.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://cwv.fktsv.cn

Ruby: s.index("x")
来源：http://ugz.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://krn.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uwl.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iej.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mka.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://huf.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jzj.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aej.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://msf.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oht.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hye.fehbvm.com

[E06] 替换子串
来源：http://wsu.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oyt.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://uzw.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://isa.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://tus.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kla.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rnu.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wah.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://fnu.9152youxi.cn

[E07] 按分隔符拆分
来源：http://ydl.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fvm.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uoi.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zur.wangshuangyany.cn

TS:   s.split(",")
来源：http://fcc.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vwe.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lla.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://lqc.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uwt.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://rqw.meibo888.top

Py:   ",".join(items)
来源：http://sgt.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://dkq.yj202588.top

JS:   items.join(",")
来源：http://aak.zhengqikj.top

TS:   items.join(",")
来源：http://fvu.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://buj.tanke756.top

Go:   strings.Join(items, ",")
来源：http://avi.jlsjyb.cn

Ruby: items.join(",")
来源：http://npk.pycfn.com

C#:   string.Join(",", items)
来源：http://erd.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://trq.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rxh.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fpf.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://cir.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://mws.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://kji.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://gfv.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://bbo.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rmo.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://qwy.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gzb.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sbu.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://zpo.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://nyn.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://lfg.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ign.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://whm.jinyuanbaomall.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fsc.zdbjq.cn

[E11] 反转字符串
来源：http://skb.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://jzc.jinqigfzy.top

PHP:  strrev($s);
来源：http://unm.tarul.cn

JS:   [...s].reverse().join("")
来源：http://nwh.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://otk.jyoumei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mho.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eqs.0kj1m.cn

Ruby: s.reverse
来源：http://inw.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tku.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://qhv.zdqjudy.top

Py:   s.count("a")
来源：http://vnm.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://bnb.sysykeji.top

JS:   s.split("a").length - 1
来源：http://hat.fengsongda.top

TS:   s.split("a").length - 1
来源：http://nvi.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qsv.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://pom.daria6918.cn

Ruby: s.count("a")
来源：http://mvf.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://pst.pycfn.com

[E13] 逐字符遍历
来源：http://wbu.cashguo.top

Py:   for ch in s: print(ch)
来源：http://gqo.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vto.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://fay.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qgd.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cxt.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fdl.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ufd.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gxk.zycfv.cn

[E14] URL 编码与 Base64
来源：http://zak.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vzf.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://dku.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kff.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ttw.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hbu.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cqw.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hah.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nco.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://qeb.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tkh.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mcp.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mzs.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mjw.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qcr.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iux.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nhx.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rja.daxiang520.top

[E16] 数字千分位
来源：http://zld.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://mlg.nanxinkj.top

PHP:  number_format(1234567);
来源：http://oct.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vms.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ued.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fmq.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cjx.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rtz.cashguo.top

C#:   1234567.ToString("N0")
来源：http://bst.zhongyouzk.top

[E17] 首字母大写
来源：http://sun.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vzp.cqqwz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wik.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zgt.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://icj.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lkh.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://trb.dashuyun.cn

Ruby: s.capitalize
来源：http://sny.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://suc.sysykeji.top

[E18] 模板占位符替换
来源：http://zos.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nut.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sod.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zyc.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zmy.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xuw.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gva.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lkj.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://asq.yvedp.cn

[E19] 多行文本按行拆分
来源：http://bnj.hnxiangtu.top

Py:   s.splitlines()
来源：http://vil.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ffx.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://ird.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://ksf.jinqigufen.top

Java: s.lines().toList()
来源：http://kbh.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://uso.ybcxt.top

Ruby: s.lines
来源：http://dql.yangfankeji.com

C#:   s.Split('\n')
来源：http://qfj.xuanzx.com

[E20] 判断字符串是否为空
来源：http://izu.cucudq.cn

Py:   if not s:
来源：http://glf.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zom.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yew.dashuyun.cn

TS:   if (s === "") {}
来源：http://huy.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://lip.9152youxi.cn

Go:   if s == "" {}
来源：http://iyu.cashguo.top

Ruby: if s.empty?
来源：http://ymq.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wur.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://ckm.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jbf.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://grf.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fmn.yanxiufei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sku.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qje.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://jdb.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jkm.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vuz.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://wkt.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dhc.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pdw.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mrk.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vso.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gku.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xbv.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://yug.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://agr.yuanzhike.top

================================================================================
来源：http://zhv.meibo888.top

F. 文件与目录
来源：http://jwm.daxiang520.top

================================================================================
来源：http://jlw.gotoacloud.top

[F01] 读取整个文件
来源：http://sgb.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://txw.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://ulm.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pbp.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://drm.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sfr.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vjq.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://hpw.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://slp.shzxlz.cn

[F02] 逐行读取文件
来源：http://sqe.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vyx.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ubc.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lbc.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qvu.0kj1m.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qyq.hammf.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gky.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dru.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hib.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://yqh.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hzg.andypj.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://umy.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ier.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rqo.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rax.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fgv.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://bts.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fsu.tanke756.top

[F04] 追加写入文件
来源：http://lsi.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://urj.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uoa.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://icx.ivvv.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vwe.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mtn.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ojw.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yrm.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kdg.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://wul.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tpz.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://olw.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://pka.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://shf.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gmf.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ogj.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://tum.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://awg.kuanghao11.cn

[F06] 删除文件
来源：http://ldu.jianghu66.top

Py:   os.remove("a.txt")
来源：http://xud.yueranfly.top

PHP:  unlink("a.txt");
来源：http://mvp.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://ohq.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://enq.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wjk.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://taq.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://one.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://jha.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://yxx.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sgk.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bcb.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ddt.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://huv.dashuyun.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ozu.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ufs.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ihp.jqgfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://joc.0kj1m.cn

[F08] 遍历目录
来源：http://ibq.yonumen.top


<!-- 参考信息 -->