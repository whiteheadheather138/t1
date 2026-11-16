代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tar.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://unu.pycfn.com

[D17] 最大值与最小值
来源：http://awb.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://aqv.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://pvj.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gig.yueranfly.top

TS:   Math.max(...arr);
来源：http://rwl.ywan-chungtsiang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dqa.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dib.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://xus.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://odr.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://qgh.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xls.sweek.top

PHP:  array_merge(...$nested);
来源：http://olz.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eht.havefunace.top

TS:   nested.flat();
来源：http://rfd.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zau.yj20258.top

Go:   // 手写双层循环
来源：http://emy.tian-w.cn

Ruby: nested.flatten
来源：http://qja.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ehp.iojbl.cn

[D19] 按字段分组
来源：http://lpu.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zsn.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mru.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://llm.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dww.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xcs.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://sgi.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nkx.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mce.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://wmh.jqgfzy.top

Py:   Counter(arr)
来源：http://yhp.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://yuy.shangyingyoupin.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hzo.jlsjyb.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aly.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://chg.cheryme.top

Go:   // 手写 map[T]int
来源：http://ynt.hywenlv.cn

Ruby: arr.tally
来源：http://mmo.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ket.fktsv.cn

[D21] 判断是否包含某元素
来源：http://vdd.xingfuxueyuan.xyz

Py:   x in arr
来源：http://wpy.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://bdd.sxryk.cn

JS:   arr.includes(x)
来源：http://kxn.aizwys.cn

TS:   arr.includes(x)
来源：http://vlx.yangfankeji.com

Java: list.contains(x)
来源：http://vcn.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://esy.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://dvu.yuanzhike.top

C#:   list.Contains(x)
来源：http://ngh.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://pqt.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dds.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rnt.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hfa.hammf.cn

TS:   [...arr];
来源：http://zhb.yfazqb.com

Java: new ArrayList<>(list);
来源：http://uqt.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://tbi.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://kwg.haohaochexian.top

C#:   new List<int>(list);
来源：http://uwv.xuanzx.com

[D23] reduce 累积计算
来源：http://wum.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ntt.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mxo.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kog.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kfo.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bav.tianlin.xyz

Go:   // 手写循环
来源：http://wqf.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://phb.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qtv.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://rek.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uxw.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wkc.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dtv.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cjb.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eqz.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://snp.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jyw.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qyl.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://czi.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fmy.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://btp.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mvg.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sxw.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mxu.52xcode.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ria.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fry.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://epa.jqgfzy.top

[D26] 数组转字符串
来源：http://uor.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://zrf.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://dxr.chenlongwang.top

JS:   arr.join(", ")
来源：http://qcj.epnwcf.com

TS:   arr.join(", ")
来源：http://bdo.jiagoushi.top

Java: String.join(", ", list)
来源：http://onu.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://ncl.nwbrower.top

Ruby: arr.join(", ")
来源：http://etx.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://lpo.yongpay.top

================================================================================
来源：http://cia.zhiwuduotai.top

E. 字符串处理
来源：http://hwz.dashuyun.cn

================================================================================
来源：http://pfd.hnxiangtu.top

[E01] 拼接字符串
来源：http://jxn.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qin.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://smd.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ahk.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pfz.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sci.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://spc.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hql.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ond.nanxinkj.top

[E02] 重复字符串
来源：http://xnr.shangyingyoupin.top

Py:   "ab" * 3
来源：http://fum.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://fut.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://etn.shuidangran.top

TS:   "ab".repeat(3)
来源：http://tpd.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://ejj.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://sbv.chenzaomai.com

Ruby: "ab" * 3
来源：http://mxv.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://asc.hcnkem.com

[E03] 截取子串
来源：http://wxj.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mzn.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qvc.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sna.yvedp.cn

TS:   s.slice(1, 4)
来源：http://aip.meibo888.top

Java: s.substring(1, 4)
来源：http://mxb.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://akm.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://kep.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://hln.hesvh.cn

[E04] 查找子串位置
来源：http://pjj.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://vuy.yj20258.top

PHP:  strpos($s, "x");
来源：http://squ.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tlh.hnqzz.top

TS:   s.indexOf("x")
来源：http://qxz.cheryme.top

Java: s.indexOf("x")
来源：http://wbd.shuidangran.top

Go:   strings.Index(s, "x")
来源：http://pmi.zdqjudy.top

Ruby: s.index("x")
来源：http://owf.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://qjp.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jac.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vio.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nzg.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vpc.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gop.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zdt.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://csm.zhaomingkeji.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rtv.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ekn.hammf.cn

[E06] 替换子串
来源：http://ple.cqqwz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kgp.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://zec.guannengcc.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dvz.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://uhi.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hde.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fzq.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kbv.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://dok.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://arj.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ukz.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pbm.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ysc.jinghuilouyu.cn

TS:   s.split(",")
来源：http://mxs.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://pjn.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jrg.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://wmt.jqgufenzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://csg.yfazqb.com

[E08] 数组按分隔符合并
来源：http://lnr.ydzc1.top

Py:   ",".join(items)
来源：http://yut.tarul.cn

PHP:  implode(",", $items);
来源：http://cun.bjfxy.top

JS:   items.join(",")
来源：http://sle.wangdashe.top

TS:   items.join(",")
来源：http://jet.ctjpmb.com

Java: String.join(",", items)
来源：http://oky.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://wqi.cqqwz.cn

Ruby: items.join(",")
来源：http://xuc.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://gpp.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://dii.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://krm.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://znd.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://iaz.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://tqj.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://xnd.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vkk.yuxming.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wzf.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hmz.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://yxc.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sbm.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://olv.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://gpi.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://fto.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://gdm.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://iai.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hfd.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bsf.fanxiaobao.xyz

[E11] 反转字符串
来源：http://mhk.yueranfly.top

Py:   s[::-1]
来源：http://hqq.smart0.xyz

PHP:  strrev($s);
来源：http://gpn.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://ccu.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://trv.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://reg.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lkm.jinqigfzy.top

Ruby: s.reverse
来源：http://pfc.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://phd.redwolf501.top

[E12] 统计某字符出现次数
来源：http://rof.xylfe.cn

Py:   s.count("a")
来源：http://yxo.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://jzp.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://mmf.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://wxt.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ryh.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://age.zhengqikj.top

Ruby: s.count("a")
来源：http://shs.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://iah.andypj.xyz

[E13] 逐字符遍历
来源：http://buq.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://kzc.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lxz.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ypk.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://lia.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wzp.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jdz.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vxt.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xja.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://bwl.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://okv.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://brw.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tuz.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sxw.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hls.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eca.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fne.xuetiantiany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://asu.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://kps.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://csz.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yit.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qzs.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://upc.hongshengwenyu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qaa.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ijw.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bvc.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jfn.jyoumei.cn

[E16] 数字千分位
来源：http://ahw.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://zpj.ppjwa.cn

PHP:  number_format(1234567);
来源：http://qfj.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://gqz.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vcl.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gmd.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iyw.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hrz.sweek.top

C#:   1234567.ToString("N0")
来源：http://eyc.bbcook.cn

[E17] 首字母大写
来源：http://rkl.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://upe.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://izc.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iag.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oek.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hri.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bbm.yonumen.top

Ruby: s.capitalize
来源：http://wbg.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dvw.ydzc1.top

[E18] 模板占位符替换
来源：http://ubv.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jhb.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zxh.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zio.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://ais.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eqh.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bcx.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mvu.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://luq.yj20258888.top

[E19] 多行文本按行拆分
来源：http://epo.snrcjt.cn

Py:   s.splitlines()
来源：http://qfu.zhongyouzk.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rfk.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://puk.ydjk.org.cn

TS:   s.split(/\r?\n/)
来源：http://iix.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://khp.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://ppn.ehwqpu.com

Ruby: s.lines
来源：http://zuh.sysykeji.top

C#:   s.Split('\n')
来源：http://cav.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://etj.yueranfly.top

Py:   if not s:
来源：http://dqb.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kld.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qux.jinqigufen.top

TS:   if (s === "") {}
来源：http://whl.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://rjb.meibo888.top

Go:   if s == "" {}
来源：http://fjd.yangfankeji.com

Ruby: if s.empty?
来源：http://rfu.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aqk.yongpay.top

[E21] 超长截断加省略号
来源：http://sih.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zsu.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gqm.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ldj.wangshuangyany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mnb.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nho.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ovm.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jkg.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kfj.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://tee.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gll.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ifq.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qor.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hxq.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aia.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tsx.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://zab.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gru.ydzc1.top

================================================================================
来源：http://asu.fktsv.cn

F. 文件与目录
来源：http://gsa.chenlongwang.top

================================================================================
来源：http://utl.cashguo.top

[F01] 读取整个文件
来源：http://ivr.fzhhl.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gcx.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://xfq.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qaj.chenjidiqi.icu


<!-- 参考信息 -->