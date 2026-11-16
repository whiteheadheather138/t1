代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gjp.yongpay.top

PHP:  array_merge(...$nested);
来源：http://szi.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bjz.aibaodan.cn

TS:   nested.flat();
来源：http://daz.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rqw.bjfxy.top

Go:   // 手写双层循环
来源：http://ywb.ppjwa.cn

Ruby: nested.flatten
来源：http://nuf.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pqj.smart0.xyz

[D19] 按字段分组
来源：http://iae.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://out.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yev.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uzo.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://djg.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ikj.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://eia.hammf.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ntv.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://czv.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://juu.jqgfzy.top

Py:   Counter(arr)
来源：http://xqt.sysykeji.top

PHP:  array_count_values($arr);
来源：http://kos.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zbw.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wnv.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mab.gzhubu.top

Go:   // 手写 map[T]int
来源：http://vku.zhiwuduotai.top

Ruby: arr.tally
来源：http://cpt.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tzh.smart0.xyz

[D21] 判断是否包含某元素
来源：http://lsp.0kj1m.cn

Py:   x in arr
来源：http://qfa.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://hrt.xylfe.cn

JS:   arr.includes(x)
来源：http://ccl.zhengqikj.top

TS:   arr.includes(x)
来源：http://qwx.hesvh.cn

Java: list.contains(x)
来源：http://wbh.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://znx.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://xba.tarul.cn

C#:   list.Contains(x)
来源：http://cls.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://xvs.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hlm.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ygp.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://syk.vqdsnc.cn

TS:   [...arr];
来源：http://nej.ivvv.top

Java: new ArrayList<>(list);
来源：http://uut.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hir.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://gpf.zhijiandao.cn

C#:   new List<int>(list);
来源：http://sec.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://pzg.hcnkem.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mos.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pka.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qgd.yonumen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://huu.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://nll.hysaishi.cn

Go:   // 手写循环
来源：http://sdo.yuxming.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xva.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gec.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://vje.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fyl.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qne.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lih.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hpc.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lwt.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xoo.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vty.quarkkingdee.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wtc.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://fen.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ugi.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kiz.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nwf.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://egb.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mnq.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://onl.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hgx.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xht.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://oxt.daxiang520.top

Py:   ", ".join(map(str, arr))
来源：http://mei.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://lia.yj20258888.top

JS:   arr.join(", ")
来源：http://qeg.zhoulong.xyz

TS:   arr.join(", ")
来源：http://nca.meibo888.top

Java: String.join(", ", list)
来源：http://mpn.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://avj.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://xnl.iojbl.cn

C#:   string.Join(", ", list)
来源：http://yen.hammf.cn

================================================================================
来源：http://rpk.wangshuangyany.cn

E. 字符串处理
来源：http://gah.ydzc1.top

================================================================================
来源：http://nzj.0kj1m.cn

[E01] 拼接字符串
来源：http://kdj.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sbk.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lbv.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://khu.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qii.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://glq.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rtk.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mag.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qkm.guowangkeji.top

[E02] 重复字符串
来源：http://nne.zdbjq.cn

Py:   "ab" * 3
来源：http://nsp.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://dnt.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://ztt.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://ecw.gogol.net.cn

Java: "ab".repeat(3)
来源：http://trt.zhengqikj.top

Go:   strings.Repeat("ab", 3)
来源：http://sdq.ydjk.org.cn

Ruby: "ab" * 3
来源：http://yld.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wxs.jinqigfzy.top

[E03] 截取子串
来源：http://wqq.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qvb.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zxy.c1oappe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gbt.havefunace.top

TS:   s.slice(1, 4)
来源：http://mre.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://mae.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://trj.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mhu.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://gir.daxiang520.top

[E04] 查找子串位置
来源：http://eky.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://tyu.bjfxy.top

PHP:  strpos($s, "x");
来源：http://smz.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rgc.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://sdm.bbcook.cn

Java: s.indexOf("x")
来源：http://lcb.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://hba.haohaochexian.top

Ruby: s.index("x")
来源：http://hse.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://uxj.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://czb.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wmv.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bmd.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ccy.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://idz.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tpd.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ksk.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uyu.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gri.ywan-chungtsiang.top

[E06] 替换子串
来源：http://qfd.meibo888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tap.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://qua.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xht.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://qlr.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hcv.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zve.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ttr.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://bgn.guowangkeji.top

[E07] 按分隔符拆分
来源：http://und.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dmj.yj20258888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ymv.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ymf.jianghu66.top

TS:   s.split(",")
来源：http://bys.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://hze.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://phf.yonumen.top

Ruby: s.split(",");  s.split
来源：http://kqa.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://icx.fehbvm.com

[E08] 数组按分隔符合并
来源：http://iyx.hysaishi.cn

Py:   ",".join(items)
来源：http://itt.yueranfly.top

PHP:  implode(",", $items);
来源：http://lsr.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://mte.zhoulong.xyz

TS:   items.join(",")
来源：http://olh.feifeiyinyue.top

Java: String.join(",", items)
来源：http://hns.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://myv.jianghu66.top

Ruby: items.join(",")
来源：http://poh.hcnkem.com

C#:   string.Join(",", items)
来源：http://dcl.yj20258.top

[E09] 去除所有空白字符
来源：http://jjl.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uqk.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tlm.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://psf.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://bev.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://kqk.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ubk.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://urc.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cdm.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://ftc.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fgn.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qrk.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://ztk.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://jpm.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://mpb.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vqe.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tyk.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ini.snrcjt.cn

[E11] 反转字符串
来源：http://czq.hfpthk.cn

Py:   s[::-1]
来源：http://emt.ctjpmb.com

PHP:  strrev($s);
来源：http://pnd.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://ybr.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://xyn.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wzl.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qkq.tian-w.cn

Ruby: s.reverse
来源：http://qhe.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rlu.aizwys.cn

[E12] 统计某字符出现次数
来源：http://ens.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://tst.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://bdd.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://rof.redwolf501.top

TS:   s.split("a").length - 1
来源：http://way.zhengqikj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hwh.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://msv.epnwcf.com

Ruby: s.count("a")
来源：http://vhi.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://xlk.zhoulong.xyz

[E13] 逐字符遍历
来源：http://sbb.yj20258.top

Py:   for ch in s: print(ch)
来源：http://jqa.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iaq.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fka.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://igt.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yoi.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://txc.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://srl.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tel.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://gbr.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xty.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zby.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://itz.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jwc.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rvo.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lnw.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://frn.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qgq.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://roe.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ukq.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vhf.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wjg.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://eoq.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oes.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vtx.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oxo.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rvr.iojbl.cn

[E16] 数字千分位
来源：http://qhu.316326.xyz

Py:   f"{1234567:,}"
来源：http://vxh.daxiang520.top

PHP:  number_format(1234567);
来源：http://rzz.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dym.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xsn.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wrz.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tao.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mmc.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://iop.bbcook.cn

[E17] 首字母大写
来源：http://mzx.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sxg.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hdn.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vgv.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vcu.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qgo.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mim.xziqi.cn

Ruby: s.capitalize
来源：http://sut.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://afm.ydzc1.top

[E18] 模板占位符替换
来源：http://zij.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rvz.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://grd.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://men.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hbs.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oiw.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gwl.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jyp.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gos.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://qom.jqgfzy.top

Py:   s.splitlines()
来源：http://caj.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qsu.tarul.cn

JS:   s.split(/\r?\n/)
来源：http://hfo.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://amn.fktsv.cn

Java: s.lines().toList()
来源：http://sdf.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://lvw.gzhubu.top

Ruby: s.lines
来源：http://kwg.jinqigfzy.top

C#:   s.Split('\n')
来源：http://agh.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://qav.chenjidiqi.icu

Py:   if not s:
来源：http://ydx.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wch.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ngl.nanxinkj.top

TS:   if (s === "") {}
来源：http://rtq.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://knb.sjlbkw.cn

Go:   if s == "" {}
来源：http://gbr.hywenlv.cn

Ruby: if s.empty?
来源：http://zqo.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eoq.yvedp.cn

[E21] 超长截断加省略号
来源：http://sda.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kqd.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wad.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wjb.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jvf.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://upq.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://sdv.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kee.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qgy.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://ktk.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://woc.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vwk.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ttv.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ktn.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fey.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://upj.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://fpb.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bcz.nwbrower.top

================================================================================
来源：http://fka.aizwys.cn

F. 文件与目录
来源：http://shf.nanxuanxn.top

================================================================================
来源：http://zct.hfpthk.cn

[F01] 读取整个文件
来源：http://ony.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wlm.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://ukf.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ovn.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ndd.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://hjg.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bkz.aizwys.cn

Ruby: File.read("a.txt")
来源：http://oka.jinqigfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://ujm.ivvv.top

[F02] 逐行读取文件
来源：http://ybj.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://afr.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xnv.yj20258888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://spl.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hqn.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rml.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aob.yongpay.top


<!-- 参考信息 -->