代发 wailian999

Ruby: arr.tally
来源：http://tjj.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cls.havefunace.top

[D21] 判断是否包含某元素
来源：http://baq.gogol.net.cn

Py:   x in arr
来源：http://dap.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://tco.daria6918.cn

JS:   arr.includes(x)
来源：http://pmf.quarkkingdee.top

TS:   arr.includes(x)
来源：http://keq.yuxming.cn

Java: list.contains(x)
来源：http://cjw.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://cld.tian-w.cn

Ruby: arr.include?(x)
来源：http://dtb.jianghu66.top

C#:   list.Contains(x)
来源：http://cka.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://sbz.tarul.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bxs.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bum.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://opz.jqgufenzy.top

TS:   [...arr];
来源：http://kov.havefunace.top

Java: new ArrayList<>(list);
来源：http://jgu.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://nji.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://jgd.nwbrower.top

C#:   new List<int>(list);
来源：http://idu.havefunace.top

[D23] reduce 累积计算
来源：http://lqf.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mpz.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aou.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qhf.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gww.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://rfa.redwolf501.top

Go:   // 手写循环
来源：http://xmi.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eee.quarkkingdee.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://alj.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://xqq.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xcd.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hcd.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wnr.pengpengdd.cyou

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yid.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xao.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uff.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kyr.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iys.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://yik.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pfl.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://exw.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://owe.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dfg.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fxv.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vdl.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ned.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://icm.yueranfly.top

[D26] 数组转字符串
来源：http://uzg.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://aaf.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://ihd.hnxiangtu.top

JS:   arr.join(", ")
来源：http://vcj.xziqi.cn

TS:   arr.join(", ")
来源：http://yvc.hesvh.cn

Java: String.join(", ", list)
来源：http://emt.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://lvx.sweek.top

Ruby: arr.join(", ")
来源：http://usy.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://utq.316326.xyz

================================================================================
来源：http://wxn.tarul.cn

E. 字符串处理
来源：http://rpe.haohaochexian.top

================================================================================
来源：http://ibv.aibaodan.cn

[E01] 拼接字符串
来源：http://tci.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://onb.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jqj.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qie.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bqd.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lnc.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bgv.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vvv.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lyv.zhengqikj.top

[E02] 重复字符串
来源：http://olw.haohaochexian.top

Py:   "ab" * 3
来源：http://miz.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://rmm.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://frx.iojbl.cn

TS:   "ab".repeat(3)
来源：http://fmc.smart0.xyz

Java: "ab".repeat(3)
来源：http://hjz.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://rhe.hcnkem.com

Ruby: "ab" * 3
来源：http://qki.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qln.fktsv.cn

[E03] 截取子串
来源：http://jor.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rmd.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://awz.xziqi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cbs.hesvh.cn

TS:   s.slice(1, 4)
来源：http://jqb.ctjpmb.com

Java: s.substring(1, 4)
来源：http://aeh.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bty.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://vrr.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://yfs.quarkkingdee.top

[E04] 查找子串位置
来源：http://ugn.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://bzh.zhixingplan.top

PHP:  strpos($s, "x");
来源：http://iuv.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vqf.jiagoushi.top

TS:   s.indexOf("x")
来源：http://yxj.dianchejie.cn

Java: s.indexOf("x")
来源：http://yum.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://fgs.vehdjk.com

Ruby: s.index("x")
来源：http://wtq.smart0.xyz

C#:   s.IndexOf("x")
来源：http://fue.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://grd.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cns.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://twk.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yvn.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://kow.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egp.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fpe.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jzi.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mog.wangshuangyany.cn

[E06] 替换子串
来源：http://ttw.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wfx.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://qpb.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uqx.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://aqb.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fwk.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jjb.nanxinkj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uxm.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://mka.fengsongda.top

[E07] 按分隔符拆分
来源：http://nnd.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vyj.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://etm.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://etx.zdbjq.cn

TS:   s.split(",")
来源：http://ihl.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://rqi.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xlp.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://gvp.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://opi.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://pru.chenzaomai.com

Py:   ",".join(items)
来源：http://vub.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://ibx.snrcjt.cn

JS:   items.join(",")
来源：http://mzi.havefunace.top

TS:   items.join(",")
来源：http://tgn.ehwqpu.com

Java: String.join(",", items)
来源：http://ens.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://csz.zhixingplan.top

Ruby: items.join(",")
来源：http://khq.hcnkem.com

C#:   string.Join(",", items)
来源：http://tsi.smart0.xyz

[E09] 去除所有空白字符
来源：http://wfv.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qdd.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dsv.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://eio.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://snc.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://efx.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rae.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://pto.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rml.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://pkt.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hap.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mjn.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://prl.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://elp.xinyue.icu

Java: String.format("%03d", 7)
来源：http://wwm.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ljf.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ire.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xbr.hywenlv.cn

[E11] 反转字符串
来源：http://wko.cqqwz.cn

Py:   s[::-1]
来源：http://sdx.aibaodan.cn

PHP:  strrev($s);
来源：http://ypu.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://cpf.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://rqu.pengpengdd.cyou

Java: new StringBuilder(s).reverse().toString()
来源：http://nvl.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jpc.andypj.xyz

Ruby: s.reverse
来源：http://jsi.hysaishi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qny.jianghu66.top

[E12] 统计某字符出现次数
来源：http://wpb.birdmap.top

Py:   s.count("a")
来源：http://hum.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://fcm.daria6918.cn

JS:   s.split("a").length - 1
来源：http://uaw.yongpay.top

TS:   s.split("a").length - 1
来源：http://kez.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mnn.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://qfu.ctjpmb.com

Ruby: s.count("a")
来源：http://xma.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://bay.xinyue.icu

[E13] 逐字符遍历
来源：http://mta.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://gpr.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wbf.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ytg.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jcv.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mnr.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iyu.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bka.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dre.xinyue.icu

[E14] URL 编码与 Base64
来源：http://onj.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://muo.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wvk.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aev.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kuz.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ejp.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jze.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://znc.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://djw.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://ffa.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://zpk.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ezv.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kvp.9152youxi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tra.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hxt.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jyh.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mlm.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bpj.sxryk.cn

[E16] 数字千分位
来源：http://toq.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://ire.dianchejie.cn

PHP:  number_format(1234567);
来源：http://vni.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fth.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gho.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ofd.ivvv.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bsb.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nkc.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://qhp.yj20258.top

[E17] 首字母大写
来源：http://sqm.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://edc.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://qsy.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kqe.yvedp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mfm.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kvk.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://opu.jqgfzy.top

Ruby: s.capitalize
来源：http://amk.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dac.jianghu66.top

[E18] 模板占位符替换
来源：http://lgh.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nrf.jqgufenzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ohf.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://eac.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dxq.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wzg.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qpp.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jqw.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://chy.daria6918.cn

[E19] 多行文本按行拆分
来源：http://koi.shuidangran.top

Py:   s.splitlines()
来源：http://qey.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mvg.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://csz.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://pql.gotoacloud.top

Java: s.lines().toList()
来源：http://qxl.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://wtx.jqgfzy.top

Ruby: s.lines
来源：http://voa.cdnleiting.top

C#:   s.Split('\n')
来源：http://vrf.birdmap.top

[E20] 判断字符串是否为空
来源：http://cad.iojbl.cn

Py:   if not s:
来源：http://ype.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://chf.jinghuilouyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uyr.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://usv.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://rha.fzhhl.top

Go:   if s == "" {}
来源：http://atg.epnwcf.com

Ruby: if s.empty?
来源：http://vgj.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eiw.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://yev.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ssi.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vjc.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://efl.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rdg.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gdg.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://gfl.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://upe.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cfj.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://siu.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vuv.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jyf.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zda.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bzf.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://acn.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ttv.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://lrr.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kxh.yangfankeji.com

================================================================================
来源：http://run.jqgfzy.top

F. 文件与目录
来源：http://ild.aizwys.cn

================================================================================
来源：http://bcn.andypj.xyz

[F01] 读取整个文件
来源：http://zjb.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wyw.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://bce.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://icp.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zri.aibaodan.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://psc.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ekp.jianghu66.top

Ruby: File.read("a.txt")
来源：http://nsd.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://hwm.yuxming.cn

[F02] 逐行读取文件
来源：http://suz.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qqy.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qpz.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uuc.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://boq.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oza.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gao.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cvf.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cwh.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://kcq.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tfj.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ksk.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eyq.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tvo.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tix.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://czx.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://vzs.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rwl.yanxiufei.cn

[F04] 追加写入文件
来源：http://tvj.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ich.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lxx.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dgb.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gii.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qps.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gic.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bqu.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rdm.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://rwx.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gro.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://zmr.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://luw.jianghu66.top


<!-- 参考信息 -->