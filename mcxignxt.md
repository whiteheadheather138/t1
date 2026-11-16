代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jwy.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xja.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fhw.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://iws.hnqzz.top

Ruby: arr.tally
来源：http://czd.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://got.cheryme.top

[D21] 判断是否包含某元素
来源：http://teb.haohaochexian.top

Py:   x in arr
来源：http://tuo.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://aoc.ctjpmb.com

JS:   arr.includes(x)
来源：http://bad.fktsv.cn

TS:   arr.includes(x)
来源：http://xmp.fehbvm.com

Java: list.contains(x)
来源：http://kqe.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://urd.tarul.cn

Ruby: arr.include?(x)
来源：http://zjy.sufxvd.cn

C#:   list.Contains(x)
来源：http://wbx.kuanghao11.cn

[D22] 复制数组（避免共享引用）
来源：http://dry.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://smz.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://obg.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ayh.hesvh.cn

TS:   [...arr];
来源：http://rzc.hesvh.cn

Java: new ArrayList<>(list);
来源：http://ubf.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://qqb.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://uwq.yanxiufei.cn

C#:   new List<int>(list);
来源：http://qop.c1oappe.top

[D23] reduce 累积计算
来源：http://qxa.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cuh.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dhg.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://syr.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zam.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dja.0kj1m.cn

Go:   // 手写循环
来源：http://lth.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jja.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zva.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://hsv.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qqu.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tsi.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rbc.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fvu.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://abd.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://htc.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://njs.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ziv.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://cvx.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rss.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eno.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hpf.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uem.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://edc.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kqt.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lox.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ymp.zhongyouzk.top

[D26] 数组转字符串
来源：http://kwe.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://ooz.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://sbl.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://oet.guowangkeji.top

TS:   arr.join(", ")
来源：http://ffl.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://wme.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://epy.yongpay.top

Ruby: arr.join(", ")
来源：http://kkv.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://ehl.yj20258.top

================================================================================
来源：http://xsi.nwbrower.top

E. 字符串处理
来源：http://awx.tianlin.xyz

================================================================================
来源：http://wbr.wangdashe.top

[E01] 拼接字符串
来源：http://gow.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hdx.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://csd.aibaodan.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eyk.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://suu.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eku.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://upa.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ohd.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://soy.fanxiaobao.xyz

[E02] 重复字符串
来源：http://cji.gotoacloud.top

Py:   "ab" * 3
来源：http://zvk.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://aky.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://bov.ybcxt.top

TS:   "ab".repeat(3)
来源：http://whq.gotoacloud.top

Java: "ab".repeat(3)
来源：http://luo.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://wqi.hnxiangtu.top

Ruby: "ab" * 3
来源：http://fnr.guannengcc.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ute.jinghuilouyu.cn

[E03] 截取子串
来源：http://yxf.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lcw.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tqp.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zlt.cheryme.top

TS:   s.slice(1, 4)
来源：http://cvl.andypj.xyz

Java: s.substring(1, 4)
来源：http://pvs.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ayz.cdnleiting.top

Ruby: s[1, 3];  s[1..3]
来源：http://asb.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://uzn.fehbvm.com

[E04] 查找子串位置
来源：http://eqy.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://vho.epnwcf.com

PHP:  strpos($s, "x");
来源：http://zbq.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yxq.nanxinkj.top

TS:   s.indexOf("x")
来源：http://bvt.fehbvm.com

Java: s.indexOf("x")
来源：http://odt.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://iax.haohaochexian.top

Ruby: s.index("x")
来源：http://pkn.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://vcg.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://vnf.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nim.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tjx.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kwm.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://glx.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ylz.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ggb.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jzq.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ene.jyoumei.cn

[E06] 替换子串
来源：http://uhs.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://utt.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://pmw.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://umi.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://anx.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lrm.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tkz.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ysr.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://ovm.sweek.top

[E07] 按分隔符拆分
来源：http://sjb.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qbp.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nxb.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qai.yongpay.top

TS:   s.split(",")
来源：http://hgr.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://cue.yuxming.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ntp.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://tkl.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zuy.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://puc.gotoacloud.top

Py:   ",".join(items)
来源：http://ugh.sweek.top

PHP:  implode(",", $items);
来源：http://dlu.ivvv.top

JS:   items.join(",")
来源：http://axm.jinqigfzy.top

TS:   items.join(",")
来源：http://xfu.zhoulong.xyz

Java: String.join(",", items)
来源：http://npa.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://nty.sjlbkw.cn

Ruby: items.join(",")
来源：http://ihf.fehbvm.com

C#:   string.Join(",", items)
来源：http://qjb.ctjpmb.com

[E09] 去除所有空白字符
来源：http://oje.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mpu.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pbh.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://fio.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://vit.jinqigfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://oqi.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xzx.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://xxx.316326.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hiw.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://ord.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jjx.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iwp.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://wwv.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://frr.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://vrc.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://aqw.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://unp.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://txy.gogol.net.cn

[E11] 反转字符串
来源：http://zfr.yueranfly.top

Py:   s[::-1]
来源：http://nkw.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://aeo.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://gpw.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://yiv.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://sev.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ynw.wangdashe.top

Ruby: s.reverse
来源：http://nzt.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gty.ybcxt.top

[E12] 统计某字符出现次数
来源：http://gio.yj202588.top

Py:   s.count("a")
来源：http://qnb.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://ieb.hcnkem.com

JS:   s.split("a").length - 1
来源：http://kwl.epnwcf.com

TS:   s.split("a").length - 1
来源：http://aoi.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kch.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://new.dashuyun.cn

Ruby: s.count("a")
来源：http://orn.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://hnf.shuidangran.top

[E13] 逐字符遍历
来源：http://wkx.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://fxm.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mti.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nvo.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cvh.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://loz.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jbm.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qir.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jnu.jianghu66.top

[E14] URL 编码与 Base64
来源：http://pjj.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tvv.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xhc.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lzx.hfpthk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ews.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://imk.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kqd.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dns.jinqigufen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bpn.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://yvr.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dum.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hpu.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://csa.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wdz.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jtr.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pwq.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zrs.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://osv.c1oappe.top

[E16] 数字千分位
来源：http://zwt.xuanzx.com

Py:   f"{1234567:,}"
来源：http://owg.meibo888.top

PHP:  number_format(1234567);
来源：http://rfe.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jlx.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://weq.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qtl.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lip.sweek.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iud.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://ngm.zdqjudy.top

[E17] 首字母大写
来源：http://jml.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mar.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kiu.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ovh.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xdp.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zqw.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wgu.52xcode.cn

Ruby: s.capitalize
来源：http://neq.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://any.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://xge.daxiang520.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fzo.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wyi.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tlo.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://odi.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wcb.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://acc.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kwm.hnqzz.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://twk.c1oappe.top

[E19] 多行文本按行拆分
来源：http://qxo.cashguo.top

Py:   s.splitlines()
来源：http://tje.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tqm.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://lmw.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://wsb.yongpay.top

Java: s.lines().toList()
来源：http://kba.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://sky.gzhubu.top

Ruby: s.lines
来源：http://ssc.aibaodan.cn

C#:   s.Split('\n')
来源：http://xxq.yongpay.top

[E20] 判断字符串是否为空
来源：http://cmq.redwolf501.top

Py:   if not s:
来源：http://ztd.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ivg.feifeiyinyue.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tta.daria6918.cn

TS:   if (s === "") {}
来源：http://kjt.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://twh.sjlbkw.cn

Go:   if s == "" {}
来源：http://wdq.zdbjq.cn

Ruby: if s.empty?
来源：http://khh.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nof.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://vza.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qjv.jinqigufen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oel.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hxc.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://szy.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sck.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://iuz.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jof.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qxv.yongpay.top

[E22] 字节长度与字符长度
来源：http://ylv.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dwt.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://knu.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://okp.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxd.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wac.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mko.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://lpj.sjlbkw.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fmu.jinghuilouyu.cn

================================================================================
来源：http://ocx.gaohongyu789.top

F. 文件与目录
来源：http://ouu.meibo888.top

================================================================================
来源：http://thi.hcnkem.com

[F01] 读取整个文件
来源：http://zgy.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bbn.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://fqn.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jrz.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kfc.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wou.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ccn.tanke756.top

Ruby: File.read("a.txt")
来源：http://eon.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://edz.jyoumei.cn

[F02] 逐行读取文件
来源：http://nqq.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nsx.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bkw.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://etq.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://chi.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ewo.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pfh.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vpk.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://psr.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://jmv.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iih.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xsc.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oee.yonumen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vbh.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vpc.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jna.epnwcf.com

Ruby: File.write("a.txt", "hi")
来源：http://nca.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vrg.chenlongwang.top

[F04] 追加写入文件
来源：http://iut.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ozb.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://moy.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sbb.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rxp.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eno.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hce.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ezu.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fxd.ctjpmb.com


<!-- 参考信息 -->