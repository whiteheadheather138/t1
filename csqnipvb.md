代发 wailian999

TS:   [...new Set(arr)]
来源：http://dkv.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lte.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://slt.xziqi.cn

Ruby: arr.uniq
来源：http://dpr.pycfn.com

C#:   list.Distinct().ToList()
来源：http://jzo.wangdashe.top

[D16] 求和与平均值
来源：http://ahj.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mlt.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dua.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cwf.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdg.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mem.quarkkingdee.top

Go:   // 手写循环累加
来源：http://cwd.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nkc.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://hxz.fengsongda.top

[D17] 最大值与最小值
来源：http://tox.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://hdb.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://zmt.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hqk.aizwys.cn

TS:   Math.max(...arr);
来源：http://wry.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://hat.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wuq.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://jtf.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://yhl.chenjidiqi.icu

[D18] 扁平化嵌套数组
来源：http://phz.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hcn.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://irm.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qbo.gogol.net.cn

TS:   nested.flat();
来源：http://kok.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hsp.svipenyu.cn

Go:   // 手写双层循环
来源：http://gtl.vehdjk.com

Ruby: nested.flatten
来源：http://viz.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gga.sufxvd.cn

[D19] 按字段分组
来源：http://apw.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gdb.andypj.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mqv.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lnm.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://epf.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://epz.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://zaz.tianlin.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://qqa.shanyushiyangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ild.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://oqv.zhiwuduotai.top

Py:   Counter(arr)
来源：http://mra.zhijiandao.cn

PHP:  array_count_values($arr);
来源：http://gjk.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://esm.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lob.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://apo.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://hgo.smart0.xyz

Ruby: arr.tally
来源：http://fhp.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vfk.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://ebz.yanxiufei.cn

Py:   x in arr
来源：http://zue.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://oym.hnqzz.top

JS:   arr.includes(x)
来源：http://uba.zhengqikj.top

TS:   arr.includes(x)
来源：http://wqj.snrcjt.cn

Java: list.contains(x)
来源：http://uaj.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://fnj.yongpay.top

Ruby: arr.include?(x)
来源：http://eei.hysaishi.cn

C#:   list.Contains(x)
来源：http://rbl.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://iqv.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qhg.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mxy.xuetiantiany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jxq.sjlbkw.cn

TS:   [...arr];
来源：http://tlt.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://zdg.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yxy.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://byf.gzhubu.top

C#:   new List<int>(list);
来源：http://hyx.yj20258888.top

[D23] reduce 累积计算
来源：http://brm.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gjl.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dtn.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ckj.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pca.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mmk.iojbl.cn

Go:   // 手写循环
来源：http://dnr.ywan-chungtsiang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mik.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xdr.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://ckf.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kta.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vtx.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sqz.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sfm.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fji.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://exu.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ogv.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dro.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://axz.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mwe.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xef.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fkt.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jxa.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vsi.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ryt.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ivx.c1oappe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bho.cucudq.cn

[D26] 数组转字符串
来源：http://ylm.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://nlp.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://zfv.wangdashe.top

JS:   arr.join(", ")
来源：http://xot.chenzaomai.com

TS:   arr.join(", ")
来源：http://mcf.kuanghao11.cn

Java: String.join(", ", list)
来源：http://nqm.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://rej.yuxming.cn

Ruby: arr.join(", ")
来源：http://nzh.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://eom.zhongyouzk.top

================================================================================
来源：http://jrg.ydzc1.top

E. 字符串处理
来源：http://bvp.jlsjyb.cn

================================================================================
来源：http://wkp.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://qtp.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wqz.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gvv.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://acr.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dyt.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bql.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lbg.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lgz.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hmn.gogol.net.cn

[E02] 重复字符串
来源：http://fcq.shuidangran.top

Py:   "ab" * 3
来源：http://nzz.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://vmw.birdmap.top

JS:   "ab".repeat(3)
来源：http://kke.vehdjk.com

TS:   "ab".repeat(3)
来源：http://sya.yongpay.top

Java: "ab".repeat(3)
来源：http://sst.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://cys.bjfxy.top

Ruby: "ab" * 3
来源：http://rup.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cjz.tanke756.top

[E03] 截取子串
来源：http://mpw.zhoulong.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kwq.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xoj.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://enn.cqqwz.cn

TS:   s.slice(1, 4)
来源：http://cdd.gotoacloud.top

Java: s.substring(1, 4)
来源：http://fwj.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lly.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://qyq.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://tzv.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://fxb.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://adw.bjfxy.top

PHP:  strpos($s, "x");
来源：http://pwf.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ftu.yangfankeji.com

TS:   s.indexOf("x")
来源：http://pxo.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://sti.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://mce.hnqzz.top

Ruby: s.index("x")
来源：http://fuz.yuxming.cn

C#:   s.IndexOf("x")
来源：http://hhl.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kfb.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iia.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pvs.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mbb.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://svz.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ixc.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://auq.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ada.yj20258888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zhn.c1oappe.top

[E06] 替换子串
来源：http://kfd.xuanzx.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cfq.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://ihi.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pwg.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://cno.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xop.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vfy.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rbt.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://dfl.epnwcf.com

[E07] 按分隔符拆分
来源：http://ylr.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zmv.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://afb.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zxk.svipenyu.cn

TS:   s.split(",")
来源：http://rhz.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://npt.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dqc.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://eyh.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bkc.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://qhs.fzhhl.top

Py:   ",".join(items)
来源：http://ywq.jinyuanbaomall.cn

PHP:  implode(",", $items);
来源：http://zpr.iojbl.cn

JS:   items.join(",")
来源：http://bnv.ctjpmb.com

TS:   items.join(",")
来源：http://ovh.ctjpmb.com

Java: String.join(",", items)
来源：http://wzz.mhx1999.top

Go:   strings.Join(items, ",")
来源：http://vuj.zhoulong.xyz

Ruby: items.join(",")
来源：http://qbu.fktsv.cn

C#:   string.Join(",", items)
来源：http://dwl.birdmap.top

[E09] 去除所有空白字符
来源：http://usu.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://diz.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wdv.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://pad.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://rka.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://bcm.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nlr.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://wzq.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nzj.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://hzb.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://irk.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zum.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://mbg.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://gin.tarul.cn

Java: String.format("%03d", 7)
来源：http://bwd.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wum.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ypq.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zwe.mhx1999.top

[E11] 反转字符串
来源：http://xpt.zhijiandao.cn

Py:   s[::-1]
来源：http://zer.cashguo.top

PHP:  strrev($s);
来源：http://hef.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://qnk.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://gdj.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ujl.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lyd.tian-w.cn

Ruby: s.reverse
来源：http://aum.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://skj.epnwcf.com

[E12] 统计某字符出现次数
来源：http://yzn.uphjek.com

Py:   s.count("a")
来源：http://kkc.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://ely.yanxiufei.cn

JS:   s.split("a").length - 1
来源：http://kff.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://szx.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nuh.sweek.top

Go:   strings.Count(s, "a")
来源：http://mjr.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://vnl.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://dpo.havefunace.top

[E13] 逐字符遍历
来源：http://yih.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://lwg.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://egm.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://djz.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xns.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://njy.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://upg.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://csv.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://auc.sufxvd.cn

[E14] URL 编码与 Base64
来源：http://rwo.hesvh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yjc.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dsy.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cax.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cba.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wff.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://phz.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tuy.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jvx.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://rzg.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jtr.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hxb.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eut.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wli.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://glv.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hpe.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ouc.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tug.hnxiangtu.top

[E16] 数字千分位
来源：http://ugd.xuanzx.com

Py:   f"{1234567:,}"
来源：http://jzm.zhixingplan.top

PHP:  number_format(1234567);
来源：http://jhu.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hvk.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rhc.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mvz.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hsi.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iuy.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://bcj.sufxvd.cn

[E17] 首字母大写
来源：http://xfd.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fjy.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://zey.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hex.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vji.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://icl.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cfe.bbcook.cn

Ruby: s.capitalize
来源：http://tpk.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lpr.jlsjyb.cn

[E18] 模板占位符替换
来源：http://rxt.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://piw.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ljd.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mnv.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pzj.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gks.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jxc.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nbq.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jxx.yuxming.cn

[E19] 多行文本按行拆分
来源：http://ers.ydjk.org.cn

Py:   s.splitlines()
来源：http://clk.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tjm.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://vus.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://tab.cheryme.top

Java: s.lines().toList()
来源：http://keb.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://jip.ybcxt.top

Ruby: s.lines
来源：http://vwr.cqqwz.cn

C#:   s.Split('\n')
来源：http://qpq.yvedp.cn

[E20] 判断字符串是否为空
来源：http://mpn.jqgufenzy.top

Py:   if not s:
来源：http://hog.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hti.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eue.zhijiandao.cn

TS:   if (s === "") {}
来源：http://ggv.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://swx.meibo888.top

Go:   if s == "" {}
来源：http://whu.316326.xyz

Ruby: if s.empty?
来源：http://zkt.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vun.fktsv.cn

[E21] 超长截断加省略号
来源：http://cmy.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gud.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oyt.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zol.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jfi.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vsm.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://vah.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cum.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vjt.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://fvc.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ddv.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xut.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://koh.ywan-chungtsiang.top


<!-- 参考信息 -->