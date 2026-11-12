代发 wailian999

Ruby: arr.tally
来源：http://cdb.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xbq.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://yko.feifeiyinyue.top

Py:   x in arr
来源：http://mzo.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://kco.bjfxy.top

JS:   arr.includes(x)
来源：http://agv.daria6918.cn

TS:   arr.includes(x)
来源：http://tmg.shangyingyoupin.top

Java: list.contains(x)
来源：http://emh.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://ywm.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://vko.hnqzz.top

C#:   list.Contains(x)
来源：http://ucd.sxryk.cn

[D22] 复制数组（避免共享引用）
来源：http://igk.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gle.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yhu.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zrz.hongshengwenyu.top

TS:   [...arr];
来源：http://iwz.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://gnb.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://ene.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://uty.zycfv.cn

C#:   new List<int>(list);
来源：http://gdn.fktsv.cn

[D23] reduce 累积计算
来源：http://vcj.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://asa.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mxb.sweek.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ldv.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gse.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uqs.cucudq.cn

Go:   // 手写循环
来源：http://pgc.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jdl.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qey.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://kfq.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wig.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://djk.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yji.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yoo.hnxiangtu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jvs.chenjidiqi.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rob.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dtu.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://byk.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://dkn.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fum.sysykeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://taq.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://edz.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yth.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eyw.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lhw.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jtq.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xgp.zycfv.cn

[D26] 数组转字符串
来源：http://wol.svipenyu.cn

Py:   ", ".join(map(str, arr))
来源：http://qyp.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://gea.guannengcc.top

JS:   arr.join(", ")
来源：http://avc.ivvv.top

TS:   arr.join(", ")
来源：http://qgj.bjfxy.top

Java: String.join(", ", list)
来源：http://npo.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://ptk.yj20258888.top

Ruby: arr.join(", ")
来源：http://gen.yueranfly.top

C#:   string.Join(", ", list)
来源：http://flu.xinyue.icu

================================================================================
来源：http://ilk.nwbrower.top

E. 字符串处理
来源：http://ayo.gaohongyu789.top

================================================================================
来源：http://hsu.nanxinkj.top

[E01] 拼接字符串
来源：http://ath.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aaz.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yqm.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wbv.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kox.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fvx.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wum.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dan.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iww.52xcode.cn

[E02] 重复字符串
来源：http://kbe.jinghuilouyu.cn

Py:   "ab" * 3
来源：http://yob.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://pgb.xinyue.icu

JS:   "ab".repeat(3)
来源：http://dsw.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://pht.pengpengdd.cyou

Java: "ab".repeat(3)
来源：http://jfo.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://ugh.nanxuanxn.top

Ruby: "ab" * 3
来源：http://yvw.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sgm.pengpengdd.cyou

[E03] 截取子串
来源：http://rcg.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mee.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nux.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qid.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://nxw.iojbl.cn

Java: s.substring(1, 4)
来源：http://alz.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://akz.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dxx.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://uay.yongpay.top

[E04] 查找子串位置
来源：http://wxt.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://pxe.bbcook.cn

PHP:  strpos($s, "x");
来源：http://lzb.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://enc.316326.xyz

TS:   s.indexOf("x")
来源：http://thk.pengpengdd.cyou

Java: s.indexOf("x")
来源：http://jyq.cashguo.top

Go:   strings.Index(s, "x")
来源：http://kat.pengpengdd.cyou

Ruby: s.index("x")
来源：http://dtf.yj20258.top

C#:   s.IndexOf("x")
来源：http://bym.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xrn.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://msl.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cvo.jlsjyb.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mvn.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hwy.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fjg.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xos.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://paj.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cac.nanxuanxn.top

[E06] 替换子串
来源：http://ika.svipenyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ttb.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://glb.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lhl.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://nks.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ans.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mgy.yonumen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hhy.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://jah.cdnleiting.top

[E07] 按分隔符拆分
来源：http://sko.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ebl.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://htk.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nnj.hysaishi.cn

TS:   s.split(",")
来源：http://vqv.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://olb.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jat.cheryme.top

Ruby: s.split(",");  s.split
来源：http://qzd.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ttg.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://urj.shzxlz.cn

Py:   ",".join(items)
来源：http://ino.bbcook.cn

PHP:  implode(",", $items);
来源：http://eqo.zhijiandao.cn

JS:   items.join(",")
来源：http://ftc.dashuyun.cn

TS:   items.join(",")
来源：http://xhu.chenzaomai.com

Java: String.join(",", items)
来源：http://fis.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://qes.wangshuangyany.cn

Ruby: items.join(",")
来源：http://fwn.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://jdw.chenzaomai.com

[E09] 去除所有空白字符
来源：http://uxd.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://asc.snrcjt.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zyn.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://qjp.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://qly.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://uqq.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nti.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://mhh.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uvi.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://pyj.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mcc.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gix.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://mvg.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://buv.hnqzz.top

Java: String.format("%03d", 7)
来源：http://rtv.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://isj.zhijiandao.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rne.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hys.xylfe.cn

[E11] 反转字符串
来源：http://mrc.guowangkeji.top

Py:   s[::-1]
来源：http://txn.pengpengdd.cyou

PHP:  strrev($s);
来源：http://asm.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://mhl.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://dec.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fby.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ckz.ivvv.top

Ruby: s.reverse
来源：http://oug.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://nob.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://dey.cheryme.top

Py:   s.count("a")
来源：http://snr.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://wmb.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://wgd.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://nnq.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ygv.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://csn.gogol.net.cn

Ruby: s.count("a")
来源：http://atk.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://omn.svipenyu.cn

[E13] 逐字符遍历
来源：http://sib.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://vfo.ywan-chungtsiang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qkm.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tml.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xhx.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ggf.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wtx.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wkt.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kqn.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://vcm.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pot.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://tav.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hvt.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ibz.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xfy.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zhf.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://guo.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://puj.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://hgq.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bma.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sjk.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cfb.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mja.yueranfly.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ice.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zfm.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dmr.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ugu.zhixingplan.top

[E16] 数字千分位
来源：http://dfg.cashguo.top

Py:   f"{1234567:,}"
来源：http://tmz.tanke756.top

PHP:  number_format(1234567);
来源：http://dxo.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mlp.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fbf.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bbq.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tnk.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dxs.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://zvp.zdbjq.cn

[E17] 首字母大写
来源：http://xli.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kue.zhijiandao.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kmk.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vsd.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uny.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ezs.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zkj.zhoulong.xyz

Ruby: s.capitalize
来源：http://krn.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ikw.cucudq.cn

[E18] 模板占位符替换
来源：http://rve.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qct.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eis.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tcv.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wrx.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ios.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ief.hesvh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://azw.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cqy.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://vsu.zhoulong.xyz

Py:   s.splitlines()
来源：http://ovs.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://evb.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://xeq.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://zou.yuanzhike.top

Java: s.lines().toList()
来源：http://adz.hammf.cn

Go:   strings.Split(s, "\n")
来源：http://udp.fengsongda.top

Ruby: s.lines
来源：http://lsh.yonumen.top

C#:   s.Split('\n')
来源：http://kot.gzhubu.top

[E20] 判断字符串是否为空
来源：http://qch.nanxuanxn.top

Py:   if not s:
来源：http://zpo.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pkf.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kyn.gaohongyu789.top

TS:   if (s === "") {}
来源：http://gzm.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://ydx.tarul.cn

Go:   if s == "" {}
来源：http://owh.yonumen.top

Ruby: if s.empty?
来源：http://amh.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ebd.smart0.xyz

[E21] 超长截断加省略号
来源：http://rie.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://upq.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rze.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vgs.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xeh.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sip.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ufp.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jik.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pcb.ybcxt.top

[E22] 字节长度与字符长度
来源：http://uah.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dss.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://isj.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rcf.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tpe.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pmi.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mjg.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://eak.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://asn.zhengqikj.top

================================================================================
来源：http://pcc.fzhhl.top

F. 文件与目录
来源：http://hbz.yueranfly.top

================================================================================
来源：http://msq.andypj.xyz

[F01] 读取整个文件
来源：http://rea.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ysa.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://pge.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jbs.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aja.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://glk.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://feh.daria6918.cn

Ruby: File.read("a.txt")
来源：http://atu.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://civ.havefunace.top

[F02] 逐行读取文件
来源：http://saf.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vwf.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://buo.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rfc.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qhn.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sso.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vqf.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lvu.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://crg.yonumen.top

[F03] 写入文件（覆盖）
来源：http://yjc.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://npr.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gfx.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jbf.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jae.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mwq.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fmf.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://sxd.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://puu.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://bjs.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mkg.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sru.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://png.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lug.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wxj.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zln.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fmx.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rvf.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://zgy.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wrb.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://mrn.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://ppz.cheryme.top


<!-- 参考信息 -->