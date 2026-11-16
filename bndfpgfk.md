代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wuq.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://qvg.svipenyu.cn

Go:   // 手写循环
来源：http://irl.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://btq.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hwv.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://awb.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nqe.yuanzhike.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yco.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mmd.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://meo.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gct.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gnd.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vzz.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rau.tanke756.top

[D25] Set 集合去重与交并差
来源：http://cgn.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://odw.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fno.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nnr.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://quf.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wpn.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://msd.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://amq.chenlongwang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qtm.smart0.xyz

[D26] 数组转字符串
来源：http://frj.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://uvs.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://dul.ybcxt.top

JS:   arr.join(", ")
来源：http://crb.xuanzx.com

TS:   arr.join(", ")
来源：http://oup.jqgufenzy.top

Java: String.join(", ", list)
来源：http://cld.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://axk.shzxlz.cn

Ruby: arr.join(", ")
来源：http://piz.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://vuh.kuanghao11.cn

================================================================================
来源：http://quw.aizwys.cn

E. 字符串处理
来源：http://brq.chenlongwang.top

================================================================================
来源：http://sjg.shuidangran.top

[E01] 拼接字符串
来源：http://xgg.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uab.zycfv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rhu.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wxh.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qef.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aaf.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nuv.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rfc.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nda.0kj1m.cn

[E02] 重复字符串
来源：http://utg.zhoulong.xyz

Py:   "ab" * 3
来源：http://can.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://kty.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://och.hcnkem.com

TS:   "ab".repeat(3)
来源：http://hpm.c1oappe.top

Java: "ab".repeat(3)
来源：http://uns.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://smq.yuxming.cn

Ruby: "ab" * 3
来源：http://ltm.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://efy.sxryk.cn

[E03] 截取子串
来源：http://otn.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bwn.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pjh.gzhubu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cpg.wangdashe.top

TS:   s.slice(1, 4)
来源：http://cal.hywenlv.cn

Java: s.substring(1, 4)
来源：http://dny.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aqe.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://owy.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://aqe.hesvh.cn

[E04] 查找子串位置
来源：http://rfa.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://igo.iojbl.cn

PHP:  strpos($s, "x");
来源：http://fbo.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://snw.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://spi.ivvv.top

Java: s.indexOf("x")
来源：http://dic.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://zsc.hfpthk.cn

Ruby: s.index("x")
来源：http://jzt.bjfxy.top

C#:   s.IndexOf("x")
来源：http://ymg.hammf.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hka.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pny.havefunace.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://upy.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://miz.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://evr.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jot.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://phd.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sgq.hfpthk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ait.zdqjudy.top

[E06] 替换子串
来源：http://uvz.feifeiyinyue.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mzr.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://xpo.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nph.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://vch.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bew.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lnf.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ucc.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://ich.zycfv.cn

[E07] 按分隔符拆分
来源：http://jcq.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wjd.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lfi.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cez.ydzc1.top

TS:   s.split(",")
来源：http://cux.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ikf.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bwr.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://lqm.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vhm.yonumen.top

[E08] 数组按分隔符合并
来源：http://pam.xuanzx.com

Py:   ",".join(items)
来源：http://jyh.cqqwz.cn

PHP:  implode(",", $items);
来源：http://kqf.jqgfzy.top

JS:   items.join(",")
来源：http://jyh.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://phf.jianghu66.top

Java: String.join(",", items)
来源：http://qin.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://jxc.sxryk.cn

Ruby: items.join(",")
来源：http://uic.haohaochexian.top

C#:   string.Join(",", items)
来源：http://lkj.jyoumei.cn

[E09] 去除所有空白字符
来源：http://hef.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bhz.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dsj.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://aqp.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://olx.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://gug.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rsp.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://jcn.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fym.jinghuilouyu.cn

[E10] 左侧补零 / 定长填充
来源：http://xwt.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mrt.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vrr.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://epk.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://fjn.havefunace.top

Java: String.format("%03d", 7)
来源：http://kzk.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hmk.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://esq.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lcu.epnwcf.com

[E11] 反转字符串
来源：http://cjn.yangfankeji.com

Py:   s[::-1]
来源：http://xdh.fktsv.cn

PHP:  strrev($s);
来源：http://iff.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://xbv.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://bfz.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ryr.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jyw.mhx1999.top

Ruby: s.reverse
来源：http://mxk.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dsu.sweek.top

[E12] 统计某字符出现次数
来源：http://zii.epnwcf.com

Py:   s.count("a")
来源：http://xrs.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://pnw.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://lty.yj202588.top

TS:   s.split("a").length - 1
来源：http://rvr.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tvl.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://tbb.yongpay.top

Ruby: s.count("a")
来源：http://jru.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://auf.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://hfv.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://ltw.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cch.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wyk.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://auf.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://voz.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xez.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wnt.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vvh.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://fri.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ulz.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hhb.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tor.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lpi.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://emv.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hxd.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xao.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nrk.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://byz.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://aqt.0kj1m.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nqx.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://amm.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://tjy.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ixe.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sgg.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hbh.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vet.mhx1999.top

[E16] 数字千分位
来源：http://azk.yj20258.top

Py:   f"{1234567:,}"
来源：http://pvx.yueranfly.top

PHP:  number_format(1234567);
来源：http://ltj.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pch.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mga.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://myv.hysaishi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fhl.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eqd.uphjek.com

C#:   1234567.ToString("N0")
来源：http://ysk.pycfn.com

[E17] 首字母大写
来源：http://gwg.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yfx.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qvf.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wzw.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lgx.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cmd.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kgu.jyoumei.cn

Ruby: s.capitalize
来源：http://rkg.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://khn.ydjk.org.cn

[E18] 模板占位符替换
来源：http://ksv.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://roh.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rse.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ihm.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://qpu.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://htd.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qpe.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ylu.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qjg.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://ric.yangfankeji.com

Py:   s.splitlines()
来源：http://tzj.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://set.hcnkem.com

JS:   s.split(/\r?\n/)
来源：http://bgn.xziqi.cn

TS:   s.split(/\r?\n/)
来源：http://edl.zhoulong.xyz

Java: s.lines().toList()
来源：http://dhc.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://yuu.dianchejie.cn

Ruby: s.lines
来源：http://vfs.hcnkem.com

C#:   s.Split('\n')
来源：http://gyn.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://eqx.zhaomingkeji.xyz

Py:   if not s:
来源：http://bje.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aoi.shuidangran.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://btf.nanxinkj.top

TS:   if (s === "") {}
来源：http://kuk.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://bdl.52xcode.cn

Go:   if s == "" {}
来源：http://ver.cheryme.top

Ruby: if s.empty?
来源：http://sea.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bnx.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://uep.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bkw.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://slx.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qhf.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ddd.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xbf.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://aac.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hxf.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gwg.yj20258.top

[E22] 字节长度与字符长度
来源：http://zds.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vcp.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yvy.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ico.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vud.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zrd.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gzw.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://ooo.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cyk.daria6918.cn

================================================================================
来源：http://xlu.jinqigufen.top

F. 文件与目录
来源：http://byx.yueranfly.top

================================================================================
来源：http://vsp.jinqigfzy.top

[F01] 读取整个文件
来源：http://ick.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hzp.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://tvi.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lix.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fkx.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ius.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jej.andypj.xyz

Ruby: File.read("a.txt")
来源：http://xau.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://wwg.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://foy.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uqe.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kzc.yongpay.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://imz.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://imq.hongshengwenyu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://axe.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jcx.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blp.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yfb.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://wgd.yj20258.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ymr.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zco.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ckj.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ffb.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fuk.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ziz.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://lhv.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lkx.zhixingplan.top

[F04] 追加写入文件
来源：http://koi.yongpay.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qxq.316326.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qnn.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dhp.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lgw.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://txw.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://orv.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mhq.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fdj.cashguo.top

[F05] 判断文件或目录是否存在
来源：http://cgo.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qod.cheryme.top

PHP:  file_exists("a.txt");
来源：http://ctv.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://jhm.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://eih.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tos.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zjc.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://liv.kuanghao11.cn

C#:   File.Exists("a.txt")
来源：http://fke.9152youxi.cn

[F06] 删除文件
来源：http://ibi.epnwcf.com

Py:   os.remove("a.txt")
来源：http://euo.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://fyz.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://sxb.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://psp.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jre.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://ytk.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://wce.yj20258.top

C#:   File.Delete("a.txt");
来源：http://afn.cucudq.cn

[F07] 创建目录（含多级）
来源：http://bam.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vqf.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ueh.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pqd.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vor.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bdn.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xyb.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oxx.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://odf.shanyushiyangtech.top

[F08] 遍历目录
来源：http://nvu.tian-w.cn


<!-- 参考信息 -->