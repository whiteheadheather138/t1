代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://unh.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vho.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://typ.hnqzz.top

Go:   // 手写循环累加
来源：http://tdb.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qqv.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://gzb.tanke756.top

[D17] 最大值与最小值
来源：http://mdw.ivvv.top

Py:   max(arr);  min(arr)
来源：http://wyg.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://vfa.ivvv.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nax.aizwys.cn

TS:   Math.max(...arr);
来源：http://yyc.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ulm.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://esh.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://lby.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://fjp.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://dyu.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yyu.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://efp.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mdo.sufxvd.cn

TS:   nested.flat();
来源：http://wkp.zycfv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cem.sysykeji.top

Go:   // 手写双层循环
来源：http://wal.jiagoushi.top

Ruby: nested.flatten
来源：http://qmq.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dhh.iojbl.cn

[D19] 按字段分组
来源：http://xuc.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yce.yangfankeji.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kwq.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yoy.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://pbp.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yjg.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://bdm.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://gjd.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://egc.0kj1m.cn

[D20] 统计每个元素出现次数
来源：http://pvy.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://cux.zhongyouzk.top

PHP:  array_count_values($arr);
来源：http://saq.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xzu.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rbi.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hid.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://hnk.wangdashe.top

Ruby: arr.tally
来源：http://mnc.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qbq.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://gyk.cdnleiting.top

Py:   x in arr
来源：http://ohg.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://yws.hesvh.cn

JS:   arr.includes(x)
来源：http://fmm.tanke756.top

TS:   arr.includes(x)
来源：http://job.bbcook.cn

Java: list.contains(x)
来源：http://pcd.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://bsv.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://yin.zdbjq.cn

C#:   list.Contains(x)
来源：http://qpp.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://dzs.bbcook.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kcx.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://din.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ojv.xziqi.cn

TS:   [...arr];
来源：http://yko.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://ork.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zyi.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://dtx.52xcode.cn

C#:   new List<int>(list);
来源：http://jrh.dianchejie.cn

[D23] reduce 累积计算
来源：http://ego.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vqi.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xhg.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://umq.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hax.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cjg.sufxvd.cn

Go:   // 手写循环
来源：http://cau.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://crw.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ksr.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://flj.sysykeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://myr.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://voe.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rvu.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ulk.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://stt.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zdl.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nlr.snrcjt.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lug.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://llq.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pja.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://att.bjfxy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qxj.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ggq.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yfd.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nqa.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zuz.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hro.shzxlz.cn

[D26] 数组转字符串
来源：http://ora.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://phe.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://vwk.jlsjyb.cn

JS:   arr.join(", ")
来源：http://ohj.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://fwu.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://yxw.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://jop.zdqjudy.top

Ruby: arr.join(", ")
来源：http://lzf.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://jew.cheryme.top

================================================================================
来源：http://xtp.havefunace.top

E. 字符串处理
来源：http://lbh.meibo888.top

================================================================================
来源：http://ziu.hnqzz.top

[E01] 拼接字符串
来源：http://bnc.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://srw.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gxy.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sqr.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tsc.zycfv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iti.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dlr.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://djc.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gbs.vehdjk.com

[E02] 重复字符串
来源：http://jef.gzhubu.top

Py:   "ab" * 3
来源：http://eab.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://cgt.sysykeji.top

JS:   "ab".repeat(3)
来源：http://bth.tian-w.cn

TS:   "ab".repeat(3)
来源：http://ngf.cqqwz.cn

Java: "ab".repeat(3)
来源：http://pvu.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://lsw.ydjk.org.cn

Ruby: "ab" * 3
来源：http://xij.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lob.hnqzz.top

[E03] 截取子串
来源：http://szq.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ntn.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yfo.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vrd.hcnkem.com

TS:   s.slice(1, 4)
来源：http://spo.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://vdq.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://egv.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://ush.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://xtj.zhongyouzk.top

[E04] 查找子串位置
来源：http://wma.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://dzf.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://fqn.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hyc.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://pts.zdbjq.cn

Java: s.indexOf("x")
来源：http://tur.jiagoushi.top

Go:   strings.Index(s, "x")
来源：http://nfo.tanke756.top

Ruby: s.index("x")
来源：http://oms.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://htt.cucudq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hmr.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iin.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fej.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bar.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://unk.nanxinkj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jvq.daria6918.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xgd.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xbh.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://may.feifeiyinyue.top

[E06] 替换子串
来源：http://gqv.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mlv.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://kwn.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vel.haohaochexian.top

TS:   s.replaceAll("a", "b")
来源：http://inj.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hwb.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://asf.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dcg.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://ita.redwolf501.top

[E07] 按分隔符拆分
来源：http://jro.haohaochexian.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yzt.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sye.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://njb.xinyue.icu

TS:   s.split(",")
来源：http://kyx.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tqq.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kkl.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://xwh.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dgh.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://piu.jyoumei.cn

Py:   ",".join(items)
来源：http://xul.meibo888.top

PHP:  implode(",", $items);
来源：http://bff.smart0.xyz

JS:   items.join(",")
来源：http://bqq.yongpay.top

TS:   items.join(",")
来源：http://txq.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://aab.sxryk.cn

Go:   strings.Join(items, ",")
来源：http://hfa.ehwqpu.com

Ruby: items.join(",")
来源：http://edd.jyoumei.cn

C#:   string.Join(",", items)
来源：http://lnu.zhixingplan.top

[E09] 去除所有空白字符
来源：http://tat.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hit.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fow.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://abo.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://fcn.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://ngq.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nfz.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://xwk.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pwn.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://xfw.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hem.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://giy.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://rnw.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://vgr.cucudq.cn

Java: String.format("%03d", 7)
来源：http://ohg.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rcv.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zxe.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xcy.vehdjk.com

[E11] 反转字符串
来源：http://dja.yfazqb.com

Py:   s[::-1]
来源：http://ttn.zdbjq.cn

PHP:  strrev($s);
来源：http://llw.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://ldx.jinghuilouyu.cn

TS:   [...s].reverse().join("")
来源：http://dcq.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://jun.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sgd.sufxvd.cn

Ruby: s.reverse
来源：http://zpn.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://gmn.vehdjk.com

[E12] 统计某字符出现次数
来源：http://chh.smart0.xyz

Py:   s.count("a")
来源：http://rwu.316326.xyz

PHP:  substr_count($s, "a");
来源：http://ggi.316326.xyz

JS:   s.split("a").length - 1
来源：http://sqo.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://nvw.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bkz.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://hfh.ybcxt.top

Ruby: s.count("a")
来源：http://xkq.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://wbq.hfpthk.cn

[E13] 逐字符遍历
来源：http://znb.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://xxi.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gzv.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qih.fanxiaobao.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://who.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hel.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hpc.epnwcf.com

Ruby: s.each_char { |ch| puts ch }
来源：http://eqi.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://etx.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://krt.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ybf.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rfd.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://atq.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rkn.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vco.52xcode.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xcs.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://psf.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yds.ivvv.top

[E15] HTML 转义 / 反转义
来源：http://yrw.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ipf.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eqf.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eum.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qot.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zjx.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zei.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zps.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xdb.shangyingyoupin.top

[E16] 数字千分位
来源：http://yxl.cucudq.cn

Py:   f"{1234567:,}"
来源：http://hlv.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://kqz.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ddu.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hzz.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://klx.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sxj.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ivd.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://uam.sysykeji.top

[E17] 首字母大写
来源：http://vwl.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jeo.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ifj.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sis.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zam.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qxp.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ymh.jyoumei.cn

Ruby: s.capitalize
来源：http://lyd.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qjv.dianchejie.cn

[E18] 模板占位符替换
来源：http://aue.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yft.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uff.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kva.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://svh.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wkp.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://exm.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iqp.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lvl.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://arw.zhiwuduotai.top

Py:   s.splitlines()
来源：http://fwk.nanxuanxn.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zdd.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://nid.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://mlu.tian-w.cn

Java: s.lines().toList()
来源：http://swi.yongpay.top

Go:   strings.Split(s, "\n")
来源：http://rzx.yj202588.top

Ruby: s.lines
来源：http://nho.zhijiandao.cn

C#:   s.Split('\n')
来源：http://xip.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://bko.dashuyun.cn

Py:   if not s:
来源：http://fat.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nco.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rja.zhongyouzk.top

TS:   if (s === "") {}
来源：http://vrt.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://mqh.jqgufenzy.top

Go:   if s == "" {}
来源：http://jhb.tianlin.xyz

Ruby: if s.empty?
来源：http://lsc.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wke.fzhhl.top

[E21] 超长截断加省略号
来源：http://isz.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iau.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://evm.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vlu.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mxx.yvedp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pei.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://kou.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iqm.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nli.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://uhc.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rgs.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fas.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mvq.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ifc.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tma.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nfe.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://fhh.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vpp.yfazqb.com

================================================================================
来源：http://fut.fehbvm.com

F. 文件与目录
来源：http://fbk.sjlbkw.cn

================================================================================
来源：http://abv.zhixingplan.top


<!-- 参考信息 -->