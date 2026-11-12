代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://rns.hysaishi.cn

Go:   // 手写循环
来源：http://ela.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://mih.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://crq.ivvv.top

[D15] 去重
来源：http://auf.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eyw.ehwqpu.com

PHP:  array_unique($arr);
来源：http://oox.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://ssj.aizwys.cn

TS:   [...new Set(arr)]
来源：http://bbf.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hln.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://rda.yangfankeji.com

Ruby: arr.uniq
来源：http://nqm.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://pol.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://azy.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://svr.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nfn.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ewm.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ctq.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qak.yangfankeji.com

Go:   // 手写循环累加
来源：http://xad.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fai.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://pio.gogol.net.cn

[D17] 最大值与最小值
来源：http://hdn.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://snl.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://mgv.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kcz.fzhhl.top

TS:   Math.max(...arr);
来源：http://xsl.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://grb.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wdn.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://abl.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://xpd.jiagoushi.top

[D18] 扁平化嵌套数组
来源：http://klx.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wuc.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://ace.ivvv.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://izc.cheryme.top

TS:   nested.flat();
来源：http://vly.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vlf.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://zzc.tarul.cn

Ruby: nested.flatten
来源：http://qum.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://qnv.ydzc1.top

[D19] 按字段分组
来源：http://vtn.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://koq.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lgv.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hpj.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://gbo.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wwd.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://lvi.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://omj.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mxx.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://jad.hysaishi.cn

Py:   Counter(arr)
来源：http://zhx.redwolf501.top

PHP:  array_count_values($arr);
来源：http://fnw.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ymb.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bnz.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hmq.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://gcv.daxiang520.top

Ruby: arr.tally
来源：http://jci.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ccb.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://tnm.sysykeji.top

Py:   x in arr
来源：http://tno.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://dnt.zycfv.cn

JS:   arr.includes(x)
来源：http://gvj.zhongyouzk.top

TS:   arr.includes(x)
来源：http://ubb.smart0.xyz

Java: list.contains(x)
来源：http://qiq.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://ibr.hfpthk.cn

Ruby: arr.include?(x)
来源：http://ihh.xinyue.icu

C#:   list.Contains(x)
来源：http://pda.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://twv.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gfj.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cbn.svipenyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://muo.shzxlz.cn

TS:   [...arr];
来源：http://ivb.zycfv.cn

Java: new ArrayList<>(list);
来源：http://pfr.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kud.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://tux.yueranfly.top

C#:   new List<int>(list);
来源：http://ksv.aizwys.cn

[D23] reduce 累积计算
来源：http://gdv.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://syn.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ckw.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ocg.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xig.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hmk.pengpengdd.cyou

Go:   // 手写循环
来源：http://jgg.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://elx.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hni.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://fms.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://avk.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ogp.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fkv.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bzv.xziqi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eag.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nxg.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hlt.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qsg.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://jdj.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wor.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://onx.svipenyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ebt.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ggk.vqdsnc.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://osw.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uqh.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blw.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qda.sufxvd.cn

[D26] 数组转字符串
来源：http://vpz.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://nfn.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://csi.cdnleiting.top

JS:   arr.join(", ")
来源：http://ime.cqqwz.cn

TS:   arr.join(", ")
来源：http://yeb.dianchejie.cn

Java: String.join(", ", list)
来源：http://brc.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://edy.sufxvd.cn

Ruby: arr.join(", ")
来源：http://nvl.guannengcc.top

C#:   string.Join(", ", list)
来源：http://npn.feifeiyinyue.top

================================================================================
来源：http://eai.ivvv.top

E. 字符串处理
来源：http://zcu.dianchejie.cn

================================================================================
来源：http://vmu.tanke756.top

[E01] 拼接字符串
来源：http://fjd.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oty.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nnk.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jiw.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aoq.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://myy.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://crt.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://teo.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ftq.bjfxy.top

[E02] 重复字符串
来源：http://gqw.yueranfly.top

Py:   "ab" * 3
来源：http://rpm.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://hni.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://jnx.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://eyp.tanke756.top

Java: "ab".repeat(3)
来源：http://rtw.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://phc.guowangkeji.top

Ruby: "ab" * 3
来源：http://ptb.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nlk.daria6918.cn

[E03] 截取子串
来源：http://wdb.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cor.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hhg.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yhj.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://mtu.nwbrower.top

Java: s.substring(1, 4)
来源：http://rpw.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vjf.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://gyf.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://svr.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://wkv.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://ueo.aibaodan.cn

PHP:  strpos($s, "x");
来源：http://spx.cashguo.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jyg.svipenyu.cn

TS:   s.indexOf("x")
来源：http://roi.epnwcf.com

Java: s.indexOf("x")
来源：http://thw.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://uaa.vqdsnc.cn

Ruby: s.index("x")
来源：http://uvs.pycfn.com

C#:   s.IndexOf("x")
来源：http://wyh.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nem.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bmp.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ykv.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xdp.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ekr.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://djr.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xnl.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hfu.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kqf.hywenlv.cn

[E06] 替换子串
来源：http://qos.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dgh.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://glt.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://adq.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://gaq.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ocj.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uej.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vxa.cheryme.top

C#:   s.Replace("a", "b")
来源：http://wxv.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://nye.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zci.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bwc.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jfv.gzhubu.top

TS:   s.split(",")
来源：http://zvo.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://mya.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pvn.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://bwf.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yns.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://kik.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://mfc.yj20258888.top

PHP:  implode(",", $items);
来源：http://cvy.shzxlz.cn

JS:   items.join(",")
来源：http://rfg.tarul.cn

TS:   items.join(",")
来源：http://ovv.zhixingplan.top

Java: String.join(",", items)
来源：http://xun.pycfn.com

Go:   strings.Join(items, ",")
来源：http://fze.dashuyun.cn

Ruby: items.join(",")
来源：http://mey.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://dos.hammf.cn

[E09] 去除所有空白字符
来源：http://ftg.yongpay.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://osy.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uej.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://oqw.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://cwa.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://tkk.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ioh.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://njn.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mgu.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://irk.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tph.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nex.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://lcd.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://udx.sxryk.cn

Java: String.format("%03d", 7)
来源：http://vhg.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://roj.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nnu.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vjf.xziqi.cn

[E11] 反转字符串
来源：http://iaw.316326.xyz

Py:   s[::-1]
来源：http://hgl.fzhhl.top

PHP:  strrev($s);
来源：http://hri.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://soy.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://dtf.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mpp.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ksq.chenzaomai.com

Ruby: s.reverse
来源：http://cyz.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://imn.zhaomingkeji.xyz

[E12] 统计某字符出现次数
来源：http://oiv.zhixingplan.top

Py:   s.count("a")
来源：http://ebs.meibo888.top

PHP:  substr_count($s, "a");
来源：http://lfn.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://udn.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://ula.yvedp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xty.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://slh.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://suc.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://lhj.zdbjq.cn

[E13] 逐字符遍历
来源：http://buc.hysaishi.cn

Py:   for ch in s: print(ch)
来源：http://lbd.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ltl.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dwa.vehdjk.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://zqy.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iwr.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cut.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oak.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gae.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://clk.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ocg.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gmi.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vym.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iqa.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zdf.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gja.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://slx.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://njw.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://hay.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fir.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qmt.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rvy.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://upo.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vfs.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dvf.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jeg.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ybg.guannengcc.top

[E16] 数字千分位
来源：http://uks.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://lrt.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://fcg.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cxc.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zle.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kxa.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cln.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://omw.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://rmz.hfpthk.cn

[E17] 首字母大写
来源：http://oeg.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xuv.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://npa.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://knd.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xjg.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cwt.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bpx.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://luz.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hmw.wangdashe.top

[E18] 模板占位符替换
来源：http://fuu.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://exz.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fna.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tiz.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kun.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cud.uphjek.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dex.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hsb.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rsv.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://kvd.jlsjyb.cn

Py:   s.splitlines()
来源：http://bma.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://igw.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://tgp.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://jfb.ybcxt.top

Java: s.lines().toList()
来源：http://rkn.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://abg.snrcjt.cn

Ruby: s.lines
来源：http://gxk.sysykeji.top

C#:   s.Split('\n')
来源：http://pwk.aizwys.cn

[E20] 判断字符串是否为空
来源：http://apz.daxiang520.top

Py:   if not s:
来源：http://vvh.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dts.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dzt.birdmap.top

TS:   if (s === "") {}
来源：http://clz.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://bpd.pengpengdd.cyou

Go:   if s == "" {}
来源：http://mwq.zdqjudy.top

Ruby: if s.empty?
来源：http://uai.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://odf.jqgfzy.top

[E21] 超长截断加省略号
来源：http://hvd.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://llp.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vrw.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xtn.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jhf.guowangkeji.top


<!-- 参考信息 -->