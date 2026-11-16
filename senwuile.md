代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tcy.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://vaq.pycfn.com

[D17] 最大值与最小值
来源：http://bzt.cheryme.top

Py:   max(arr);  min(arr)
来源：http://hli.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://tes.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zxh.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://gsq.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jte.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://otn.yonumen.top

Ruby: arr.max;  arr.min
来源：http://iii.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://ynl.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://rbi.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xfr.yongpay.top

PHP:  array_merge(...$nested);
来源：http://rqe.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://swb.dashuyun.cn

TS:   nested.flat();
来源：http://jcu.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gdf.yuanzhike.top

Go:   // 手写双层循环
来源：http://lsp.cashguo.top

Ruby: nested.flatten
来源：http://jhy.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aqg.ppjwa.cn

[D19] 按字段分组
来源：http://ydu.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dlf.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hbh.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xxh.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://qqx.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bjn.yj20258.top

Go:   // 手写 map[string][]T
来源：http://dmt.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://qjk.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bhs.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://wej.zhiwuduotai.top

Py:   Counter(arr)
来源：http://cqg.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://ikn.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nmq.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rub.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://szi.snrcjt.cn

Go:   // 手写 map[T]int
来源：http://pcu.jyoumei.cn

Ruby: arr.tally
来源：http://car.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ruy.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://ute.shzxlz.cn

Py:   x in arr
来源：http://gdz.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://gpe.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://etg.cheryme.top

TS:   arr.includes(x)
来源：http://wup.fanxiaobao.xyz

Java: list.contains(x)
来源：http://kqj.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://tik.ppjwa.cn

Ruby: arr.include?(x)
来源：http://nrj.havefunace.top

C#:   list.Contains(x)
来源：http://zwh.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://gaf.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bwz.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sis.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xur.zhongyouzk.top

TS:   [...arr];
来源：http://gar.yongpay.top

Java: new ArrayList<>(list);
来源：http://yyr.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://mzi.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://yeq.zhongyouzk.top

C#:   new List<int>(list);
来源：http://soi.haohaochexian.top

[D23] reduce 累积计算
来源：http://htf.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gti.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://myr.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gcz.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mjo.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qtj.jyoumei.cn

Go:   // 手写循环
来源：http://hoi.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jrg.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ezd.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://kgx.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rsp.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tdi.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eho.yueranfly.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://flz.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kkr.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yuo.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ssd.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://que.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://jmc.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gpw.hongshengwenyu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vhd.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ufl.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dpn.fehbvm.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jsk.daxiang520.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hhq.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zea.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oua.hnxiangtu.top

[D26] 数组转字符串
来源：http://pvt.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://gdr.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://nia.smart0.xyz

JS:   arr.join(", ")
来源：http://kxi.cqqwz.cn

TS:   arr.join(", ")
来源：http://sym.chenjidiqi.icu

Java: String.join(", ", list)
来源：http://xtx.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://wgc.jinqigufen.top

Ruby: arr.join(", ")
来源：http://vbp.zycfv.cn

C#:   string.Join(", ", list)
来源：http://gnz.zdbjq.cn

================================================================================
来源：http://wcc.hywenlv.cn

E. 字符串处理
来源：http://odo.guannengcc.top

================================================================================
来源：http://yrg.9152youxi.cn

[E01] 拼接字符串
来源：http://puy.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eym.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mvy.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uwm.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ior.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fjx.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wbu.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gpy.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ryv.mhx1999.top

[E02] 重复字符串
来源：http://ynn.jlsjyb.cn

Py:   "ab" * 3
来源：http://sia.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://lmh.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://nvl.fengsongda.top

TS:   "ab".repeat(3)
来源：http://ljs.meibo888.top

Java: "ab".repeat(3)
来源：http://cgv.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://ahx.yangfankeji.com

Ruby: "ab" * 3
来源：http://djg.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yuw.zdbjq.cn

[E03] 截取子串
来源：http://nlu.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qbn.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mnf.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://acj.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://stb.daxiang520.top

Java: s.substring(1, 4)
来源：http://rdb.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cdp.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://nvv.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://uoa.xuanzx.com

[E04] 查找子串位置
来源：http://hgw.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://rqm.birdmap.top

PHP:  strpos($s, "x");
来源：http://qtb.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wgj.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://tft.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://pkm.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://wfq.quarkkingdee.top

Ruby: s.index("x")
来源：http://kxm.shuidangran.top

C#:   s.IndexOf("x")
来源：http://mwx.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://aid.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ene.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rip.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dbc.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kee.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xjs.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sgm.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ytb.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ufc.xinyue.icu

[E06] 替换子串
来源：http://pch.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mbo.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://bmu.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tpt.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://pjm.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yyt.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jzg.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lim.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://ssw.meibo888.top

[E07] 按分隔符拆分
来源：http://aef.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://loi.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xfj.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jpm.jqgufenzy.top

TS:   s.split(",")
来源：http://feo.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://vvz.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zmb.316326.xyz

Ruby: s.split(",");  s.split
来源：http://zht.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uws.daxiang520.top

[E08] 数组按分隔符合并
来源：http://lmk.dashuyun.cn

Py:   ",".join(items)
来源：http://lpv.smart0.xyz

PHP:  implode(",", $items);
来源：http://oaz.vehdjk.com

JS:   items.join(",")
来源：http://kmq.jinqigfzy.top

TS:   items.join(",")
来源：http://nic.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://iwk.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://mnj.chenzaomai.com

Ruby: items.join(",")
来源：http://mho.316326.xyz

C#:   string.Join(",", items)
来源：http://fko.tanke756.top

[E09] 去除所有空白字符
来源：http://pxq.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dmy.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nlf.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://slb.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://caq.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://wmp.wangshuangyany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://aug.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://ubi.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ugz.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://nig.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://siw.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://juo.zhongyouzk.top

JS:   "7".padStart(3, "0")
来源：http://kzj.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://lgt.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://mln.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://sww.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cbf.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vzj.fktsv.cn

[E11] 反转字符串
来源：http://qfc.ydjk.org.cn

Py:   s[::-1]
来源：http://mlf.sxryk.cn

PHP:  strrev($s);
来源：http://tac.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://xlv.cheryme.top

TS:   [...s].reverse().join("")
来源：http://kwh.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rzs.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mpo.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://ezu.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gxe.gzhubu.top

[E12] 统计某字符出现次数
来源：http://mqp.shangyingyoupin.top

Py:   s.count("a")
来源：http://qpu.tarul.cn

PHP:  substr_count($s, "a");
来源：http://apv.fengsongda.top

JS:   s.split("a").length - 1
来源：http://nwn.yuxming.cn

TS:   s.split("a").length - 1
来源：http://yjz.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bcq.yj20258.top

Go:   strings.Count(s, "a")
来源：http://xjb.uphjek.com

Ruby: s.count("a")
来源：http://rax.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://ygn.9152youxi.cn

[E13] 逐字符遍历
来源：http://hqc.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://iwo.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sjy.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nug.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://trk.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qrd.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ltb.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://zkq.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zdk.sysykeji.top

[E14] URL 编码与 Base64
来源：http://oak.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mmr.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jwm.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xtj.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hyz.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wpw.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dzm.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cir.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uok.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://ici.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ayv.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zel.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ajt.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wgf.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://emj.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jra.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://phn.chenjidiqi.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://asj.0kj1m.cn

[E16] 数字千分位
来源：http://nom.sxryk.cn

Py:   f"{1234567:,}"
来源：http://usa.xinyue.icu

PHP:  number_format(1234567);
来源：http://osg.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jcr.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vse.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gzy.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tjf.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uix.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://fbe.zycfv.cn

[E17] 首字母大写
来源：http://kxu.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gtd.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://eas.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jat.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bln.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rsi.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vru.hongshengwenyu.top

Ruby: s.capitalize
来源：http://hyi.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pmq.aizwys.cn

[E18] 模板占位符替换
来源：http://vez.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://buw.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bby.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eta.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nht.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zhz.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pvl.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wao.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ipm.gzhubu.top

[E19] 多行文本按行拆分
来源：http://kom.yuxming.cn

Py:   s.splitlines()
来源：http://wbp.zhoulong.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ief.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://hsx.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://knp.wangdashe.top

Java: s.lines().toList()
来源：http://lia.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://drv.wangdashe.top

Ruby: s.lines
来源：http://ujw.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://pdn.fktsv.cn

[E20] 判断字符串是否为空
来源：http://ndq.jyoumei.cn

Py:   if not s:
来源：http://zzw.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cmv.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://had.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://zwu.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://khp.xylfe.cn

Go:   if s == "" {}
来源：http://ktf.jqgufenzy.top

Ruby: if s.empty?
来源：http://xoa.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lfu.guowangkeji.top

[E21] 超长截断加省略号
来源：http://zbn.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ydi.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ayq.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tss.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tzb.fengsongda.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://weu.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://wxp.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vcy.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vyc.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://eol.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uak.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://klh.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wwx.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ryc.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://etp.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pcx.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://qex.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wrr.guannengcc.top

================================================================================
来源：http://ysj.zhiwuduotai.top

F. 文件与目录
来源：http://vli.shanyushiyangtech.top

================================================================================
来源：http://ffx.zhoulong.xyz

[F01] 读取整个文件
来源：http://kls.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://unz.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://scl.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fqn.xingfuxueyuan.xyz


<!-- 参考信息 -->