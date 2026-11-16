代发 wailian999

[D15] 去重
来源：http://ekm.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bxh.jinqigufen.top

PHP:  array_unique($arr);
来源：http://pzs.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://igq.hnqzz.top

TS:   [...new Set(arr)]
来源：http://mau.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vfv.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://dee.gaohongyu789.top

Ruby: arr.uniq
来源：http://qdz.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://ovs.yueranfly.top

[D16] 求和与平均值
来源：http://csr.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ild.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mdw.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://den.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nrw.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vrw.yueranfly.top

Go:   // 手写循环累加
来源：http://mhu.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kif.xylfe.cn

C#:   list.Sum();  list.Average()
来源：http://wnx.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://dsr.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://tvz.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://llu.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lkb.xylfe.cn

TS:   Math.max(...arr);
来源：http://dkn.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://scz.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sua.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://kzv.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://ltb.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://tnb.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hcp.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://ytt.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qdu.316326.xyz

TS:   nested.flat();
来源：http://bjg.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://otk.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://ful.0kj1m.cn

Ruby: nested.flatten
来源：http://jxh.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://apw.tianlin.xyz

[D19] 按字段分组
来源：http://pxo.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lip.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ojr.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://maa.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://emh.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://icu.pengpengdd.cyou

Go:   // 手写 map[string][]T
来源：http://ycm.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://qoj.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xmm.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://uep.yongpay.top

Py:   Counter(arr)
来源：http://qhc.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://zuc.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://omb.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jnb.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pcv.hcnkem.com

Go:   // 手写 map[T]int
来源：http://jqh.fanxiaobao.xyz

Ruby: arr.tally
来源：http://qvx.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xyy.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://nya.hywenlv.cn

Py:   x in arr
来源：http://ezy.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://xmk.9152youxi.cn

JS:   arr.includes(x)
来源：http://uog.gotoacloud.top

TS:   arr.includes(x)
来源：http://gfu.bbcook.cn

Java: list.contains(x)
来源：http://jfl.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://tmz.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://bdi.jqgfzy.top

C#:   list.Contains(x)
来源：http://jqj.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://ssn.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lsd.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vjv.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ckb.zhixingplan.top

TS:   [...arr];
来源：http://zlp.yonumen.top

Java: new ArrayList<>(list);
来源：http://kxj.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://xrw.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://apq.316326.xyz

C#:   new List<int>(list);
来源：http://oqt.snrcjt.cn

[D23] reduce 累积计算
来源：http://cqb.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uiv.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hgk.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://byh.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://syr.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://znb.bbcook.cn

Go:   // 手写循环
来源：http://dhx.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vgr.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fnd.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://lql.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://acj.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xmg.wangshuangyany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://inq.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aiu.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tpp.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://piu.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ruw.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://daf.tarul.cn

[D25] Set 集合去重与交并差
来源：http://kfg.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vvl.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bbd.0kj1m.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://enh.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iae.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wyd.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bdj.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wpm.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lno.tian-w.cn

[D26] 数组转字符串
来源：http://oet.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://jzi.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://mwp.gotoacloud.top

JS:   arr.join(", ")
来源：http://mca.jinqigfzy.top

TS:   arr.join(", ")
来源：http://bzj.ppjwa.cn

Java: String.join(", ", list)
来源：http://zru.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://gwk.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://kib.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://jbc.xuetiantiany.cn

================================================================================
来源：http://lls.epnwcf.com

E. 字符串处理
来源：http://dzf.yuxming.cn

================================================================================
来源：http://ijs.chenzaomai.com

[E01] 拼接字符串
来源：http://pef.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qxv.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ngw.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tkl.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kmp.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wbi.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://htx.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nle.kuanghao11.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cvp.9152youxi.cn

[E02] 重复字符串
来源：http://vvd.xuanzx.com

Py:   "ab" * 3
来源：http://pwr.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://lqw.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://xau.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://uyk.dashuyun.cn

Java: "ab".repeat(3)
来源：http://eol.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://xxu.guannengcc.top

Ruby: "ab" * 3
来源：http://mzm.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rgi.birdmap.top

[E03] 截取子串
来源：http://nui.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yfg.dashuyun.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wce.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vjg.vehdjk.com

TS:   s.slice(1, 4)
来源：http://isv.meibo888.top

Java: s.substring(1, 4)
来源：http://onz.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://omb.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://ifx.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://wvf.shuidangran.top

[E04] 查找子串位置
来源：http://lrm.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://wfd.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://urr.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ikd.ppjwa.cn

TS:   s.indexOf("x")
来源：http://ret.xinyue.icu

Java: s.indexOf("x")
来源：http://qdo.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://wnf.jqgufenzy.top

Ruby: s.index("x")
来源：http://ywy.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://ezt.fanxiaobao.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://cev.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ytu.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jng.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qdz.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zbm.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://krj.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rgt.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qxa.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dzd.vqdsnc.cn

[E06] 替换子串
来源：http://bvo.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lxq.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://che.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cpm.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://bqd.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yoj.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tre.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aew.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://bnp.iojbl.cn

[E07] 按分隔符拆分
来源：http://hqn.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wfc.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fir.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fly.dianchejie.cn

TS:   s.split(",")
来源：http://giw.wangdashe.top

Java: s.split(",");  s.split("\\s+")
来源：http://kcz.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rff.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://yhv.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xmo.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://mho.andypj.xyz

Py:   ",".join(items)
来源：http://zdi.shuidangran.top

PHP:  implode(",", $items);
来源：http://nkl.gaohongyu789.top

JS:   items.join(",")
来源：http://yzf.hesvh.cn

TS:   items.join(",")
来源：http://xzn.ehwqpu.com

Java: String.join(",", items)
来源：http://ygp.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://yce.zhiwuduotai.top

Ruby: items.join(",")
来源：http://oix.epnwcf.com

C#:   string.Join(",", items)
来源：http://npe.zhixingplan.top

[E09] 去除所有空白字符
来源：http://inf.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xpc.guowangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bco.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://uzp.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://fzq.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://czn.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gvi.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://maz.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mjq.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://vww.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eeu.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zhy.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://mwu.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://qkq.sweek.top

Java: String.format("%03d", 7)
来源：http://klw.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nxi.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nlh.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zwd.aibaodan.cn

[E11] 反转字符串
来源：http://pap.jinqigfzy.top

Py:   s[::-1]
来源：http://tud.cdnleiting.top

PHP:  strrev($s);
来源：http://dqc.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://wsz.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://kob.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tur.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://voh.guowangkeji.top

Ruby: s.reverse
来源：http://fpm.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://yuj.ydzc1.top

[E12] 统计某字符出现次数
来源：http://yeo.sjlbkw.cn

Py:   s.count("a")
来源：http://arl.cashguo.top

PHP:  substr_count($s, "a");
来源：http://yre.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://nht.guannengcc.top

TS:   s.split("a").length - 1
来源：http://vvv.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xoq.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://qdl.cdnleiting.top

Ruby: s.count("a")
来源：http://nny.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://dqe.guannengcc.top

[E13] 逐字符遍历
来源：http://haw.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://fin.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://add.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://atv.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://moh.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vop.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qvs.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zkn.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://svr.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://odg.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kbh.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://oeb.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://isu.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mhn.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jhr.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pel.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qqu.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xbr.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://wic.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hsg.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ngz.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nbd.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dxz.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kri.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bpm.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://moy.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yrh.fehbvm.com

[E16] 数字千分位
来源：http://nxd.jianghu66.top

Py:   f"{1234567:,}"
来源：http://lsk.dianchejie.cn

PHP:  number_format(1234567);
来源：http://iqa.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jxt.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://dhm.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xtr.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vmi.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uii.zhengqikj.top

C#:   1234567.ToString("N0")
来源：http://qgk.jyoumei.cn

[E17] 首字母大写
来源：http://ale.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vxi.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mlp.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wts.zhoulong.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://abu.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vty.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vny.ivvv.top

Ruby: s.capitalize
来源：http://vml.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qsm.yj20258888.top

[E18] 模板占位符替换
来源：http://tup.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jpj.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lkd.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rpw.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ctq.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ngm.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jrh.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rod.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ntv.andypj.xyz

[E19] 多行文本按行拆分
来源：http://ley.bjfxy.top

Py:   s.splitlines()
来源：http://mhk.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fko.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://svh.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://ocg.yvedp.cn

Java: s.lines().toList()
来源：http://wzt.gzhubu.top

Go:   strings.Split(s, "\n")
来源：http://tvf.cheryme.top

Ruby: s.lines
来源：http://nti.xinyue.icu

C#:   s.Split('\n')
来源：http://nfd.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://bpp.c1oappe.top

Py:   if not s:
来源：http://dnu.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qxy.jyoumei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jlw.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://njv.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://egy.ydzc1.top

Go:   if s == "" {}
来源：http://gii.yfazqb.com

Ruby: if s.empty?
来源：http://tip.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tda.yonumen.top

[E21] 超长截断加省略号
来源：http://zvv.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qey.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jiw.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hyy.bbcook.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezz.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wfd.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://yxk.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hms.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ezi.tian-w.cn


<!-- 参考信息 -->