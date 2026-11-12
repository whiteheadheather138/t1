代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sxv.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://drp.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://fze.cashguo.top

[D18] 扁平化嵌套数组
来源：http://ujd.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dkf.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://itx.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://trc.aibaodan.cn

TS:   nested.flat();
来源：http://jwa.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://etd.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://jdz.xuanzx.com

Ruby: nested.flatten
来源：http://vmv.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ooi.aizwys.cn

[D19] 按字段分组
来源：http://tpu.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xdu.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nsf.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://irj.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://voo.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mon.nwbrower.top

Go:   // 手写 map[string][]T
来源：http://has.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rie.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ywa.yj202588.top

[D20] 统计每个元素出现次数
来源：http://doy.nanxinkj.top

Py:   Counter(arr)
来源：http://drq.birdmap.top

PHP:  array_count_values($arr);
来源：http://rpg.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fjo.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eex.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ogj.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://ifu.smart0.xyz

Ruby: arr.tally
来源：http://ixp.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zrd.gzhubu.top

[D21] 判断是否包含某元素
来源：http://gcb.ehwqpu.com

Py:   x in arr
来源：http://rep.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://kow.nanxuanxn.top

JS:   arr.includes(x)
来源：http://fld.epnwcf.com

TS:   arr.includes(x)
来源：http://wjo.sxryk.cn

Java: list.contains(x)
来源：http://ilk.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://kel.vehdjk.com

Ruby: arr.include?(x)
来源：http://yvv.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://mol.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://bmk.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sbi.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nac.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rmf.mhx1999.top

TS:   [...arr];
来源：http://kdj.hnqzz.top

Java: new ArrayList<>(list);
来源：http://dah.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oag.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://qzy.jyoumei.cn

C#:   new List<int>(list);
来源：http://mbi.gzhubu.top

[D23] reduce 累积计算
来源：http://hff.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fry.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ayu.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rgq.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aiz.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://eal.cashguo.top

Go:   // 手写循环
来源：http://dzr.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hsh.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jmb.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://mzz.kuanghao11.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://slu.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hcv.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pcg.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hht.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oqr.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bqe.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qck.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ulz.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://nss.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zil.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nbk.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://itv.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qem.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fbk.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gzy.bbcook.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://esl.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://knq.zhoulong.xyz

[D26] 数组转字符串
来源：http://nub.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://dnd.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://dff.zhengqikj.top

JS:   arr.join(", ")
来源：http://lqn.yongpay.top

TS:   arr.join(", ")
来源：http://vzx.daria6918.cn

Java: String.join(", ", list)
来源：http://tyw.bjfxy.top

Go:   strings.Join(strs, ", ")
来源：http://lxk.uphjek.com

Ruby: arr.join(", ")
来源：http://yvj.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://hum.fktsv.cn

================================================================================
来源：http://jjj.yj20258888.top

E. 字符串处理
来源：http://rwy.hywenlv.cn

================================================================================
来源：http://jux.bjfxy.top

[E01] 拼接字符串
来源：http://unw.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://spw.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mdi.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tuk.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fym.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ztb.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ovs.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tpi.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xpl.0kj1m.cn

[E02] 重复字符串
来源：http://isb.sxryk.cn

Py:   "ab" * 3
来源：http://hlq.svipenyu.cn

PHP:  str_repeat("ab", 3);
来源：http://gax.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://gly.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://rmd.9152youxi.cn

Java: "ab".repeat(3)
来源：http://cfo.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://rtr.uphjek.com

Ruby: "ab" * 3
来源：http://irx.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://crg.tarul.cn

[E03] 截取子串
来源：http://oqo.aizwys.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://umy.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://btz.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tim.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://rqb.yvedp.cn

Java: s.substring(1, 4)
来源：http://irz.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iva.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://ojz.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://cdw.yuxming.cn

[E04] 查找子串位置
来源：http://gvh.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://hgw.guannengcc.top

PHP:  strpos($s, "x");
来源：http://euw.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://loi.daria6918.cn

TS:   s.indexOf("x")
来源：http://wut.daria6918.cn

Java: s.indexOf("x")
来源：http://pfb.ivvv.top

Go:   strings.Index(s, "x")
来源：http://ulm.pycfn.com

Ruby: s.index("x")
来源：http://ytp.cucudq.cn

C#:   s.IndexOf("x")
来源：http://lyz.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uqv.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zmx.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://esp.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vad.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://dsx.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hrq.iojbl.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jwf.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yyu.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mkk.svipenyu.cn

[E06] 替换子串
来源：http://igu.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wtk.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://gjv.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fry.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://gjf.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://muk.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kpj.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ahs.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://gnv.sufxvd.cn

[E07] 按分隔符拆分
来源：http://ohq.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ccp.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fof.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://voz.andypj.xyz

TS:   s.split(",")
来源：http://khj.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://wos.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://min.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://xkt.ydzc1.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nlo.sweek.top

[E08] 数组按分隔符合并
来源：http://wfh.wangdashe.top

Py:   ",".join(items)
来源：http://ovx.gogol.net.cn

PHP:  implode(",", $items);
来源：http://vtc.wangshuangyany.cn

JS:   items.join(",")
来源：http://xqy.hammf.cn

TS:   items.join(",")
来源：http://fsu.hysaishi.cn

Java: String.join(",", items)
来源：http://kfy.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://gkr.316326.xyz

Ruby: items.join(",")
来源：http://def.jyoumei.cn

C#:   string.Join(",", items)
来源：http://fwh.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://ulm.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qda.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sra.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://wik.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://qpd.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://aam.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zil.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://hlb.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ftf.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://ksq.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://czy.shanyushiyangtech.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rau.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://wih.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://eql.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://vgr.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://hjz.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yjo.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gnf.guannengcc.top

[E11] 反转字符串
来源：http://hxp.tian-w.cn

Py:   s[::-1]
来源：http://dsz.xinyue.icu

PHP:  strrev($s);
来源：http://thp.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://dyh.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://qov.shanyushiyangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kaz.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gdc.chenzaomai.com

Ruby: s.reverse
来源：http://bac.jiagoushi.top

C#:   new string(s.Reverse().ToArray())
来源：http://gjw.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://cnk.guowangkeji.top

Py:   s.count("a")
来源：http://nlz.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://lzm.havefunace.top

JS:   s.split("a").length - 1
来源：http://xri.yj202588.top

TS:   s.split("a").length - 1
来源：http://ssa.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wwd.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://fyq.chenlongwang.top

Ruby: s.count("a")
来源：http://xjw.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://qca.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://bkx.tarul.cn

Py:   for ch in s: print(ch)
来源：http://aaz.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ahx.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cuc.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xgn.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xxy.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fzo.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oaz.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kwk.hammf.cn

[E14] URL 编码与 Base64
来源：http://veo.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ynl.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://erq.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://npz.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qse.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://olh.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nyw.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aoi.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lpo.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://kho.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xri.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gcd.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qij.9152youxi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aic.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sck.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rpd.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uxy.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jdv.yvedp.cn

[E16] 数字千分位
来源：http://saf.hcnkem.com

Py:   f"{1234567:,}"
来源：http://dza.bjfxy.top

PHP:  number_format(1234567);
来源：http://uxk.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://gfl.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qbn.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eza.sufxvd.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ibi.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uci.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://zec.pycfn.com

[E17] 首字母大写
来源：http://ahm.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xqt.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lri.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zgd.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fyo.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uss.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vaz.tianlin.xyz

Ruby: s.capitalize
来源：http://ddr.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kuj.hnqzz.top

[E18] 模板占位符替换
来源：http://sqr.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ayn.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jvv.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ptl.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ftv.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ohv.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wjr.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://thu.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yck.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://nzj.zhongyouzk.top

Py:   s.splitlines()
来源：http://koo.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bdq.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://mvk.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://dvm.zdbjq.cn

Java: s.lines().toList()
来源：http://pob.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://rtb.sysykeji.top

Ruby: s.lines
来源：http://ftd.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://yyj.cucudq.cn

[E20] 判断字符串是否为空
来源：http://mop.fengsongda.top

Py:   if not s:
来源：http://pta.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hkm.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sjk.xuanzx.com

TS:   if (s === "") {}
来源：http://ttz.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://aok.ydzc1.top

Go:   if s == "" {}
来源：http://rje.0kj1m.cn

Ruby: if s.empty?
来源：http://fgh.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vqx.epnwcf.com

[E21] 超长截断加省略号
来源：http://cuh.cheryme.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hzn.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bba.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tdn.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://udo.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sss.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://cdu.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aab.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nyb.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://izb.zhixingplan.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qhz.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wwc.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://urp.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fus.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xgk.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bqy.52xcode.cn

Ruby: s.bytesize;  s.length
来源：http://ewj.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nkt.jqgufenzy.top

================================================================================
来源：http://pov.aizwys.cn

F. 文件与目录
来源：http://wia.pengpengdd.cyou

================================================================================
来源：http://yuu.daria6918.cn

[F01] 读取整个文件
来源：http://qpy.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mrd.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://van.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pri.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sdb.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tla.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nac.havefunace.top

Ruby: File.read("a.txt")
来源：http://wug.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://ikv.snrcjt.cn

[F02] 逐行读取文件
来源：http://qse.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qew.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cgl.jinqigufen.top


<!-- 参考信息 -->