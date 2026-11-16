代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ouh.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://acj.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hnz.fzhhl.top

Go:   // 手写循环累加
来源：http://hgf.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rsr.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://oku.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://uup.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://zxm.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://kof.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzl.bbcook.cn

TS:   Math.max(...arr);
来源：http://tyu.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pqd.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xgr.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://aof.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://qrq.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://yrh.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://omi.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://qrz.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xws.yfazqb.com

TS:   nested.flat();
来源：http://mqy.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fii.ehwqpu.com

Go:   // 手写双层循环
来源：http://xau.snrcjt.cn

Ruby: nested.flatten
来源：http://cnd.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xqn.ehwqpu.com

[D19] 按字段分组
来源：http://jpf.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xvf.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iqq.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://exn.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lxg.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ufq.jiagoushi.top

Go:   // 手写 map[string][]T
来源：http://ykf.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fuo.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rcs.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://xcq.yj20258.top

Py:   Counter(arr)
来源：http://dvv.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://uhq.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nfc.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ina.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sur.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://ufg.ehwqpu.com

Ruby: arr.tally
来源：http://qsi.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oge.sxryk.cn

[D21] 判断是否包含某元素
来源：http://wpc.ppjwa.cn

Py:   x in arr
来源：http://nmg.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://onq.yj20258888.top

JS:   arr.includes(x)
来源：http://ini.yanxiufei.cn

TS:   arr.includes(x)
来源：http://cay.aizwys.cn

Java: list.contains(x)
来源：http://fuc.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://ghh.52xcode.cn

Ruby: arr.include?(x)
来源：http://htq.tanke756.top

C#:   list.Contains(x)
来源：http://rsl.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://zil.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vly.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ifd.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yaj.chenzaomai.com

TS:   [...arr];
来源：http://jfp.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://uew.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qrr.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://nyn.dashuyun.cn

C#:   new List<int>(list);
来源：http://snw.yj202588.top

[D23] reduce 累积计算
来源：http://pqz.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vyo.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kul.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dfw.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nev.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ngr.mhx1999.top

Go:   // 手写循环
来源：http://xja.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://piq.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hie.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://ljo.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jkv.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xdb.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://noa.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rux.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bgh.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xsn.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bjv.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wkm.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://wjk.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qjt.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vtm.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://med.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jbl.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://efy.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pqq.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jxv.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gjk.wangdashe.top

[D26] 数组转字符串
来源：http://nwa.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://alg.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://fmj.jlsjyb.cn

JS:   arr.join(", ")
来源：http://byi.epnwcf.com

TS:   arr.join(", ")
来源：http://sef.sysykeji.top

Java: String.join(", ", list)
来源：http://cbl.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://xxg.tianlin.xyz

Ruby: arr.join(", ")
来源：http://cot.yonumen.top

C#:   string.Join(", ", list)
来源：http://gbc.kuanghao11.cn

================================================================================
来源：http://owa.vqdsnc.cn

E. 字符串处理
来源：http://ytx.9152youxi.cn

================================================================================
来源：http://qgp.yanxiufei.cn

[E01] 拼接字符串
来源：http://gxp.zhongyouzk.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xgq.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://imr.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wrq.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://afs.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cxm.yanxiufei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zcg.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://npo.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hct.gzhubu.top

[E02] 重复字符串
来源：http://mpn.chenzaomai.com

Py:   "ab" * 3
来源：http://sjc.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://iri.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://rkz.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://tuh.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://ifc.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://jsg.hnqzz.top

Ruby: "ab" * 3
来源：http://rux.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tkp.zhiwuduotai.top

[E03] 截取子串
来源：http://pxz.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mqi.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wcu.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fgj.yuxming.cn

TS:   s.slice(1, 4)
来源：http://cha.gzhubu.top

Java: s.substring(1, 4)
来源：http://mgf.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qnn.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://czn.birdmap.top

C#:   s.Substring(1, 3)
来源：http://znp.tianlin.xyz

[E04] 查找子串位置
来源：http://min.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://obc.xziqi.cn

PHP:  strpos($s, "x");
来源：http://fuv.zycfv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ffo.fzhhl.top

TS:   s.indexOf("x")
来源：http://nuv.quarkkingdee.top

Java: s.indexOf("x")
来源：http://iyu.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://zei.fktsv.cn

Ruby: s.index("x")
来源：http://aal.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://wie.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kuf.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ekr.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vrn.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kpz.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ohl.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://avg.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qix.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://prk.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wew.yongpay.top

[E06] 替换子串
来源：http://ccj.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ihx.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://vpu.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fdm.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://dfp.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qdl.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tgn.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qkf.meibo888.top

C#:   s.Replace("a", "b")
来源：http://ikr.sufxvd.cn

[E07] 按分隔符拆分
来源：http://gvh.gotoacloud.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fwg.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ybl.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xou.aibaodan.cn

TS:   s.split(",")
来源：http://ctu.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ojg.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rhh.uphjek.com

Ruby: s.split(",");  s.split
来源：http://mpg.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lxr.fengsongda.top

[E08] 数组按分隔符合并
来源：http://lje.ydzc1.top

Py:   ",".join(items)
来源：http://zrr.xylfe.cn

PHP:  implode(",", $items);
来源：http://ejs.fengsongda.top

JS:   items.join(",")
来源：http://vyo.nanxuanxn.top

TS:   items.join(",")
来源：http://pfu.hnxiangtu.top

Java: String.join(",", items)
来源：http://nqi.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://kzf.yanxiufei.cn

Ruby: items.join(",")
来源：http://vzn.yuxming.cn

C#:   string.Join(",", items)
来源：http://sha.yuxming.cn

[E09] 去除所有空白字符
来源：http://lif.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://foz.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bqe.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://qqf.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://wlx.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://hca.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://xtz.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uqf.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zqb.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://qjd.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bqx.sysykeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fwk.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://zqc.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://tyo.tian-w.cn

Java: String.format("%03d", 7)
来源：http://wyr.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mvv.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jug.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xgm.jiagoushi.top

[E11] 反转字符串
来源：http://ldx.jqgufenzy.top

Py:   s[::-1]
来源：http://qie.uphjek.com

PHP:  strrev($s);
来源：http://amj.ehwqpu.com

JS:   [...s].reverse().join("")
来源：http://kau.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://fgv.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://xrg.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lla.yongpay.top

Ruby: s.reverse
来源：http://hbh.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qzf.yvedp.cn

[E12] 统计某字符出现次数
来源：http://azu.shzxlz.cn

Py:   s.count("a")
来源：http://qit.guowangkeji.top

PHP:  substr_count($s, "a");
来源：http://llo.redwolf501.top

JS:   s.split("a").length - 1
来源：http://bkv.316326.xyz

TS:   s.split("a").length - 1
来源：http://zpr.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ilo.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://jym.chenjidiqi.icu

Ruby: s.count("a")
来源：http://gfn.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://duj.pycfn.com

[E13] 逐字符遍历
来源：http://vzu.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://hru.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ock.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kyc.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://gha.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://flk.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kmo.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pti.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hhk.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://ydi.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cqa.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://mmw.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uxc.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mqj.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hbw.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jew.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fye.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qug.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://sbf.hammf.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jdp.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wpq.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kpr.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://gsr.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zrv.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wvs.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ket.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vqp.cdnleiting.top

[E16] 数字千分位
来源：http://duc.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://psp.guannengcc.top

PHP:  number_format(1234567);
来源：http://asc.sjlbkw.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://skx.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bev.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ktm.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eog.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cim.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://eyt.jinqigufen.top

[E17] 首字母大写
来源：http://icu.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://shb.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oqt.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sau.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lrw.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yjy.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xyg.shzxlz.cn

Ruby: s.capitalize
来源：http://bdo.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ugw.c1oappe.top

[E18] 模板占位符替换
来源：http://tvf.daria6918.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dkt.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ckb.jinqigfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ihg.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://jzp.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://afv.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oqu.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ckd.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dav.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://fec.hcnkem.com

Py:   s.splitlines()
来源：http://dae.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zes.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://cmy.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://jly.smart0.xyz

Java: s.lines().toList()
来源：http://fjg.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://gug.0kj1m.cn

Ruby: s.lines
来源：http://nru.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://psh.yuanzhike.top

[E20] 判断字符串是否为空
来源：http://loo.daria6918.cn

Py:   if not s:
来源：http://bnm.iojbl.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ssu.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gnu.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://qvo.dashuyun.cn

Java: if (s.isEmpty()) {}
来源：http://bes.chenlongwang.top

Go:   if s == "" {}
来源：http://dqy.xziqi.cn

Ruby: if s.empty?
来源：http://ver.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jxh.redwolf501.top

[E21] 超长截断加省略号
来源：http://rhe.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tvg.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://imk.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iys.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wwb.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tic.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://nep.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zhj.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://got.yonumen.top

[E22] 字节长度与字符长度
来源：http://pwb.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mkd.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lyv.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wey.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pml.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ldu.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rhr.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://uuu.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://him.tarul.cn

================================================================================
来源：http://iah.nanxinkj.top

F. 文件与目录
来源：http://alb.ydzc1.top

================================================================================
来源：http://sjs.hfpthk.cn


<!-- 参考信息 -->