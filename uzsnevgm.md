代发 wailian999

[D15] 去重
来源：http://ahd.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oil.tian-w.cn

PHP:  array_unique($arr);
来源：http://ugw.jianghu66.top

JS:   [...new Set(arr)]
来源：http://dbs.smart0.xyz

TS:   [...new Set(arr)]
来源：http://zrh.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jqq.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://erj.daria6918.cn

Ruby: arr.uniq
来源：http://lgi.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://ews.ybcxt.top

[D16] 求和与平均值
来源：http://dzj.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jut.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jvn.jinqigfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bfu.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://quf.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://viv.nanxuanxn.top

Go:   // 手写循环累加
来源：http://sig.cdnleiting.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nxm.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://hzp.sysykeji.top

[D17] 最大值与最小值
来源：http://gjz.pycfn.com

Py:   max(arr);  min(arr)
来源：http://rsw.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://fgb.zdbjq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kbx.xylfe.cn

TS:   Math.max(...arr);
来源：http://duf.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://atu.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wby.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://tkk.sysykeji.top

C#:   list.Max();  list.Min()
来源：http://hvm.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://rjs.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pum.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://jwe.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xev.hcnkem.com

TS:   nested.flat();
来源：http://kbk.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kzi.shuidangran.top

Go:   // 手写双层循环
来源：http://aqd.zhoulong.xyz

Ruby: nested.flatten
来源：http://dsj.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kmj.jyoumei.cn

[D19] 按字段分组
来源：http://cse.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qoa.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fdd.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mnf.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mpa.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lzx.hammf.cn

Go:   // 手写 map[string][]T
来源：http://nfy.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oap.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nep.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://qrx.havefunace.top

Py:   Counter(arr)
来源：http://gnk.andypj.xyz

PHP:  array_count_values($arr);
来源：http://rym.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hhf.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kui.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jtt.uphjek.com

Go:   // 手写 map[T]int
来源：http://mvq.quarkkingdee.top

Ruby: arr.tally
来源：http://gdv.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ttr.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://opn.daria6918.cn

Py:   x in arr
来源：http://rkz.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://wpd.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://vcq.cucudq.cn

TS:   arr.includes(x)
来源：http://pxq.kuanghao11.cn

Java: list.contains(x)
来源：http://gbl.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://urm.ctjpmb.com

Ruby: arr.include?(x)
来源：http://hxc.epnwcf.com

C#:   list.Contains(x)
来源：http://scf.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://lwn.xuanzx.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dsb.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://epi.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uxy.cashguo.top

TS:   [...arr];
来源：http://hip.hnqzz.top

Java: new ArrayList<>(list);
来源：http://zfv.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pdh.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://inr.zhijiandao.cn

C#:   new List<int>(list);
来源：http://nlf.aizwys.cn

[D23] reduce 累积计算
来源：http://clz.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://onv.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vkt.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wzd.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tvr.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fqz.uphjek.com

Go:   // 手写循环
来源：http://mfx.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://isb.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xbw.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://bxb.yfazqb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hau.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://obl.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nze.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ipg.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://llg.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dul.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://amj.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pew.cashguo.top

[D25] Set 集合去重与交并差
来源：http://xtd.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ckd.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vbk.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://efo.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gfw.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cwn.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wtq.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://apo.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mdy.xinyue.icu

[D26] 数组转字符串
来源：http://ipf.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://fiu.havefunace.top

PHP:  implode(", ", $arr);
来源：http://mxi.tarul.cn

JS:   arr.join(", ")
来源：http://emz.hesvh.cn

TS:   arr.join(", ")
来源：http://ron.svipenyu.cn

Java: String.join(", ", list)
来源：http://kie.yuxming.cn

Go:   strings.Join(strs, ", ")
来源：http://sjr.jiagoushi.top

Ruby: arr.join(", ")
来源：http://zct.birdmap.top

C#:   string.Join(", ", list)
来源：http://hwq.yongpay.top

================================================================================
来源：http://qev.jqgufenzy.top

E. 字符串处理
来源：http://rca.hysaishi.cn

================================================================================
来源：http://lwp.shangyingyoupin.top

[E01] 拼接字符串
来源：http://dtw.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fio.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://osn.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://igt.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gil.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qkr.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zbe.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zcb.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gsz.jiagoushi.top

[E02] 重复字符串
来源：http://tah.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://mix.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://umg.xinyue.icu

JS:   "ab".repeat(3)
来源：http://xdj.zdbjq.cn

TS:   "ab".repeat(3)
来源：http://hvy.sufxvd.cn

Java: "ab".repeat(3)
来源：http://bhl.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://xkr.jinqigfzy.top

Ruby: "ab" * 3
来源：http://grh.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kpx.wangshuangyany.cn

[E03] 截取子串
来源：http://zad.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ffv.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ugb.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tmg.yj20258.top

TS:   s.slice(1, 4)
来源：http://zma.ybcxt.top

Java: s.substring(1, 4)
来源：http://dph.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://epz.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ter.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://rpp.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://qtv.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://erl.yfazqb.com

PHP:  strpos($s, "x");
来源：http://jsj.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://voz.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://jei.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://dzq.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://tdp.zdbjq.cn

Ruby: s.index("x")
来源：http://rdg.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://wmk.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ixq.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mpc.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://egn.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mux.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://nbx.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lpk.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hpf.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fnk.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wmd.tanke756.top

[E06] 替换子串
来源：http://eyq.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://arm.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://slz.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://trw.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://ndr.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sgd.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tgj.sxryk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://brc.yj202588.top

C#:   s.Replace("a", "b")
来源：http://gjg.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://kli.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pde.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://njb.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wuo.cqqwz.cn

TS:   s.split(",")
来源：http://pqv.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cde.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hxm.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://rhy.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yvs.yueranfly.top

[E08] 数组按分隔符合并
来源：http://isv.tanke756.top

Py:   ",".join(items)
来源：http://etd.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://hio.svipenyu.cn

JS:   items.join(",")
来源：http://qrn.pycfn.com

TS:   items.join(",")
来源：http://kzi.sysykeji.top

Java: String.join(",", items)
来源：http://njh.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://isb.zhoulong.xyz

Ruby: items.join(",")
来源：http://fmh.ppjwa.cn

C#:   string.Join(",", items)
来源：http://iss.havefunace.top

[E09] 去除所有空白字符
来源：http://iqk.sysykeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qcc.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rgw.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://jqm.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://jqz.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://lag.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kep.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://wsh.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uwn.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://cag.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ana.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vva.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://buc.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://ywg.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://zaf.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://vdu.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tfp.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ium.xuetiantiany.cn

[E11] 反转字符串
来源：http://xpn.hammf.cn

Py:   s[::-1]
来源：http://ufs.c1oappe.top

PHP:  strrev($s);
来源：http://ljr.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://gkk.haohaochexian.top

TS:   [...s].reverse().join("")
来源：http://vna.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wrw.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mgd.tianlin.xyz

Ruby: s.reverse
来源：http://zft.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://fwq.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://abr.jianghu66.top

Py:   s.count("a")
来源：http://awz.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://kez.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://iml.bbcook.cn

TS:   s.split("a").length - 1
来源：http://sks.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gaw.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://las.yonumen.top

Ruby: s.count("a")
来源：http://ggj.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://xcc.yuanzhike.top

[E13] 逐字符遍历
来源：http://xye.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://csm.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ekf.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uty.guowangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://eoi.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://opm.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mrh.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ecu.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://szj.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://kla.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vwf.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wnw.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ubw.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vcj.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://job.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://auj.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ion.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cri.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://mka.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xnl.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://okn.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ttp.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://off.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cxq.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mra.hammf.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sbo.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xcb.aizwys.cn

[E16] 数字千分位
来源：http://kth.xylfe.cn

Py:   f"{1234567:,}"
来源：http://ksg.hnqzz.top

PHP:  number_format(1234567);
来源：http://lqv.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://goo.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yur.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ecm.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sld.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rfe.yvedp.cn

C#:   1234567.ToString("N0")
来源：http://ked.jiagoushi.top

[E17] 首字母大写
来源：http://jwj.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tbq.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ttc.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxb.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oep.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uun.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pmk.haohaochexian.top

Ruby: s.capitalize
来源：http://knn.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tcp.9152youxi.cn

[E18] 模板占位符替换
来源：http://che.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zrn.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mfy.gotoacloud.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uiu.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kmq.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jec.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://txi.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://imr.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://omw.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://zex.jiagoushi.top

Py:   s.splitlines()
来源：http://ieo.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tjj.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://qif.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://twy.hfpthk.cn

Java: s.lines().toList()
来源：http://gxy.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://hel.zycfv.cn

Ruby: s.lines
来源：http://duk.hammf.cn

C#:   s.Split('\n')
来源：http://rlu.52xcode.cn

[E20] 判断字符串是否为空
来源：http://cby.dashuyun.cn

Py:   if not s:
来源：http://omi.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xqg.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pij.gaohongyu789.top

TS:   if (s === "") {}
来源：http://yei.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://zmv.wangdashe.top

Go:   if s == "" {}
来源：http://cld.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://cay.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vqy.tianlin.xyz

[E21] 超长截断加省略号
来源：http://glm.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xyo.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oez.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ssq.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ylp.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ghq.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://tbk.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hpc.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tqb.tianlin.xyz


<!-- 参考信息 -->