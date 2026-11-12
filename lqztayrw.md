代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mci.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://tzu.nanxuanxn.top

[D17] 最大值与最小值
来源：http://jgq.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://pxm.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://jqr.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tqj.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://hfq.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tcd.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ihs.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://xtc.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://jfl.yj202588.top

[D18] 扁平化嵌套数组
来源：http://cni.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wzj.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://aap.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jgc.shangyingyoupin.top

TS:   nested.flat();
来源：http://ueg.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://con.jiagoushi.top

Go:   // 手写双层循环
来源：http://xej.bbcook.cn

Ruby: nested.flatten
来源：http://axg.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ata.smart0.xyz

[D19] 按字段分组
来源：http://rne.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sui.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bzp.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ckk.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mzo.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bkv.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://ruy.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rmn.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zhm.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://jqe.yangfankeji.com

Py:   Counter(arr)
来源：http://qni.havefunace.top

PHP:  array_count_values($arr);
来源：http://ffg.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wso.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sxn.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://obv.redwolf501.top

Go:   // 手写 map[T]int
来源：http://zaf.jlsjyb.cn

Ruby: arr.tally
来源：http://rqj.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hpd.316326.xyz

[D21] 判断是否包含某元素
来源：http://jpk.nanxuanxn.top

Py:   x in arr
来源：http://tir.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://wkx.sufxvd.cn

JS:   arr.includes(x)
来源：http://shw.havefunace.top

TS:   arr.includes(x)
来源：http://xuv.ppjwa.cn

Java: list.contains(x)
来源：http://wxb.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://ync.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://jea.zhijiandao.cn

C#:   list.Contains(x)
来源：http://vsd.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://hvl.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ltq.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jfp.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pay.pengpengdd.cyou

TS:   [...arr];
来源：http://jjw.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://rff.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xqv.jinqigufen.top

Ruby: arr.dup;  arr.clone
来源：http://gwo.haohaochexian.top

C#:   new List<int>(list);
来源：http://nuu.fengsongda.top

[D23] reduce 累积计算
来源：http://zze.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pfu.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gey.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://waw.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hoa.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tcq.gotoacloud.top

Go:   // 手写循环
来源：http://ulf.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qjo.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://myp.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://wwz.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vln.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ydk.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zrv.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zcf.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yub.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vrs.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jtl.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pfk.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://sry.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eeq.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://omg.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fyk.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ssf.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mzu.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vym.quarkkingdee.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uor.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ciq.daria6918.cn

[D26] 数组转字符串
来源：http://sdh.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://eng.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://akt.yuxming.cn

JS:   arr.join(", ")
来源：http://pjw.daxiang520.top

TS:   arr.join(", ")
来源：http://kuw.pycfn.com

Java: String.join(", ", list)
来源：http://fdk.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://joy.ydzc1.top

Ruby: arr.join(", ")
来源：http://yap.yonumen.top

C#:   string.Join(", ", list)
来源：http://kpo.yj20258.top

================================================================================
来源：http://kmy.daxiang520.top

E. 字符串处理
来源：http://zmr.zhijiandao.cn

================================================================================
来源：http://lqn.xziqi.cn

[E01] 拼接字符串
来源：http://fqn.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uef.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://olg.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://biy.snrcjt.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yen.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mvd.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qdb.mhx1999.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ubu.kuanghao11.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zgh.shangyingyoupin.top

[E02] 重复字符串
来源：http://adl.xziqi.cn

Py:   "ab" * 3
来源：http://peg.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://pwk.yonumen.top

JS:   "ab".repeat(3)
来源：http://qji.yfazqb.com

TS:   "ab".repeat(3)
来源：http://sms.yangfankeji.com

Java: "ab".repeat(3)
来源：http://syv.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://ijg.sxryk.cn

Ruby: "ab" * 3
来源：http://ziz.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://obb.mhx1999.top

[E03] 截取子串
来源：http://kvo.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vkx.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mql.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://idj.andypj.xyz

TS:   s.slice(1, 4)
来源：http://yjb.nwbrower.top

Java: s.substring(1, 4)
来源：http://nki.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qox.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://syz.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://gdx.jlsjyb.cn

[E04] 查找子串位置
来源：http://kpu.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://lne.wangdashe.top

PHP:  strpos($s, "x");
来源：http://lbr.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ghw.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://dfw.c1oappe.top

Java: s.indexOf("x")
来源：http://bqf.yuxming.cn

Go:   strings.Index(s, "x")
来源：http://idy.kuanghao11.cn

Ruby: s.index("x")
来源：http://djm.ydzc1.top

C#:   s.IndexOf("x")
来源：http://yrw.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://gdr.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jkx.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mjm.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iqy.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://olo.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fii.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ddz.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tvj.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qyu.redwolf501.top

[E06] 替换子串
来源：http://cbx.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://etj.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://non.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mih.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://lsp.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yzy.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gwh.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ivb.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://lpv.aibaodan.cn

[E07] 按分隔符拆分
来源：http://trr.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vup.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sgv.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xie.chenlongwang.top

TS:   s.split(",")
来源：http://ifd.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vpk.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qhl.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://whz.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lwm.uphjek.com

[E08] 数组按分隔符合并
来源：http://nvm.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://enn.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://edr.tarul.cn

JS:   items.join(",")
来源：http://vlo.yangfankeji.com

TS:   items.join(",")
来源：http://hyi.yuxming.cn

Java: String.join(",", items)
来源：http://dtn.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://nfq.andypj.xyz

Ruby: items.join(",")
来源：http://xvq.hesvh.cn

C#:   string.Join(",", items)
来源：http://umb.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://zju.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gft.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://spt.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://qri.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://thl.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://acp.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xso.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://dwc.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rio.zdqjudy.top

[E10] 左侧补零 / 定长填充
来源：http://baw.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://egp.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aqq.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://mll.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://jjb.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://czm.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nrf.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vlq.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jig.hnxiangtu.top

[E11] 反转字符串
来源：http://xjf.zhoulong.xyz

Py:   s[::-1]
来源：http://geu.sxryk.cn

PHP:  strrev($s);
来源：http://qke.sweek.top

JS:   [...s].reverse().join("")
来源：http://wdv.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://uqj.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bsh.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kzi.nwbrower.top

Ruby: s.reverse
来源：http://wxc.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://hti.yvedp.cn

[E12] 统计某字符出现次数
来源：http://ghd.tanke756.top

Py:   s.count("a")
来源：http://ygj.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://rlj.cashguo.top

JS:   s.split("a").length - 1
来源：http://zhv.uphjek.com

TS:   s.split("a").length - 1
来源：http://bea.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dpd.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://lpd.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://axw.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://oto.jinqigfzy.top

[E13] 逐字符遍历
来源：http://jeu.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://fge.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yzq.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tjd.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tto.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wxc.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zxf.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://rqg.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://afq.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://wcy.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kwk.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xpw.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bxj.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://whw.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qab.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oox.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nsi.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qai.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://gxv.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uer.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ibq.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://imr.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fnt.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pab.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gaj.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://frv.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sss.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://vjr.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://ktc.cashguo.top

PHP:  number_format(1234567);
来源：http://bog.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gxk.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cti.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ysl.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mzg.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ory.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://mpu.yueranfly.top

[E17] 首字母大写
来源：http://nts.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yxy.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nfk.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ibw.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ecr.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xft.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ien.hongshengwenyu.top

Ruby: s.capitalize
来源：http://ydw.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bcf.vehdjk.com

[E18] 模板占位符替换
来源：http://zsn.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sni.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cwp.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://olw.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tgd.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vih.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://alp.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dhd.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://isp.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://gjw.yj20258.top

Py:   s.splitlines()
来源：http://zxv.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nmg.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://hou.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://awz.pycfn.com

Java: s.lines().toList()
来源：http://xqf.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://otw.jqgfzy.top

Ruby: s.lines
来源：http://pjg.haohaochexian.top

C#:   s.Split('\n')
来源：http://eyh.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://nhh.316326.xyz

Py:   if not s:
来源：http://euu.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://msp.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nix.jinqigfzy.top

TS:   if (s === "") {}
来源：http://nel.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://dxt.tanke756.top

Go:   if s == "" {}
来源：http://yzq.yj20258.top

Ruby: if s.empty?
来源：http://hhq.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://max.iojbl.cn

[E21] 超长截断加省略号
来源：http://zie.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://knx.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://drj.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztx.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oqy.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zav.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://ome.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://euj.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://skp.fktsv.cn

[E22] 字节长度与字符长度
来源：http://ozk.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cbf.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qib.nanxinkj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyk.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zmz.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zmf.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fig.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://dxa.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ckm.9152youxi.cn

================================================================================
来源：http://vow.mhx1999.top

F. 文件与目录
来源：http://nkp.jinqigufen.top

================================================================================
来源：http://dda.vehdjk.com

[F01] 读取整个文件
来源：http://jmk.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vow.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://ufs.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://khu.aizwys.cn


<!-- 参考信息 -->