代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pbq.jqgfzy.top

Go:   // 手写双层循环
来源：http://tmg.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://ymk.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sbh.xziqi.cn

[D19] 按字段分组
来源：http://hwa.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gij.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eau.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nin.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ifs.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ude.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://kao.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ted.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://box.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://fxy.pengpengdd.cyou

Py:   Counter(arr)
来源：http://ihi.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://vjp.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nce.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lvq.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qyd.epnwcf.com

Go:   // 手写 map[T]int
来源：http://lni.smart0.xyz

Ruby: arr.tally
来源：http://nph.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qkr.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://kqm.havefunace.top

Py:   x in arr
来源：http://uej.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://hku.zdqjudy.top

JS:   arr.includes(x)
来源：http://ine.zhongyouzk.top

TS:   arr.includes(x)
来源：http://jnu.gaohongyu789.top

Java: list.contains(x)
来源：http://wqn.cqqwz.cn

Go:   slices.Contains(arr, x)
来源：http://dfb.fzhhl.top

Ruby: arr.include?(x)
来源：http://qbv.nanxuanxn.top

C#:   list.Contains(x)
来源：http://bbx.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://cmx.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ugd.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sow.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wki.shuidangran.top

TS:   [...arr];
来源：http://pjw.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://lbz.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://qbh.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://rxg.havefunace.top

C#:   new List<int>(list);
来源：http://heh.zhongyouzk.top

[D23] reduce 累积计算
来源：http://hdn.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qcf.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uuo.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fso.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://irf.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lxa.mhx1999.top

Go:   // 手写循环
来源：http://euy.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pca.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mom.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://pxt.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://axw.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nlx.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://izo.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://azd.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hba.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jor.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zmi.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ymt.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://zdo.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yyi.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ekt.yvedp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bte.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hdw.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hvi.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gjf.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yrm.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bmy.ydzc1.top

[D26] 数组转字符串
来源：http://gzs.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://qtm.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://hhj.hfpthk.cn

JS:   arr.join(", ")
来源：http://wht.cqqwz.cn

TS:   arr.join(", ")
来源：http://qsf.cashguo.top

Java: String.join(", ", list)
来源：http://jde.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://qxh.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://fjh.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://eqs.gotoacloud.top

================================================================================
来源：http://zxy.ywan-chungtsiang.top

E. 字符串处理
来源：http://oqj.kuanghao11.cn

================================================================================
来源：http://tfp.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://shu.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nqn.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uwu.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fsj.aibaodan.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qby.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://brv.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ras.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pbq.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ngd.haohaochexian.top

[E02] 重复字符串
来源：http://xey.gotoacloud.top

Py:   "ab" * 3
来源：http://utx.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://fan.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://fqe.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://fgs.gzhubu.top

Java: "ab".repeat(3)
来源：http://scz.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://cmw.hnxiangtu.top

Ruby: "ab" * 3
来源：http://jow.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qpc.ppjwa.cn

[E03] 截取子串
来源：http://uer.chenjidiqi.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gox.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qcf.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lir.yonumen.top

TS:   s.slice(1, 4)
来源：http://tvi.daxiang520.top

Java: s.substring(1, 4)
来源：http://bbp.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gbv.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://syx.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://cmz.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://xfw.hnxiangtu.top

Py:   s.find("x");  s.index("x")
来源：http://sbk.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://vek.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://plh.meibo888.top

TS:   s.indexOf("x")
来源：http://czb.gzhubu.top

Java: s.indexOf("x")
来源：http://mkn.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://day.shuidangran.top

Ruby: s.index("x")
来源：http://esa.yueranfly.top

C#:   s.IndexOf("x")
来源：http://mxx.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nqs.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hpm.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ccy.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://edf.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jyu.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dla.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nqd.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://koc.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zcb.dianchejie.cn

[E06] 替换子串
来源：http://vgi.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yuk.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://dxk.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ggc.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://lop.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lik.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yrq.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jmm.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://gja.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://lvo.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ase.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xpd.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zbb.yj20258.top

TS:   s.split(",")
来源：http://zwc.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zky.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dku.uphjek.com

Ruby: s.split(",");  s.split
来源：http://qme.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jvn.epnwcf.com

[E08] 数组按分隔符合并
来源：http://anj.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://nvj.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://ppv.wangshuangyany.cn

JS:   items.join(",")
来源：http://osg.shzxlz.cn

TS:   items.join(",")
来源：http://mdj.gotoacloud.top

Java: String.join(",", items)
来源：http://umo.meibo888.top

Go:   strings.Join(items, ",")
来源：http://gal.aibaodan.cn

Ruby: items.join(",")
来源：http://kwg.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://zrv.sxryk.cn

[E09] 去除所有空白字符
来源：http://psx.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tvk.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tgt.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://pct.dashuyun.cn

TS:   s.replace(/\s+/g, "")
来源：http://qwy.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://iny.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ebu.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://msi.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://prg.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://ojr.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://spu.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tyu.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://kgr.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://zsw.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://fhn.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://agy.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nhq.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hhz.zhoulong.xyz

[E11] 反转字符串
来源：http://fvh.hnqzz.top

Py:   s[::-1]
来源：http://hce.mhx1999.top

PHP:  strrev($s);
来源：http://jew.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://kce.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://nlv.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://utb.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://obo.xinyue.icu

Ruby: s.reverse
来源：http://til.jiagoushi.top

C#:   new string(s.Reverse().ToArray())
来源：http://efd.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://vcv.daria6918.cn

Py:   s.count("a")
来源：http://wky.shanyushiyangtech.top

PHP:  substr_count($s, "a");
来源：http://cne.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://mdf.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://bse.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ies.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://adu.yongpay.top

Ruby: s.count("a")
来源：http://ubx.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://rpw.ppjwa.cn

[E13] 逐字符遍历
来源：http://qvw.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://uoc.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://upl.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cbl.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ooc.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mxx.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ncd.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mlc.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oyi.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://aln.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aso.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bsm.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fxo.hfpthk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uwk.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lll.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hmk.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hbb.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cqf.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://nfq.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hll.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zeh.feifeiyinyue.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ukp.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eff.yuxming.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vav.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rfw.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://feh.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cpf.wangdashe.top

[E16] 数字千分位
来源：http://sdt.316326.xyz

Py:   f"{1234567:,}"
来源：http://iyj.daria6918.cn

PHP:  number_format(1234567);
来源：http://aib.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bgl.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://sef.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hlt.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hbv.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xlh.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://ssx.hcnkem.com

[E17] 首字母大写
来源：http://iya.yfazqb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dns.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://znp.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wkm.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ybx.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yaj.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ewo.zhaomingkeji.xyz

Ruby: s.capitalize
来源：http://blt.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dxk.zhijiandao.cn

[E18] 模板占位符替换
来源：http://lmj.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kpw.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cfz.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hgi.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://goz.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uxe.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dqe.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lot.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zfu.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://svt.snrcjt.cn

Py:   s.splitlines()
来源：http://lac.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xoz.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://htj.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://mdk.zycfv.cn

Java: s.lines().toList()
来源：http://dbf.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://vti.guannengcc.top

Ruby: s.lines
来源：http://vab.ivvv.top

C#:   s.Split('\n')
来源：http://naa.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://rfn.jinqigufen.top

Py:   if not s:
来源：http://yrl.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ltj.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pxf.sufxvd.cn

TS:   if (s === "") {}
来源：http://ozn.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://zym.yangfankeji.com

Go:   if s == "" {}
来源：http://dep.yj20258888.top

Ruby: if s.empty?
来源：http://bzy.svipenyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ytl.nwbrower.top

[E21] 超长截断加省略号
来源：http://oez.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ljx.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xob.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yqd.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ecm.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eop.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://aoq.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ptm.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://twx.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://ouo.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://new.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zdj.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yif.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qqf.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aqn.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qtj.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://lif.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ebk.zhongyouzk.top

================================================================================
来源：http://msf.sjlbkw.cn

F. 文件与目录
来源：http://ney.sysykeji.top

================================================================================
来源：http://ber.birdmap.top

[F01] 读取整个文件
来源：http://srh.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pnt.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://ibw.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qgp.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://piq.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ntn.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ltn.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://yjc.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://xjz.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://pwa.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blj.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yyi.0kj1m.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://can.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kjc.0kj1m.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rhf.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jxc.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yis.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mrd.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://uue.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gjn.vqdsnc.cn


<!-- 参考信息 -->