代发 wailian999

[D15] 去重
来源：http://wqk.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bzn.yvedp.cn

PHP:  array_unique($arr);
来源：http://rfs.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://eqc.aizwys.cn

TS:   [...new Set(arr)]
来源：http://pfr.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dri.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://iik.jiagoushi.top

Ruby: arr.uniq
来源：http://smn.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://wfe.xziqi.cn

[D16] 求和与平均值
来源：http://fww.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bbg.pycfn.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ywf.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cyx.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nzm.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tin.hfpthk.cn

Go:   // 手写循环累加
来源：http://snd.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://obv.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://jft.tanke756.top

[D17] 最大值与最小值
来源：http://mvn.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://vaf.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://kjp.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wto.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://qtx.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://enx.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zer.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://euq.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://vmt.daxiang520.top

[D18] 扁平化嵌套数组
来源：http://hfm.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://myu.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://pcz.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wcu.iojbl.cn

TS:   nested.flat();
来源：http://vgz.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ufi.sufxvd.cn

Go:   // 手写双层循环
来源：http://ntk.pengpengdd.cyou

Ruby: nested.flatten
来源：http://bnk.0kj1m.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gmf.kuanghao11.cn

[D19] 按字段分组
来源：http://eyw.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zjb.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nmj.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ffd.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pav.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ojv.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://lsa.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://gyu.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sys.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://amy.feifeiyinyue.top

Py:   Counter(arr)
来源：http://mcf.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://smu.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://njr.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wea.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dge.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://nuc.xinyue.icu

Ruby: arr.tally
来源：http://tpk.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xrs.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://fyn.c1oappe.top

Py:   x in arr
来源：http://aso.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://xem.yuxming.cn

JS:   arr.includes(x)
来源：http://amf.hysaishi.cn

TS:   arr.includes(x)
来源：http://dwl.hongshengwenyu.top

Java: list.contains(x)
来源：http://vwu.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://ndc.ehwqpu.com

Ruby: arr.include?(x)
来源：http://cee.zhijiandao.cn

C#:   list.Contains(x)
来源：http://ncq.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://akt.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://azq.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sxm.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oal.snrcjt.cn

TS:   [...arr];
来源：http://qep.sysykeji.top

Java: new ArrayList<>(list);
来源：http://ytl.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://zdv.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://cmi.sjlbkw.cn

C#:   new List<int>(list);
来源：http://led.xylfe.cn

[D23] reduce 累积计算
来源：http://dvz.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eps.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cid.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eju.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ngl.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dib.hesvh.cn

Go:   // 手写循环
来源：http://rct.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fgg.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eym.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://cqb.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mgd.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://llc.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aex.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wnt.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hxo.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ifo.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mkm.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://shv.shanyushiyangtech.top

[D25] Set 集合去重与交并差
来源：http://kmu.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mtt.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rys.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qqm.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qmw.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tzs.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hcl.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vpf.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://exx.cqqwz.cn

[D26] 数组转字符串
来源：http://vvy.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://msd.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://crt.andypj.xyz

JS:   arr.join(", ")
来源：http://owf.cashguo.top

TS:   arr.join(", ")
来源：http://rhk.yvedp.cn

Java: String.join(", ", list)
来源：http://ocq.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://asf.hywenlv.cn

Ruby: arr.join(", ")
来源：http://nmc.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://gml.jinghuilouyu.cn

================================================================================
来源：http://wwk.sufxvd.cn

E. 字符串处理
来源：http://jth.nanxinkj.top

================================================================================
来源：http://ivu.nanxinkj.top

[E01] 拼接字符串
来源：http://say.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rvq.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://afb.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://npe.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dir.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://asb.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uoh.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mxo.zhoulong.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cge.nanxinkj.top

[E02] 重复字符串
来源：http://ewm.hesvh.cn

Py:   "ab" * 3
来源：http://lzl.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://foo.cucudq.cn

JS:   "ab".repeat(3)
来源：http://mei.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://jpd.svipenyu.cn

Java: "ab".repeat(3)
来源：http://chr.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://ugd.jianghu66.top

Ruby: "ab" * 3
来源：http://sko.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lpy.jlsjyb.cn

[E03] 截取子串
来源：http://auc.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qcp.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://neo.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://csd.zdqjudy.top

TS:   s.slice(1, 4)
来源：http://hpm.ydzc1.top

Java: s.substring(1, 4)
来源：http://gfj.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jft.jqgfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://roz.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://wfe.ydzc1.top

[E04] 查找子串位置
来源：http://zfx.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://mtc.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://uun.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sln.yj20258.top

TS:   s.indexOf("x")
来源：http://llq.guannengcc.top

Java: s.indexOf("x")
来源：http://tiu.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://lwo.ivvv.top

Ruby: s.index("x")
来源：http://ouj.havefunace.top

C#:   s.IndexOf("x")
来源：http://nhe.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iuy.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rru.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://slj.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qvw.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pvj.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zdg.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jns.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sal.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bkx.zdqjudy.top

[E06] 替换子串
来源：http://fzv.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dns.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://ura.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gvx.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://deu.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xwh.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://igd.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mhp.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://qus.yvedp.cn

[E07] 按分隔符拆分
来源：http://pzc.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://add.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jvo.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ows.xuetiantiany.cn

TS:   s.split(",")
来源：http://yma.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://env.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://brr.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://jux.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nef.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://lpg.wangshuangyany.cn

Py:   ",".join(items)
来源：http://uhj.guannengcc.top

PHP:  implode(",", $items);
来源：http://uao.jinghuilouyu.cn

JS:   items.join(",")
来源：http://eie.zhijiandao.cn

TS:   items.join(",")
来源：http://uty.aibaodan.cn

Java: String.join(",", items)
来源：http://eqc.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://cep.hfpthk.cn

Ruby: items.join(",")
来源：http://qov.yuanzhike.top

C#:   string.Join(",", items)
来源：http://obe.kuanghao11.cn

[E09] 去除所有空白字符
来源：http://mfv.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wjn.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://agm.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://fkf.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://oac.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://zeg.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://mzu.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wcd.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zzj.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://pqy.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mve.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zya.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://cah.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://fzn.nwbrower.top

Java: String.format("%03d", 7)
来源：http://gmi.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://hbj.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ztx.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oth.fzhhl.top

[E11] 反转字符串
来源：http://fdo.bjfxy.top

Py:   s[::-1]
来源：http://jjo.9152youxi.cn

PHP:  strrev($s);
来源：http://dvs.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://cpe.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://tlu.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pro.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zkg.bjfxy.top

Ruby: s.reverse
来源：http://fue.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://iph.cucudq.cn

[E12] 统计某字符出现次数
来源：http://vdy.cucudq.cn

Py:   s.count("a")
来源：http://tdj.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://ool.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://zyn.52xcode.cn

TS:   s.split("a").length - 1
来源：http://dkj.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gjb.zdbjq.cn

Go:   strings.Count(s, "a")
来源：http://huj.ydjk.org.cn

Ruby: s.count("a")
来源：http://lee.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://vac.birdmap.top

[E13] 逐字符遍历
来源：http://qlm.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://jux.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://osk.redwolf501.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nmr.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pvc.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lix.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eji.cdnleiting.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hrp.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uja.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://lzp.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ozf.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qsj.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wmx.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://amr.quarkkingdee.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nmc.bjfxy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rfw.bbcook.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yex.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iln.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://vzi.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tmy.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ixs.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zlr.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yum.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sdv.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zrx.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ivt.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://imm.guowangkeji.top

[E16] 数字千分位
来源：http://dok.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://hgl.tanke756.top

PHP:  number_format(1234567);
来源：http://yej.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wka.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xqp.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fan.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dxd.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wwi.birdmap.top

C#:   1234567.ToString("N0")
来源：http://qqe.chenlongwang.top

[E17] 首字母大写
来源：http://jgn.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oug.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vvr.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vnq.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://psp.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://koa.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://txp.jlsjyb.cn

Ruby: s.capitalize
来源：http://rso.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nrp.xinyue.icu

[E18] 模板占位符替换
来源：http://ajd.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://owt.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pft.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ess.sweek.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yak.hcnkem.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eim.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gvg.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sjk.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://umv.guannengcc.top

[E19] 多行文本按行拆分
来源：http://byt.fzhhl.top

Py:   s.splitlines()
来源：http://leg.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hxs.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://hmq.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://xxq.yueranfly.top

Java: s.lines().toList()
来源：http://adu.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://drp.xinyue.icu

Ruby: s.lines
来源：http://quk.yuanzhike.top

C#:   s.Split('\n')
来源：http://nmg.fehbvm.com

[E20] 判断字符串是否为空
来源：http://xoc.hongshengwenyu.top

Py:   if not s:
来源：http://czw.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://avt.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fwy.quarkkingdee.top

TS:   if (s === "") {}
来源：http://zvs.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://gwi.quarkkingdee.top

Go:   if s == "" {}
来源：http://dmh.ehwqpu.com

Ruby: if s.empty?
来源：http://nif.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wqa.snrcjt.cn

[E21] 超长截断加省略号
来源：http://fdw.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uvs.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zks.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xsq.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sdf.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dst.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://mfy.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eqm.snrcjt.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://smm.zhongyouzk.top


<!-- 参考信息 -->