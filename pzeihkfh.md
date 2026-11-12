代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bos.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://cxi.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://pbt.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://yrh.tanke756.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pau.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://tdz.gaohongyu789.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pzw.zycfv.cn

TS:   nested.flat();
来源：http://rbv.gogol.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dnw.jqgufenzy.top

Go:   // 手写双层循环
来源：http://cxw.nanxuanxn.top

Ruby: nested.flatten
来源：http://jyu.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kty.jinqigufen.top

[D19] 按字段分组
来源：http://dmw.cqqwz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zde.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vod.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hxe.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://vdf.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mtu.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://rga.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bjd.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cwt.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://axv.bbcook.cn

Py:   Counter(arr)
来源：http://fgf.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://zsb.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://llx.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ubk.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kkw.guannengcc.top

Go:   // 手写 map[T]int
来源：http://cmo.shuidangran.top

Ruby: arr.tally
来源：http://nni.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gbf.cucudq.cn

[D21] 判断是否包含某元素
来源：http://igp.snrcjt.cn

Py:   x in arr
来源：http://wnv.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://mpk.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://spg.cashguo.top

TS:   arr.includes(x)
来源：http://gnb.birdmap.top

Java: list.contains(x)
来源：http://jof.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://svo.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://ikm.dianchejie.cn

C#:   list.Contains(x)
来源：http://czt.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://mth.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vmp.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sql.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://odw.epnwcf.com

TS:   [...arr];
来源：http://rzm.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://giv.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zyx.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://vxs.nanxuanxn.top

C#:   new List<int>(list);
来源：http://mpz.ydzc1.top

[D23] reduce 累积计算
来源：http://jhx.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://men.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eav.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://inb.ydzc1.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vqn.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://xet.yonumen.top

Go:   // 手写循环
来源：http://sqq.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nru.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xpx.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://tic.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lbr.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ayw.yj20258.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qri.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yiv.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hvq.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fns.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tjs.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zdm.shanyushiyangtech.top

[D25] Set 集合去重与交并差
来源：http://rno.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hvo.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://syv.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rki.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dvv.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mpl.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qfe.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zzu.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kjx.gotoacloud.top

[D26] 数组转字符串
来源：http://aao.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://ovu.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://vdt.0kj1m.cn

JS:   arr.join(", ")
来源：http://mha.zhoulong.xyz

TS:   arr.join(", ")
来源：http://anm.yvedp.cn

Java: String.join(", ", list)
来源：http://qcj.guannengcc.top

Go:   strings.Join(strs, ", ")
来源：http://drf.c1oappe.top

Ruby: arr.join(", ")
来源：http://yao.sysykeji.top

C#:   string.Join(", ", list)
来源：http://ajc.0kj1m.cn

================================================================================
来源：http://tqp.fktsv.cn

E. 字符串处理
来源：http://xsi.epnwcf.com

================================================================================
来源：http://sde.zhengqikj.top

[E01] 拼接字符串
来源：http://hjo.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dsq.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fgw.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://orm.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wzs.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yxd.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jrp.nwbrower.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tqf.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ugk.nwbrower.top

[E02] 重复字符串
来源：http://xvz.bjfxy.top

Py:   "ab" * 3
来源：http://fuy.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://wje.xuanzx.com

JS:   "ab".repeat(3)
来源：http://ypq.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://ptt.havefunace.top

Java: "ab".repeat(3)
来源：http://dyf.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://dks.ehwqpu.com

Ruby: "ab" * 3
来源：http://sgk.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kwm.shzxlz.cn

[E03] 截取子串
来源：http://axi.ctjpmb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hnt.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://enc.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xms.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://tko.fengsongda.top

Java: s.substring(1, 4)
来源：http://aqy.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fyn.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zli.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://acs.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://kni.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://npf.zhixingplan.top

PHP:  strpos($s, "x");
来源：http://mnu.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zxb.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://omd.meibo888.top

Java: s.indexOf("x")
来源：http://bpm.jlsjyb.cn

Go:   strings.Index(s, "x")
来源：http://ksw.yanxiufei.cn

Ruby: s.index("x")
来源：http://anq.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://vvg.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ynl.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tbo.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yrd.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eqg.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qmb.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nqs.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://feb.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fwn.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qev.yangfankeji.com

[E06] 替换子串
来源：http://roh.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mlr.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://jvl.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ffv.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://fox.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iys.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qvh.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cwy.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://idr.snrcjt.cn

[E07] 按分隔符拆分
来源：http://jgj.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://roh.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zfg.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://nck.ehwqpu.com

TS:   s.split(",")
来源：http://ucg.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://wgc.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iap.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://wyw.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lvd.zycfv.cn

[E08] 数组按分隔符合并
来源：http://brv.ivvv.top

Py:   ",".join(items)
来源：http://hmc.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://rev.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://xxt.pengpengdd.cyou

TS:   items.join(",")
来源：http://zvn.tanke756.top

Java: String.join(",", items)
来源：http://riq.316326.xyz

Go:   strings.Join(items, ",")
来源：http://ere.meibo888.top

Ruby: items.join(",")
来源：http://pvl.ehwqpu.com

C#:   string.Join(",", items)
来源：http://nzp.ybcxt.top

[E09] 去除所有空白字符
来源：http://lsi.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oia.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ijx.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://zan.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://tch.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://cac.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qtb.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://obw.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vsz.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://klh.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kks.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jcd.dianchejie.cn

JS:   "7".padStart(3, "0")
来源：http://ipf.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://nyc.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://ngc.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://crh.andypj.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ayr.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tqz.yvedp.cn

[E11] 反转字符串
来源：http://icj.epnwcf.com

Py:   s[::-1]
来源：http://jgv.guowangkeji.top

PHP:  strrev($s);
来源：http://fag.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://wwe.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://btm.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xuc.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rht.sysykeji.top

Ruby: s.reverse
来源：http://cxh.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xno.fktsv.cn

[E12] 统计某字符出现次数
来源：http://kim.xziqi.cn

Py:   s.count("a")
来源：http://urj.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://omn.fehbvm.com

JS:   s.split("a").length - 1
来源：http://poq.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://kol.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nbr.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://fwx.tanke756.top

Ruby: s.count("a")
来源：http://pev.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://lan.xuanzx.com

[E13] 逐字符遍历
来源：http://xol.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://xwd.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yys.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zwx.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wur.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gai.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://skm.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://owe.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kjz.andypj.xyz

[E14] URL 编码与 Base64
来源：http://sll.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uzo.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hqw.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hzv.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dif.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://afy.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://his.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zpf.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lgr.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://xyp.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://tfk.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wlc.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yrm.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nef.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ogh.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cgw.cqqwz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jbq.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pcg.havefunace.top

[E16] 数字千分位
来源：http://txc.zhengqikj.top

Py:   f"{1234567:,}"
来源：http://hva.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://sgn.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://nfs.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zgj.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nqz.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zyb.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fiy.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://ool.vehdjk.com

[E17] 首字母大写
来源：http://oqi.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ldv.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://stm.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lus.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gda.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gll.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xsz.hesvh.cn

Ruby: s.capitalize
来源：http://yaz.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kuy.zdbjq.cn

[E18] 模板占位符替换
来源：http://vbc.jiagoushi.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ubd.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dzn.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xnp.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ttw.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qme.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hcx.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zke.wangdashe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pwg.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://zlt.cdnleiting.top

Py:   s.splitlines()
来源：http://jgm.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tad.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://joq.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://rfu.guannengcc.top

Java: s.lines().toList()
来源：http://joa.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://anl.iojbl.cn

Ruby: s.lines
来源：http://eyv.uphjek.com

C#:   s.Split('\n')
来源：http://omi.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://scg.shanyushiyangkeji.top

Py:   if not s:
来源：http://dxg.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://avk.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nct.c1oappe.top

TS:   if (s === "") {}
来源：http://srq.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://blh.feifeiyinyue.top

Go:   if s == "" {}
来源：http://xor.hnqzz.top

Ruby: if s.empty?
来源：http://plg.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tzq.zhengqikj.top

[E21] 超长截断加省略号
来源：http://zbf.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://chz.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vch.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qkk.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://azf.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ixi.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://knf.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hwi.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kpn.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://nhw.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rif.sxryk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jpl.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vpg.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lmv.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aqc.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yuo.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://yhz.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qbv.chenjidiqi.icu

================================================================================
来源：http://afx.ybcxt.top

F. 文件与目录
来源：http://kvs.tian-w.cn

================================================================================
来源：http://uiq.jianghu66.top

[F01] 读取整个文件
来源：http://irj.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ngf.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://nuf.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fwq.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://egm.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kvh.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hvo.jianghu66.top

Ruby: File.read("a.txt")
来源：http://uir.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://mri.kuanghao11.cn

[F02] 逐行读取文件
来源：http://lkm.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wkr.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xdc.jiagoushi.top


<!-- 参考信息 -->