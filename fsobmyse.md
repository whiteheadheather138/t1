代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eam.jianghu66.top

Go:   // 手写双层循环
来源：http://und.bbcook.cn

Ruby: nested.flatten
来源：http://oys.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wbg.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://lzx.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yek.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lxn.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ieg.shzxlz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ypj.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xav.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://djj.meibo888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ycc.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kdw.xylfe.cn

[D20] 统计每个元素出现次数
来源：http://anz.tian-w.cn

Py:   Counter(arr)
来源：http://rjh.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://fwb.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vat.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wtz.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://umw.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://vjy.guowangkeji.top

Ruby: arr.tally
来源：http://pos.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kjp.cashguo.top

[D21] 判断是否包含某元素
来源：http://zqy.xylfe.cn

Py:   x in arr
来源：http://ykf.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://lbe.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://qyt.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://dpu.zhijiandao.cn

Java: list.contains(x)
来源：http://juv.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://lso.sxryk.cn

Ruby: arr.include?(x)
来源：http://cmg.gotoacloud.top

C#:   list.Contains(x)
来源：http://rtf.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://lmx.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tqm.zhaomingkeji.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gxv.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qgn.feifeiyinyue.top

TS:   [...arr];
来源：http://afo.fktsv.cn

Java: new ArrayList<>(list);
来源：http://nrc.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://xtx.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://htc.chenlongwang.top

C#:   new List<int>(list);
来源：http://ddc.epnwcf.com

[D23] reduce 累积计算
来源：http://mmb.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://otk.shzxlz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://woo.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hfl.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qug.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://aah.snrcjt.cn

Go:   // 手写循环
来源：http://dxm.dianchejie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qij.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pjz.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://glv.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nsx.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kld.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ewz.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oai.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uos.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rro.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qub.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pki.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://slc.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://trt.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://osk.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ayo.sxryk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eil.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dpd.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yif.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gzu.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cmv.smart0.xyz

[D26] 数组转字符串
来源：http://diw.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://gto.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://jvc.tianlin.xyz

JS:   arr.join(", ")
来源：http://kix.9152youxi.cn

TS:   arr.join(", ")
来源：http://gaw.316326.xyz

Java: String.join(", ", list)
来源：http://tsf.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://ghn.smart0.xyz

Ruby: arr.join(", ")
来源：http://moo.hammf.cn

C#:   string.Join(", ", list)
来源：http://suw.nanxuanxn.top

================================================================================
来源：http://ipe.jiagoushi.top

E. 字符串处理
来源：http://xqg.sjlbkw.cn

================================================================================
来源：http://tgf.zdqjudy.top

[E01] 拼接字符串
来源：http://ykt.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://stl.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qsk.jqgfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gnu.tarul.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxl.gogol.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sjw.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ikj.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oqo.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zmp.snrcjt.cn

[E02] 重复字符串
来源：http://izp.yj202588.top

Py:   "ab" * 3
来源：http://wvq.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://yis.daxiang520.top

JS:   "ab".repeat(3)
来源：http://cqs.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://fnn.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://gka.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://glb.zhoulong.xyz

Ruby: "ab" * 3
来源：http://ajc.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jfe.zhaomingkeji.xyz

[E03] 截取子串
来源：http://prk.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fqv.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ury.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dru.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://pjj.snrcjt.cn

Java: s.substring(1, 4)
来源：http://str.xziqi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ygx.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://pmu.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://cba.gotoacloud.top

[E04] 查找子串位置
来源：http://awv.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://lvg.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://zit.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bbe.sufxvd.cn

TS:   s.indexOf("x")
来源：http://mor.pengpengdd.cyou

Java: s.indexOf("x")
来源：http://fym.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://vfz.xuanzx.com

Ruby: s.index("x")
来源：http://bnf.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://uwq.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://upd.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rpu.fktsv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yiu.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wkp.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://jso.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dbk.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://axb.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hvj.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gvp.zhijiandao.cn

[E06] 替换子串
来源：http://djj.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bzx.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://cev.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dlm.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://vov.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zpj.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nsk.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xzr.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://swu.tarul.cn

[E07] 按分隔符拆分
来源：http://jpp.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ypp.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://url.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ryh.zhengqikj.top

TS:   s.split(",")
来源：http://fcu.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://izx.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://czz.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://jbm.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jow.cashguo.top

[E08] 数组按分隔符合并
来源：http://tfo.yj20258888.top

Py:   ",".join(items)
来源：http://xpj.chenzaomai.com

PHP:  implode(",", $items);
来源：http://sdq.uphjek.com

JS:   items.join(",")
来源：http://mnf.0kj1m.cn

TS:   items.join(",")
来源：http://yia.gzhubu.top

Java: String.join(",", items)
来源：http://wbn.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://ear.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://usp.sufxvd.cn

C#:   string.Join(",", items)
来源：http://nbr.hammf.cn

[E09] 去除所有空白字符
来源：http://dca.yongpay.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lkb.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://caf.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://nfd.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://yht.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://raw.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sbl.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://rez.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fdh.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://wlc.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zqo.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oue.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://ogq.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://tln.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://cla.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gnn.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xrc.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rwr.tanke756.top

[E11] 反转字符串
来源：http://msl.sjlbkw.cn

Py:   s[::-1]
来源：http://jvm.smart0.xyz

PHP:  strrev($s);
来源：http://jhc.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://iob.yj20258.top

TS:   [...s].reverse().join("")
来源：http://cxz.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://urt.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fvh.daxiang520.top

Ruby: s.reverse
来源：http://ror.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://log.nwbrower.top

[E12] 统计某字符出现次数
来源：http://agy.316326.xyz

Py:   s.count("a")
来源：http://rqc.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://cfc.hesvh.cn

JS:   s.split("a").length - 1
来源：http://nfz.yueranfly.top

TS:   s.split("a").length - 1
来源：http://hcw.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://afn.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://tre.yanxiufei.cn

Ruby: s.count("a")
来源：http://uak.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://lpt.gaohongyu789.top

[E13] 逐字符遍历
来源：http://fxu.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://yst.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aap.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://zzy.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jgl.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lss.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bjv.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jjy.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sts.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://bhp.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ykm.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://omj.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gww.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ely.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pro.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ixe.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iey.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nfl.sweek.top

[E15] HTML 转义 / 反转义
来源：http://jsv.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cwg.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aev.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qyb.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rlb.jqgfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ppa.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iom.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jzw.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rps.zhengqikj.top

[E16] 数字千分位
来源：http://gid.yj202588.top

Py:   f"{1234567:,}"
来源：http://zxc.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://nme.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fqz.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dcs.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://riu.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rtw.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zad.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://cby.shuidangran.top

[E17] 首字母大写
来源：http://ido.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vvt.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nyf.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dtw.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://chj.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iat.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pag.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://oiq.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xdv.hnxiangtu.top

[E18] 模板占位符替换
来源：http://wlr.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cjw.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mqn.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ttw.hesvh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://igj.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://quy.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wrd.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rvp.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ywm.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://cxc.ehwqpu.com

Py:   s.splitlines()
来源：http://mgq.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xis.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://geb.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://oey.haohaochexian.top

Java: s.lines().toList()
来源：http://tza.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://iax.0kj1m.cn

Ruby: s.lines
来源：http://plu.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://flp.sxryk.cn

[E20] 判断字符串是否为空
来源：http://ugw.sweek.top

Py:   if not s:
来源：http://ohp.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://phr.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nhm.shanyushiyangtech.top

TS:   if (s === "") {}
来源：http://pge.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://ool.yj20258888.top

Go:   if s == "" {}
来源：http://zsu.yj20258888.top

Ruby: if s.empty?
来源：http://znz.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eje.uphjek.com

[E21] 超长截断加省略号
来源：http://mvw.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uqs.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jwt.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hnc.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ofz.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ydo.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://add.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://skp.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zvp.sysykeji.top

[E22] 字节长度与字符长度
来源：http://ydh.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ejy.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iwd.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hjm.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kgy.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lzs.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xqv.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://tsu.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wzy.yfazqb.com

================================================================================
来源：http://omi.nwbrower.top

F. 文件与目录
来源：http://eap.cashguo.top

================================================================================
来源：http://cow.hywenlv.cn

[F01] 读取整个文件
来源：http://rxp.c1oappe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jvc.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://aht.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pyf.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hel.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cbu.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fal.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://zpx.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://guz.haohaochexian.top

[F02] 逐行读取文件
来源：http://bvs.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dlu.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vpl.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ola.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ehw.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fxn.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qzl.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ivs.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zqq.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://kni.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yjl.zdbjq.cn


<!-- 参考信息 -->